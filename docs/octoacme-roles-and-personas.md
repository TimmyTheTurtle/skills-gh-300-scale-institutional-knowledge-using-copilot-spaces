# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Additional Project Roles

These are accountabilities, not mandatory separate positions. Name an owner for each accountability that is needed; one person may cover more than one role on a smaller team if they have the capacity and relevant skills. Keep independent review for high-impact quality, security, privacy, and release decisions even when responsibilities are combined. Bring in a specialist when the work, risk, regulation, or operational impact requires expertise the team does not have.

The Product Manager owns product outcomes, priority, and scope trade-offs; the Project Manager owns delivery coordination, schedule, dependencies, and status. Neither role replaces the accountable technical, design, analysis, quality, operational, or security owner. Stakeholders provide context, feedback, and required approvals; the delivery team records decisions, owners, risks, and handoffs in the project artifacts.

### Engineering / Technical Lead

#### When needed
Name a lead when work spans multiple developers or systems, introduces significant technical choices or dependencies, or carries material technical risk. For a small, low-risk change, a Developer may take this accountability.

#### Role Summary
The Engineering or Technical Lead guides technical direction and coordinates engineering work so the solution is feasible, maintainable, testable, and aligned with product goals.

#### Primary Responsibilities
- Shape architecture and technical approach with the Developers doing the work.
- Coordinate estimates, integration points, engineering dependencies, and technical risk mitigations during planning.
- Ensure implementation plans address reliability, observability, accessibility, and testability as relevant.
- Coordinate technical review and support QA/Testing in resolving defects and assessing technical readiness.

#### Goals
- Deliver a coherent, maintainable solution with understood technical trade-offs.
- Surface technical constraints and risks early enough to inform scope and milestones.

#### Decision and Ownership Boundaries
Owns technical design and engineering recommendations within agreed product scope and standards. Partners with the Product Manager on technical/product trade-offs and with the Project Manager on delivery impact, dependencies, and risks. Does not unilaterally set product priority or waive acceptance, quality, security, or privacy requirements; escalate unresolved trade-offs to the accountable Product Manager or appropriate specialist.

#### Typical Communication, Collaboration, and Handoffs
- With Developers: review designs, divide integration work, and hand off implementation details and technical decisions.
- With the Product Manager: explain feasibility and options so scope and acceptance criteria can be refined.
- With the Project Manager: provide estimates, dependencies, and owned mitigations for the plan and risk register.
- With QA/Testing: agree on testability, environments, and technical evidence; hand over a testable increment and known limitations.
- With Stakeholders: explain technical impacts in accessible terms when a decision or approval is needed; the Project Manager coordinates the update.

### UX/UI Designer or User Researcher

#### When needed
Involve a designer or researcher when success depends on understanding user needs, changing a user journey or interface, or validating usability or accessibility. Developers and the Product Manager can cover lightweight discovery for a simple change, but should seek specialist input when user impact or uncertainty is substantial.

#### Role Summary
This role turns user needs into usable, accessible experiences and evidence that proposed solutions work for intended users.

#### Primary Responsibilities
- Plan and conduct appropriate user research; synthesize findings and share limitations.
- Create interaction flows, prototypes, and interface guidance aligned with product goals and design standards.
- Validate usability and accessibility with users or suitable methods, then communicate findings.
- Partner with Developers and QA/Testing to make designs feasible and define observable acceptance criteria.

#### Goals
- Help users complete their tasks effectively and accessibly.
- Reduce product uncertainty through research and validation before and during delivery.

#### Decision and Ownership Boundaries
Owns research methods, design artifacts, and design recommendations, not product priority or final business scope. The Product Manager decides product trade-offs using research alongside business and stakeholder input. Developers own implementation choices within the agreed design and technical approach; deviations affecting user experience are reviewed with design and product.

#### Typical Communication, Collaboration, and Handoffs
- With the Product Manager and Stakeholders: frame user needs and share research evidence to inform outcomes, scope, and acceptance criteria.
- With Developers: hand over flows, prototypes, interaction states, and accessibility considerations; resolve implementation questions together.
- With QA/Testing: hand over usability and accessibility expectations and collaborate on validation of the delivered experience.
- With the Project Manager: identify research or design dependencies and timing early for the plan and status updates.

### Business Analyst

#### When needed
Use a Business Analyst when workflows, policies, data, integrations, or stakeholder needs are complex, ambiguous, or subject to formal approval. The Product Manager or Project Manager can clarify straightforward requirements on a small team.

#### Role Summary
The Business Analyst makes business needs and processes explicit and traceable so the team can agree on scope and verify that delivery addresses the intended need.

#### Primary Responsibilities
- Elicit and document business needs, user or operational workflows, assumptions, and constraints.
- Map requirements to backlog items, acceptance criteria, decisions, and relevant stakeholders.
- Identify gaps, conflicting needs, dependencies, and impacts of proposed changes.
- Support validation with stakeholders and QA/Testing against agreed requirements.

