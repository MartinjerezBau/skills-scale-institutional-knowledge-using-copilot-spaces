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

## Delivery Manager

### Role Summary
Delivery Managers own the end-to-end coordination of cross-team delivery. They maintain the delivery roadmap, remove impediments, and track milestones and dependencies to ensure work flows smoothly from planning to release.

### Responsibilities
- Maintain and communicate the delivery roadmap across teams
- Identify and remove blockers and dependencies that impede progress
- Track milestones, commitments, and delivery health metrics
- Facilitate cross-team ceremonies and alignment checkpoints
- Escalate risks or delays to senior stakeholders as needed

### Goals
- Ensure predictable, on-time delivery across all workstreams
- Reduce dependency friction and unplanned interruptions
- Maintain a clear, shared view of delivery status for all stakeholders

### Typical Communication
- Cross-team delivery syncs and dependency reviews
- Weekly delivery health reports and milestone updates
- Go/no-go coordination with Release Coordinator and Engineering Lead

### Interactions
- Works with **Product Manager** to align roadmap priorities
- Coordinates with **Engineering Lead** on team capacity and velocity
- Partners with **Release Coordinator** on go/no-go decisions
- Escalates blockers to **Project Manager** and senior leadership

---

## QA Lead (Quality Assurance)

### Role Summary
QA Leads define and enforce quality standards across the project lifecycle. They own test planning, coordinate regression and integration testing, and gate releases on agreed quality metrics to ensure software meets acceptance criteria before deployment.

### Responsibilities
- Define and maintain release acceptance criteria and quality gates
- Create, manage, and execute test plans (unit, integration, regression, UAT)
- Coordinate testing windows with engineering and delivery teams
- Track, triage, and report defects against quality thresholds
- Champion quality practices (e.g., shift-left testing, test automation standards)

### Goals
- Prevent defects from reaching production
- Establish measurable, repeatable quality benchmarks
- Enable faster releases by reducing manual testing overhead through automation

### Typical Communication
- Test status reports and defect dashboards
- Coordination with developers during sprint reviews
- Release readiness sign-off communications

### Interactions
- Collaborates with **Engineering Lead** and **Delivery Manager** to schedule testing windows
- Reports defect trends and release readiness to **Product Manager**
- Partners with **Release Coordinator** to gate releases on quality metrics
- Works with **Observability Owner** to align test coverage with monitoring signals

---

## Release Coordinator

### Role Summary
Release Coordinators own the release process end-to-end. They manage the release calendar, runbooks, cutover plans, and deployment communications, ensuring all stakeholders are aligned and rollback plans are in place before any release proceeds.

### Responsibilities
- Maintain the release calendar and communicate upcoming release windows
- Author and maintain release runbooks, cutover checklists, and rollback plans
- Coordinate deployment approvals across engineering, operations, and security
- Communicate release status and outcomes to stakeholders
- Facilitate post-release reviews and capture lessons learned

### Goals
- Execute releases with zero surprises through thorough planning and communication
- Minimize release risk through documented runbooks and tested rollback procedures
- Establish a repeatable, auditable release process

### Typical Communication
- Release readiness briefings and go/no-go meetings
- Deployment notifications and status updates
- Post-release summaries and incident reports

### Interactions
- Coordinates with **Delivery Manager** for milestone and timeline alignment
- Works with **Security Liaison** to ensure security gates are cleared before release
- Partners with **QA Lead** to confirm quality acceptance criteria are met
- Engages **Documentation Steward** to ensure release notes and runbooks are current

---

## Documentation Steward

### Role Summary
Documentation Stewards ensure that process documents, runbooks, and institutional knowledge artifacts are accurate, current, and discoverable. They own the doc lifecycle from creation through review, publishing, and archival.

### Responsibilities
- Maintain and update process docs, runbooks, and knowledge base articles
- Facilitate regular doc reviews with role owners and subject matter experts
- Own doc publishing standards, templates, and discoverability (e.g., search, tagging)
- Track documentation gaps and create issues for missing or outdated content
- Onboard new contributors to documentation standards and tooling

### Goals
- Ensure all team members have access to accurate, up-to-date process information
- Reduce onboarding time by maintaining comprehensive, searchable documentation
- Prevent knowledge loss when team members transition

