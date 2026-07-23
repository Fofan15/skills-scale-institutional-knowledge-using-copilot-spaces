# OctoAcme Project Management Processes

## Overview

This directory contains the definitive guides for how OctoAcme manages projects from initiation through completion. Our approach emphasizes **customer value**, **iterative delivery**, **clear ownership**, **data-informed decisions**, and **psychological safety**.

OctoAcme operates on a structured, lifecycle-based project management approach with well-defined roles and lightweight but deliberate artifacts at each stage. We believe in delivering features incrementally while maintaining alignment across stakeholders, and we embed continuous improvement into our culture through structured retrospectives and action item tracking.

### Key Characteristics
- **Execution and quality are tightly integrated** — Teams use GitHub Projects with standardized workflows, small pull requests (≤400 lines), automated testing, and manual QA to ensure reliability
- **Communication cadence is designed for transparency** — Daily standups, weekly delivery syncs, regular demos, and structured risk registers ensure early escalation of business-impacting issues
- **Continuous improvement is embedded** — Retrospectives after each sprint or milestone capture learnings and drive 2–3 prioritized action items that feed back into the backlog

## Quick Navigation

### Core Guides

| Guide | Purpose |
|-------|---------|
| [Project Management Overview](./octoacme-project-management-overview.md) | High-level introduction to roles, principles, and key artifacts |
| [Project Initiation](./octoacme-project-initiation.md) | Steps to validate and authorize new work |
| [Project Planning](./octoacme-project-planning.md) | Breaking work into actionable increments and creating backlogs |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Day-to-day delivery management and progress tracking |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Risk registers, stakeholder communication, and escalation |
| [Release & Deployment](./octoacme-release-and-deployment.md) | Standardized release processes and deployment checklists |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Capturing learnings and driving improvements |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Detailed descriptions of key project roles |

## Key Principles

- **Customer-first** — Prioritize customer value and usability
- **Iterative delivery** — Deliver small, testable increments
- **Clear ownership** — Each project has a named Project Manager (PM) and Product Lead
- **Data-informed** — Measure impact and iterate based on evidence
- **Psychological safety** — Encourage feedback and learning

## Project Lifecycle at a Glance

```
1. INITIATION          2. PLANNING           3. EXECUTION         4. RELEASE            5. CLOSE & RETRO
↓                      ↓                     ↓                    ↓                     ↓
Problem statement      Scope, resources,     Build, test,         Deploy, verify,       Capture learnings,
Stakeholders           milestones,           review, iterate      announce              next steps
High-level timeline    dependencies
```

### Phase Descriptions

1. **Initiation** — Confirm business need, identify stakeholders, define success criteria, decide go/no-go for planning
2. **Planning** — Break work into shippable increments, estimate scope, identify dependencies, create release plan
3. **Execution** — Build and test features, manage daily standups, track progress, escalate blockers
4. **Release** — Deploy to production, run post-deploy verifications, announce to stakeholders
5. **Close & Retrospective** — Capture learnings, generate action items, measure improvements

## Core Roles

| Role | Responsibilities |
|------|------------------|
| **Project Manager (PM)** | Coordinates delivery, manages schedules, owns risk communication, facilitates meetings |
| **Product Manager (PdM)** | Defines outcomes, prioritizes backlog, measures success, validates solutions |
| **Developers** | Implement features, write tests, collaborate on design, estimate work |
| **QA/Testing** | Validate quality, verify acceptance criteria, run smoke tests |
| **Stakeholders** | Provide inputs, approvals, and business context |

## Key Artifacts

- **Project Charter / One-pager** — Problem, goal, success metrics, stakeholders, timeline, risks
- **Roadmap and Release Plan** — High-level features, milestones, dependencies
- **Sprint/Iteration Backlog** — Prioritized work with acceptance criteria and estimates
- **Risk Register** — ID, description, impact, likelihood, owner, mitigation, status
- **GitHub Project Board** — Columns: Backlog, Ready, In Progress, In Review, QA, Done
- **Definition of Done** — Acceptance criteria: tests, linting, documentation, security scans
- **Retrospective Notes** — Learnings and action items with owners and due dates

## Communication Cadence

- **Daily standups** (15 min) — Focus on progress, blockers, dependencies
- **Weekly PM sync** — Alignment between Project Manager and Product Manager
- **Twice-weekly delivery standups** — Team coordination and risk review (or as agreed)
- **Weekly stakeholder updates** — Status, risks, decisions needed
- **End-of-sprint demos** — Show progress and validate solutions
- **Monthly stakeholder briefings** — High-level updates and roadmap reviews
- **Ad-hoc escalations** — For critical blockers and security incidents

## How to Use These Docs

### For New Team Members
1. Start with the [Project Management Overview](./octoacme-project-management-overview.md) for a high-level introduction
2. Review [Roles & Personas](./octoacme-roles-and-personas.md) to understand your role and responsibilities
3. Choose the guide that matches your current project phase

### For Project Managers
- Use [Project Initiation](./octoacme-project-initiation.md) to kick off new work
- Reference [Project Planning](./octoacme-project-planning.md) for sprint planning
- Maintain the Risk Register from [Risk Management & Communication](./octoacme-risks-and-communication.md)
- Use [Execution & Tracking](./octoacme-execution-and-tracking.md) for daily cadence
- Follow [Release & Deployment](./octoacme-release-and-deployment.md) for go-to-market activities
- Facilitate [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) sessions

### For Product Managers
- Define success metrics and acceptance criteria using [Project Initiation](./octoacme-project-initiation.md)
- Prioritize the backlog using [Project Planning](./octoacme-project-planning.md)
- Measure impact and iterate based on [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) learnings
- Communicate with stakeholders using templates from [Risk Management & Communication](./octoacme-risks-and-communication.md)

### For Developers
- Understand acceptance criteria and Definition of Done from [Project Planning](./octoacme-project-planning.md)
- Follow PR and testing guidance in [Execution & Tracking](./octoacme-execution-and-tracking.md)
- Participate in daily standups and retrospectives
- Reference [Roles & Personas](./octoacme-roles-and-personas.md) for developer responsibilities

### For the Entire Organization
- Keep the Project Charter updated in your project repository
- Add process-specific docs to `.copilot/` if using Copilot Spaces for context
- Review and update this README when adding new process guides
- Use issue template [Add Content to Process Docs](./.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) for proposing improvements

## Quick Reference: Risk Escalation

| Level | Owner | Action |
|-------|-------|--------|
| **Level 1: Team** | Delivery team | Triage in daily standup |
| **Level 2: PM** | Project Manager | Escalate to Product Lead and dependent teams |
| **Level 3: Executive** | Sponsor | Escalation for business-impacting issues |

## Quick Reference: Deployment Checklist

Before releasing to production:
- ✅ All acceptance criteria met and PRs merged
- ✅ Passing CI and security scans
- ✅ Release notes drafted
- ✅ Rollback plan documented
- ✅ Smoke tests prepared and passing on staging
- ✅ Post-deploy verification plan ready

## Contributing to These Docs

To propose updates or new process documents:
1. Create an issue using the [Add Content to Process Docs](./.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template
2. Describe the change and rationale
3. Get stakeholder feedback
4. Submit a PR with your proposed changes
5. Ensure alignment with existing process docs

---

**Last Updated:** 2026-07-23  
**Maintained By:** OctoAcme Project Management Team