#### Goals
- Establish a shared, testable understanding of what the project must achieve.
- Reduce rework caused by missing, conflicting, or unverified requirements.

#### Decision and Ownership Boundaries
Owns the quality and traceability of analysis, not product priority, schedule, or approval of business trade-offs. The Product Manager remains accountable for product scope and acceptance criteria, with required stakeholder approvals recorded. The Project Manager tracks decisions and dependencies in project artifacts.

#### Typical Communication, Collaboration, and Handoffs
- With Stakeholders and the Product Manager: elicit needs, resolve ambiguity, and hand over documented workflows and options for prioritization.
- With the Project Manager: record decisions, assumptions, owners, and dependencies for the plan and risk register.
- With Developers and QA/Testing: explain requirement intent and hand over traceable acceptance criteria for implementation and verification.
- Raise changes or unresolved conflicts to the Product Manager for scope decisions and to the Project Manager for delivery-impact coordination.

### Operations / Site Reliability or Release Owner

#### When needed
Assign this accountability when a change affects production services, deployment coordination, reliability, data migration, monitoring, or rollback. For low-impact changes, a Developer may own release tasks with review from the appropriate operational contact.

#### Role Summary
The Operations, Site Reliability, or Release Owner helps ensure a change can be deployed, operated, observed, and recovered safely.

#### Primary Responsibilities
- Advise on operational requirements, service-level expectations, capacity, monitoring, alerting, and support readiness.
- Define or coordinate deployment steps, release windows, runbooks, and rollback or mitigation plans.
- Review release readiness, including staging or smoke-test evidence and post-deployment verification.
- Coordinate operational incident response and capture follow-up actions when a release causes an issue.

#### Goals
- Release changes predictably while protecting service reliability and recoverability.
- Ensure teams can detect, communicate, and respond to production impact.

#### Decision and Ownership Boundaries
Owns operational readiness recommendations and assigned release execution. Can block or escalate a release that misses agreed safety or readiness criteria; the accountable release decision and any accepted risk must be explicit and recorded by the designated authority. Does not own product scope or independently waive acceptance or security requirements.

#### Typical Communication, Collaboration, and Handoffs
- With Developers and QA/Testing: agree on deployment configuration, environments, smoke tests, operational checks, and evidence; hand over release criteria before the release gate.
- With the Project Manager: coordinate release timing, dependencies, readiness status, and risks.
- With the Product Manager and Stakeholders: communicate release impact, known issues, and verification outcomes; the Project Manager coordinates announcements.
- Hand over deployment and rollback instructions to the on-call or support team, and share incidents through the agreed incident communication path.

### Security / Privacy Specialist

#### When needed
Engage a specialist when work handles sensitive data, changes identity or access, exposes a service or integration, has regulatory obligations, or introduces meaningful security or privacy risk. Teams may apply established low-risk controls without dedicated specialist involvement, but must escalate uncertainty or material risk.

#### Role Summary
The Security or Privacy Specialist identifies security, privacy, and compliance requirements and advises the team on controls, risk treatment, and verification.

#### Primary Responsibilities
- Identify applicable data, threat, privacy, and compliance considerations during initiation and design.
- Recommend proportionate controls, data minimization, access protections, and risk mitigations.
- Review designs or changes when risk warrants specialist review and define evidence needed to verify controls.
- Advise on security/privacy findings, incident escalation, and required remediation.

#### Goals
- Protect users, data, and services while enabling informed delivery decisions.
- Find and address material risks before release rather than relying on late-stage fixes.

#### Decision and Ownership Boundaries
Owns specialist assessments and recommendations; the accountable business or technical owner remains responsible for implementing mitigations and recording accepted residual risk. Required legal, regulatory, or organizational approvals cannot be replaced by team consensus. Security/privacy concerns that could affect release are escalated through the risk and incident paths and resolved before proceeding under applicable policy.

#### Typical Communication, Collaboration, and Handoffs
- With the Product Manager and Technical Lead: translate requirements and risks into design constraints, backlog work, and planning decisions.
- With Developers: advise on controls and remediation; hand over actionable findings with verification expectations.
- With QA/Testing: coordinate security/privacy verification and review relevant scan or test results.
- With the Project Manager: ensure risks have named owners, mitigations, due dates, and visible status in the risk register.
- With Stakeholders: explain material impacts and required decisions through the agreed communication and escalation channels.

### Combining Roles on Small Teams

Combine roles when scope and risk are modest and the person has the necessary skills; record who owns each accountability in the project plan. A person may contribute in multiple roles, but must distinguish recommendations from approval authority and make conflicts visible. Use independent review or escalate to a qualified specialist for high-impact technical, usability, quality, operational, security, privacy, or compliance decisions. Revisit role coverage when scope, risk, or release impact changes.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
