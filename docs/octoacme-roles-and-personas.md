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

## Additional Personas and Roles

### Executive Sponsor

#### Role Summary and Primary Goals
Executive Sponsors provide organizational direction, authorize investment, and remove barriers that the delivery team cannot resolve. Their goal is to keep the initiative aligned to business outcomes and make timely go/no-go and major trade-off decisions.

#### Responsibilities, Interactions, and Decision Rights
- Approve the Project One-pager, funding, major scope or priority changes, and planning-to-delivery decision gates.
- Review milestone status, risks, and decisions from Product Managers and Project Managers; represent stakeholder priorities and resolve cross-organization conflicts.
- Receive escalations from the Project Manager through the Team-level -> PM -> Product Lead -> Sponsor path, including business-impacting delivery, security, privacy, or compliance risks.
- Sponsor outcomes with Stakeholders while Developers, QA/Testing, and delivery leads provide the evidence needed for approval.
- Provide decisions and documented direction; hand off approved priorities and constraints to Product Managers and Project Managers.

### Engineering Lead or Technical Lead

#### Role Summary and Primary Goals
Engineering Leads or Technical Leads own technical direction and delivery feasibility. Their goal is to help the team deliver maintainable, reliable software while managing technical risk.

#### Responsibilities, Interactions, and Decision Rights
- Define or approve technical designs, architecture decisions, engineering estimates, and technical standards; record significant decisions in technical design docs or the decision log.
- Partner with Product Managers on feasibility and trade-offs, Project Managers on dependencies and milestones, and Developers on implementation and code review.
- Coordinate with QA/Testing on test strategy, Definition of Done, defect priority, and release readiness; work with Security, Privacy, or Compliance Leads on required controls.
- Escalate material technical risks, blocked dependencies, or changes that threaten the release plan to the Project Manager for the Risk Register and stakeholder communication.
- Hand off implementation-ready designs and estimates to Developers, and release-readiness evidence to the Release or DevOps Engineer.

### UX/UI Designer or User Researcher

#### Role Summary and Primary Goals
UX/UI Designers or User Researchers represent user needs through research, workflows, and interface design. Their goal is to make solutions understandable, usable, and validated against user outcomes.

#### Responsibilities, Interactions, and Decision Rights
- Conduct discovery, document user insights, create workflows or designs, and define usability acceptance criteria.
- Partner with Product Managers on problem statements, success metrics, prioritization, and solution validation; consult Business Analysts or Domain Experts for workflow accuracy.
- Collaborate with Developers on implementation intent and accessibility, and with QA/Testing on usability and acceptance validation.
- Share research findings with Stakeholders and Customer or Support Representatives; flag unmet user needs or usability risks to the Product Manager and Project Manager.
- Deliver approved design artifacts and research findings for backlog refinement; Product Managers make product-priority decisions after considering the evidence.

### Business Analyst or Domain Expert

#### Role Summary and Primary Goals
Business Analysts or Domain Experts translate business processes, policies, and stakeholder needs into clear requirements. Their goal is to reduce ambiguity and ensure the team delivers the intended business outcome.

#### Responsibilities, Interactions, and Decision Rights
- Refine requirements, business rules, process flows, and acceptance criteria with Product Managers and Stakeholders.
- Support Project Managers with dependency identification and Developers and QA/Testing with clarifications needed for implementation and validation.
- Consult with UX/UI Designers or User Researchers on workflows, and Security, Privacy, or Compliance Leads on regulated or policy-driven requirements.
- Escalate unresolved requirements or conflicting stakeholder needs to the Product Manager; document agreed clarifications in backlog items or related specifications.
- Hand off clear, testable requirements to Developers and QA/Testing; Product Managers retain priority and scope decision rights.

### Release or DevOps Engineer

#### Role Summary and Primary Goals
Release or DevOps Engineers enable safe, repeatable delivery through environments, CI/CD, observability, deployment, rollback, and post-deploy verification. Their goal is to make releases reliable and recoverable.

#### Responsibilities, Interactions, and Decision Rights
- Maintain or coordinate deployment pipelines, environment readiness, observability, release checklists, rollback plans, and post-deploy verification.
- Partner with Developers on build and deployment automation, QA/Testing on staging and smoke-test readiness, and Project Managers on release plans and deployment windows.
- Verify that release prerequisites are met, including passing CI and security scans, release notes, smoke tests, and rollback or mitigation plans.
- Coordinate release communications with Product Managers, Customer or Support Representatives, and Stakeholders; escalate failed deployments or operational risks through incident response and the Project Manager.
- Provide release-readiness status and deployment evidence; halt or roll back a release when required safeguards are not met, escalating the decision to the appropriate delivery and business owners.

### Security, Privacy, or Compliance Lead

#### Role Summary and Primary Goals
Security, Privacy, or Compliance Leads identify required safeguards and assess risk before and during delivery. Their goal is to protect customers and the organization while enabling compliant releases.

#### Responsibilities, Interactions, and Decision Rights
- Define applicable security, privacy, regulatory, and compliance requirements; review risks, controls, and evidence for higher-risk work.
- Partner with Engineering Leads or Technical Leads and Developers on threat mitigation, secure implementation, and security scanning; partner with QA/Testing on validation.
- Advise Product Managers and Business Analysts or Domain Experts on policy constraints and acceptance criteria, and notify Project Managers of risks that belong in the Risk Register.
- Escalate security incidents using the security incident runbook and Security on-call process; inform the Executive Sponsor when a business-impacting decision is required.
- Provide control requirements and review findings; approve or require remediation for controls within their authority before release, while the Executive Sponsor owns business-risk acceptance.