### Typical Communication
- Doc review requests and feedback cycles
- Documentation health reports (coverage, staleness)
- Onboarding guides and doc contribution guidelines

### Interactions
- Works with **all role owners** to capture decisions, updates, and new processes
- Partners with **Release Coordinator** to publish release notes and runbooks
- Coordinates with **Project Manager** to ensure project artifacts are documented
- Supports onboarding efforts in collaboration with **Engineering Lead**

---

## Security Liaison

### Role Summary
Security Liaisons are the point of contact for all security-related activities in the project lifecycle. They coordinate security reviews, facilitate threat modeling, manage vulnerability triage, and ensure compliance requirements are met before releases proceed.

### Responsibilities
- Conduct or coordinate security reviews and threat modeling sessions
- Triage and track vulnerabilities from discovery through remediation
- Ensure security acceptance criteria are defined and met for each release
- Maintain awareness of compliance requirements (e.g., SOC 2, GDPR, HIPAA) affecting the project
- Champion security best practices (e.g., dependency scanning, secret management, SAST/DAST)

### Goals
- Prevent security defects from reaching production
- Embed security early in the development lifecycle (shift-left security)
- Maintain a clear, auditable record of security decisions and sign-offs

### Typical Communication
- Security review findings and remediation tracking
- Pre-release security sign-off communications
- Compliance status updates to project leadership

### Interactions
- Works with **Engineering Lead** to integrate security practices into development workflows
- Coordinates with **Release Coordinator** to gate releases on security sign-off
- Escalates unresolved vulnerabilities or compliance risks to **Project Manager**
- Engages **Procurement/Legal Liaison** on vendor security assessments and contract terms

---

## Observability Owner

### Role Summary
Observability Owners define and maintain the standards for monitoring, alerting, and telemetry across the project. They own SLO/SLI definitions, coordinate incident post-mortems, and ensure the team has the visibility needed to detect and respond to production issues quickly.

### Responsibilities
- Define and maintain SLOs (Service Level Objectives) and SLIs (Service Level Indicators)
- Own monitoring and alerting standards, tooling, and dashboards
- Coordinate incident response processes and facilitate post-mortem reviews
- Work with engineering to instrument new features with appropriate telemetry
- Track and report on system reliability and performance trends

### Goals
- Achieve agreed reliability targets through proactive monitoring and alerting
- Reduce mean time to detect (MTTD) and mean time to resolve (MTTR) for incidents
- Foster a blameless post-mortem culture that drives continuous improvement

### Typical Communication
- Reliability dashboards and SLO burn-rate reports
- Incident post-mortem documents and action item tracking
- Monitoring standards and runbook documentation

### Interactions
- Collaborates with **Engineering Lead** on instrumentation and telemetry requirements
- Works with **QA Lead** to align observability signals with test coverage
- Partners with **Release Coordinator** to validate monitoring is in place before releases
- Coordinates with **Security Liaison** on security monitoring and anomaly detection

---

## Procurement / Legal Liaison

### Role Summary
Procurement/Legal Liaisons manage the intersection of project delivery with vendor relationships, contracts, and legal obligations. They ensure that third-party dependencies, licensing requirements, and contractual milestones do not become blockers to project timelines.

### Responsibilities
- Manage third-party vendor evaluation, selection, and approval processes
- Review and track contracts, SOWs, and licensing agreements relevant to the project
- Flag legal or compliance risks (e.g., open-source license conflicts, data processing agreements)
- Coordinate vendor onboarding and off-boarding in alignment with project timelines
- Track contract milestones and renewal dates that affect delivery

### Goals
- Prevent legal or procurement issues from blocking project delivery
- Ensure all third-party tools, services, and code comply with organizational policies
- Maintain clear documentation of vendor relationships and contractual obligations

### Typical Communication
- Vendor evaluation summaries and recommendations
- Contract status updates and milestone tracking
- Legal risk advisories for project leadership

### Interactions
- Engages with **Product Manager** and **Delivery Manager** when vendor selection or contract milestones affect delivery timelines
- Coordinates with **Security Liaison** on vendor security assessments
- Works with **Project Manager** to surface procurement risks in the project risk register

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When modeling a process or workflow, identify which personas are involved at each stage and what decisions or artifacts they own.
