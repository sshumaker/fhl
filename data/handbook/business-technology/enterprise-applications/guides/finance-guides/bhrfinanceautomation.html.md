WIP

# How the Integration Works:

- The integration is powered around the Policy Matrix, which determines how the employee’s user record in Expensify and Netsuite should be set up.
   - Based on an Employee’s Location, Department and Currency, that will determine which Netsuite Subsidiary to assign them to and which Expensify Policy to add them to.
- The integration is triggered by any new or updated employees in BambooHR.
   - This could result in a job being run even if there isn’t a necessary change to the employee’s Netsuite or Expensify record, which is fine. It’s better that than missing an update.
- Every _**Five**_ minutes, the integration takes the new and updates employees and updates Netsuite and Expensify in that order.
It will first validate that all the necessary data is there on the Employee record.
   - Necessary Data: Name, Email, Manager, Location, Currency, Department.
   - If any of that data is missing, job will stop and it will throw an error.
- Integration will first create or update Netsuite.
   - Updates to Employee Vendor Record based on the BHR ID and Email fields.
       - Will update Name, Email, Currency, Department and BHR ID
   - If Employee’s Subsidiary changes, a new vendor will be created and nothing will happen to the old vendor record.
      - Accounts Payable team will need to deactivate manually.
- Once Netsuite is complete, it will then move onto Expensify.
   - Based on an Employee’s Location, Department and Currency, that will determine which Netsuite Subsidiary to assign them to and which Expensify Policy to add them to.
    - It will also evaluate the Employee’s manager details to determine if they need to also be added to the Expensify policy in order to approve their reportee’s expense reports.
- If it is able to successfully action in Netsuite and Expensify then it will return a success, otherwise it will retry twice, if it still fails it will proceed to generate an error (see next section)

# Error Handling:
- Errors will be summarized daily and dropped into a Google Sheet and should be resolved timely.
   - There are 6 different types of errors
      - Sid’s direct reports: Because Sid doesn’t have a manager, there is a step in the Integration that evaluates an Employee’s Manager’s Manager, so that step will fail for Sid, since he doesn’t have a manager in BambooHR (rightfully so).


# Maintenance:

### **BambooHR: Location Creation/Changes**
   - If the business decides to rename/repurpose an existing Location in BHR, the HR team should cc FinanceOps in the ticket, so the integration can be updated accordingly.
      - If they don’t, the risk is a delay in updating and adding employees to Expensify and Netsuite, but they will be captured in the daily error log and actioned then.

### **Expensify Policy Creation/Changes:**
 Courtney Cote to notify the EntApps: FinSys team in their tickets, by CC’ing FinanceOps, so the integration can be updated accordingly. This is a proactive measure, so if it doesn’t happen then we’ll encounter more errors than usual.