### Customer or Support Representative

#### Role Summary and Primary Goals
Customer or Support Representatives bring customer feedback and operational context into delivery. Their goal is to ensure the team prepares customers and support channels for changes and learns from production use.

#### Responsibilities, Interactions, and Decision Rights
- Share customer pain points, common support scenarios, and release-impact information with Product Managers, UX/UI Designers or User Researchers, and Stakeholders.
- Review support readiness, known issues, release notes, and customer communications with the Release or DevOps Engineer and Project Manager.
- Provide QA/Testing with representative customer scenarios and help triage customer-reported issues after release with Developers.
- Escalate significant customer impact through the Project Manager and incident process; contribute customer evidence to prioritization decisions owned by Product Managers.
- Deliver support-readiness input and customer communication needs before release, then hand off production feedback for backlog refinement and retrospectives.

### Data or Analytics Partner

#### Role Summary and Primary Goals
Data or Analytics Partners define how success is measured and help the team learn from delivery outcomes. Their goal is to provide trustworthy evidence for product and project decisions.

#### Responsibilities, Interactions, and Decision Rights
- Define measurement plans, instrumentation requirements, dashboards, and success-metric reporting with Product Managers.
- Partner with Developers on instrumentation implementation, QA/Testing on data validation, and UX/UI Designers or User Researchers on behavioral hypotheses.
- Provide Project Managers and Stakeholders with milestone and outcome reporting; identify data-quality, privacy, or measurement risks for the Risk Register.
- Escalate material metric, data-quality, or privacy concerns to the Product Manager, Project Manager, and Security, Privacy, or Compliance Lead as applicable.
- Deliver validated measurement results for release review and retrospectives; Product Managers use the evidence to make prioritization decisions.

---

## Role Coverage and Combined Responsibilities

### Core and Situational Roles

Every initiative needs accountable coverage for product direction, delivery coordination, implementation, quality validation, and stakeholder sponsorship. Product Managers, Project Managers, Developers, QA/Testing, and Stakeholders provide this core coverage; an Executive Sponsor is required when authorization or business-risk decisions cannot be made by the accountable Stakeholder.

The additional roles above are situational and should be engaged when their expertise is relevant: technical complexity (Engineering Lead or Technical Lead), user discovery (UX/UI Designer or User Researcher), complex business rules (Business Analyst or Domain Expert), operational release work (Release or DevOps Engineer), regulated or sensitive data (Security, Privacy, or Compliance Lead), material customer impact (Customer or Support Representative), or measurable product outcomes (Data or Analytics Partner).

Smaller teams may assign several roles to one person. They must still name a single accountable owner for each decision, deliverable, risk, and handoff in the Project One-pager, backlog, Risk Register, or decision log. When one person holds multiple roles, use an independent reviewer for high-risk approvals where practical, and escalate conflicts of interest or unresolvable trade-offs through the established escalation path.

### Lifecycle Responsibility and Interaction Guide

| Lifecycle activity | Accountable owner | Required collaborators | Key deliverable, handoff, or escalation |
| --- | --- | --- | --- |
| Initiation | Product Manager | Executive Sponsor, Project Manager, Stakeholders, Business Analyst or Domain Expert, Data or Analytics Partner | Project One-pager, success metrics, initial risks, and approval to plan |
| Planning | Project Manager | Product Manager, Developers, Engineering Lead or Technical Lead, QA/Testing, UX/UI Designer or User Researcher, Security, Privacy, or Compliance Lead | Prioritized backlog, estimates, Definition of Done, release plan, and Risk Register |
| Execution | Developers | Engineering Lead or Technical Lead, Product Manager, Project Manager, QA/Testing, Business Analyst or Domain Expert | Implemented increments, reviews, updated project board, and escalation of blockers or technical risks |
| Quality validation | QA/Testing | Developers, Engineering Lead or Technical Lead, Product Manager, UX/UI Designer or User Researcher, Security, Privacy, or Compliance Lead | Test evidence and acceptance results; unresolved defects or control gaps escalate to the Project Manager |
| Release | Release or DevOps Engineer | Developers, QA/Testing, Project Manager, Product Manager, Security, Privacy, or Compliance Lead, Customer or Support Representative | Release checklist, deployment and rollback evidence, release notes, and stakeholder/support announcement |
| Risk escalation | Project Manager | Risk owner, Product Manager, Engineering Lead or Technical Lead, Security, Privacy, or Compliance Lead, Executive Sponsor | Updated Risk Register; escalate Team-level -> PM -> Product Lead -> Sponsor, or use the security incident runbook |
| Stakeholder communication | Project Manager | Product Manager, Executive Sponsor, Customer or Support Representative, Data or Analytics Partner | Weekly or milestone-based status with progress, next steps, risks, blockers, and decisions needed |
| Retrospectives | Project Manager | Product Manager, Developers, QA/Testing, Release or DevOps Engineer, Customer or Support Representative, Data or Analytics Partner, Stakeholders | Blameless retrospective action items with owners, due dates, and success criteria |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
