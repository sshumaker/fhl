---
layout: markdown_page
title: "Evolution Workflow"
---

As engineers at GitLab, we lead the **evolution** of software, constantly
working to find the right balance between proactive work, reactive work,
and innovation. We strive to determine what work is important
and what work is not, leveraging knowledge from those that know the most about
GitLab, and empowering people to work on things that make everyone more
productive. Experimenting and innovating are core to how we work, and **we
focus on collaboration, results and iteration** to achieve our goals.

With growth, however, comes complexity. An organic approach to our work
sometimes requires help to ensure we are most effective. Help may be in the
form of validating our technical approaches, ensuring organizational alignment
across teams and departments, and driving priorities to key decision makers.
**Technical Engineering Leaders take on the task of helping engineers through
these challenges**. The **Architecture Evolution Workflow** is intended to
provide influence amplification and iteration framework to drive the solution
of complex problems both technically and organizationally.

## Blueprints

Blueprints are the primary artifact that the workflow revolves around.
They are version controlled documents that are released alongside our
[user-facing documentation](https://gitlab.com/gitlab-org/gitlab/-/tree/master/doc/architecture/blueprints).

Long-term iterations, either on features or complex architectural changes, are
challenging because it is easy to lose consensus, conceptual integrity,
architectural consistency, or alignment in why and how we are doing something.

A blueprint describes a technical vision and a set of principles that evolve as
we move forward. It acts as guardrails to keep team aligned. A blueprint gets
constantly updated with new insights and knowledge, after every iteration, to
become even more useful as we make progress with implementing it.

### Why are blueprints tracked?

Blueprints are tracked as version controlled documents. This enables anyone to propose
changes in the form of merge requests. By doing so we can ensure that:

- there is always a single document that represents the current state of a given proposal
- you do not have to traverse multiple issues or threaded discussions to grok our direction
- feedback can be given and applied in the form of concrete suggestions

### Does my thing require a blueprint?

A blueprint is required for changes that meet any of the following conditions:

- a blog post would be written about after its release
- requires coordination across multiple functions
- could impact overall system stability
- requires significant effort or changes GitLab in a significant way
  (ex. something that would take 10 person-weeks to implement,
  introduce or redesign a system component, or introduces API changes)
- impacts the operation of GitLab substantially, will require manual upgrades,
  or introduce special handling across distributions and deployments
- adds a new service outside of the rails monolith, or an additional data source.

Invoking this workflow is unnecessary if:

- fixing a flaky test
- minor refactoring of code
- performance improvements, which are only visible to users as faster API operations
- upgrading API-compatible versions of dependencies

## Workflow: TL;DR

As an engineer, you and your manager determine whether to invoke the
Architecture Evolution Workflow. When in doubt, do not hesitate to reach out to
a Principal+ Engineer for input.

1. Determine with your manager whether to invoke the workflow.
1. Start writing a blueprint somewhere! Depending on whether the content can be
   considered [SAFE](/handbook/legal/safe-framework/) or not you may want to do
   that in a private space first. If you don't know how what content to start
   with you can use [a template](https://gitlab.com/gitlab-org/gitlab/-/blob/master/doc/architecture/blueprints/_template.md?plain=1).
1. Post a link to your blueprint with a brief description in the internal
   [`#architecture`](https://gitlab.slack.com/archives/CJ4DB7517) channel on Slack.
1. Involve Architecture Evolution Coach, a Principal+ Engineer who will
   support you throughout the process.
1. Open an architecture evolution blueprint [merge request](https://gitlab.com/gitlab-org/gitlab/-/tree/master/doc/architecture/blueprints)
   if you have not done it already.
1. Work with Architecture Evolution Coach, a Product Manager, Engineering
   Manager, and Domain Experts to get the blueprint properly reviewed,
   commented, refined, and eventually merged!

### Getting things done

Once your blueprint has been merged you can start collaborating with the DRIs
to get the work done in a way that seems best for everyone involved.

The blueprint is an artifact that accompanies you during the implementation
journey. After each iteration you can get back to it, to update it with the
current state of the architectural initiative.

## Workflow: The Detailed View

### Proposing changes

Anyone can propose a change they believe we should work on.  When these changes
turn out to be too intricate for a single individual contributor to handle
(complex backstage improvements, architectural changes, productivity or
efficiency improvements), or they span multiple iterations or teams, it may be
helpful to invoke the Architecture Evolution Workflow, as the change may not be
something directly actionable.

The issue author collaborates with the Architecture Evolution Coach to involve
the right people and reach the right decision makes, DRIs, domain experts, and
other stakeholders.

### Amplifying your influence

![influence](/handbook/engineering/architecture/workflow/influence.png)

For any given proposal, the following people should be involved:

* An Architecture Evolution Coach (a Principal+ Engineer) who will be a coach
  and a mentor guiding the author through the process,
* A Management Engineering Leader, who is a people's leader supposed to support
  the process,
* A Product Manager responsible for finding a way to fund the initiative.

During the process of working on the proposal, the author collaborates with an
Architecture Evolution Coach, managers and domain experts, to create a blueprint.

In order to choose the right stakeholders, the author and their manager will
first need to understand what is the scope of their proposal, what departments
and teams will need to help to get the work done and how important it is for
the organization, then they can involve the Architecture Evolution Coach to
guide them through the workflow.

Once the blueprint has enough content to evaluate the proposal (it can still be
fairly short and simple) new processes and workflows become available for you,
to make the proposal visible to the right people. See the section about
[amplification](#amplification).

### Roles

#### The Author

As the original author of a proposal, you are the primary DRI.

#### The Architecture Evolution Coach

Architecture Evolution Coaching is a Principal+ Engineers, who has been already
involved in work on the complex technical initiatives, who can guide the author
throughout the process as a mentor and a coach.

The purpose of involving a coach in the process of creating a blueprint is to
allow people that know most about GitLab to share their knowledge and
perspective on introducing complex architectural changes, help navigate
organizational, ensure the proposal is aligned with our roadmap, and help
management Engineering Leaders prioritize the work.

#### The Engineering Management Leader

The AEC will help you identify the right management Engineering Leader to
evaluate the proposal. Managers are key decision-makers, and, ultimately, will
help to navigate the organizational complexities to get your proposal approved
and funded.

#### The Product Management Leader

The Engineering Management Leader and AEC will help you to identify the right
Product Manager to collaborate on the proposal. PMs are the decision-makers
that will help to include your proposal in the stream of work that is always
in-flight. PMs can also help with funding your proposal if the believe that we
need to hire new people to get it done or to invoke other processes to find
people who can work on it.

#### Domain Experts

[Domain Experts](https://docs.gitlab.com/ee/development/code_review.html#domain-experts)
are engineers with a deep understanding of one or more particular areas. Domain
Experts:

1. Help to ensure conceptual integrity of the features and changes their groups
   / stages / sections are working on
1. Help to collaborate with EMs and PMs and other Engineers to ensure the
   quality of work done in their area of interest
1. Help to plan and draft necessary architectural and conceptual changes that
   will become a leverage in their area of interest

A Domain Expert is an engineer, usually an individual contributor, who knows
most about specific aspects of the codebase and a domain in the area of
proposed changes, but might still lack the deep understanding of the process
behind introducing complex architectural changes, hence the collaboration
between a Domain Expert and an Architecture Evolution Coach might be very
useful.

Sometimes there is an Architecture Evolution Coach available who is also a
Domain Expert in a particular area. In that case there is no need to involve
another person.

#### Functional Experts

Functional Experts are engineers with deep knowledge across specific functional
areas, which include [Security](/handbook/security/#-contacting-the-team), QA, Database, and Infrastructure. You should
always involve these functional experts during the generation of blueprint so
that we generate awareness early in the cycle and so that they can provide
appropriate input into the blueprint.

It is a responsibility of a proposal DRIs, especially Architecture Evolution
Coach and managers to figure it out which Functional Experts need to get
involved early in the blueprint creation phase, to provide feedback and
guidance.

### Blueprint

The Author, Architecture Evolution Coach, Engineering Management Leader,
Product Management Leader, Domain Experts, Functional Experts collaborate
initially in a [blueprint merge request](https://gitlab.com/gitlab-org/gitlab/-/tree/master/doc/architecture/blueprints)

A blueprint merge request is a description of [Why, How and What](https://en.wikipedia.org/wiki/Start_With_Why)
of the change that has been proposed in the issue. It is also a mind map of
future iterations. It describes challenges, opportunities and a technical
vision that are supposed to guide team members throughout their iterations,
even though it usually does not describe the path to the success in detail. As
we move forward with implementation and iterate on a project, we continuously
incorporate feedback gained after each of the iterations, into the blueprint
itself. The blueprint evolves as we move forward, hence it supports "an
evolutionary architecture" practice.

Blueprints are mostly written by engineers, but their content should not be
deeply technical. The audience are Product Team Members, management Engineering
Leaders and the wider community. A blueprint should describe a clear vision
that is easy to understand: use simple diagrams, and avoid technical jargon
overload. Technical details will be fleshed out in subsequent epics and issues
associated with a blueprint once we enter the execution phase.

Merged blueprints will be published on [GitLab Architecture Docs](https://docs.gitlab.com/ee/architecture/)
public pages.

If you don't know what content you should put into a blueprint, you can use
[this template](https://gitlab.com/gitlab-org/gitlab/-/blob/master/doc/architecture/blueprints/_template.md?plain=1)
as a starting point.

Please be conscious of our [SAFE](/handbook/legal/safe-framework/) framework
guidelines, and start collaborating on a blueprint in a private space (like a
Google Doc) if it should not be made public.

### Getting things done

Once the blueprint is merged and there is a buy in from Engineering Management
and Product Management Leaders, it is important to find DRIs responsible for
the implementation. Those DRIs can be the same as DRIs responsible for the
blueprint creation / proposal, but it is okay to reassign people too.

The blueprint needs three people that will become DRIs:

1. An Engineering Management Leader (for example - Director of Engineering)
1. A Product Management Leader (for example - Senior Product Manager)
1. A Technical Leader (for example - Senior Backend Engineer)

These people will be responsible for the evolution of the blueprint and
figuring it out how to get the blueprint implemented.

DRIs can decide to form a [Working Group](/company/team/structure/working-groups/)
to structure the efforts related to the architecture change. Key considerations
in deciding to form a Working Group are the size, complexity, and
organizational impact of the change.

The concept of a Working Groups can be an extension of the Architecture
Evolution Workflow, but if it is not applicable in a particular case, a
different process can be followed, like the suggested one that is described
below.

### Amplification

We recognize the challenge of implementing complex architectural changes, over
many months or even years. It is difficult to start such a work, fund it in the
long term and avoid disruptive distractions as the implementation moves
forward.

Blueprints are often written by individual engineers, yet these documents
usually describe far-reaching visions. Implementing such a vision takes time
and might require funding. The Architecture Evolution Workflow has been built
to better support teams in getting this kind of work done. There are a few
associated processes, established to increase the likelihood of a success.

One of processes designed to help is a monthly Architecture Evolution Sync
meeting with Engineering Fellows and VP of Development, among others. The
purpose of this meeting is to:

- Increase visibility and awareness of blueprints.
- Coordinate large initiatives across the organization.
- Provide status updates about the most important initiatives.
- Receive guidance regarding staffing and funding.

### Evolution

Once the work starts, it is important to realize that working on complex
technical / architectural initiatives is an evolutionary process. The DRIs will
be responsible for getting back to the content described in the blueprint to
update it with the information from the feedback every iteration gives them.
The blueprint is a document that evolves as the implementation continues.

### Finally

When the work is completed, blueprints no longer represent a forward-looking
architectural vision, instead the content describes the work done. As such,
they should be removed from *docs* and should be move to an
[archive](https://gitlab.com/groups/gitlab-org/architecture/-/archived) or transformed
into blog posts.
