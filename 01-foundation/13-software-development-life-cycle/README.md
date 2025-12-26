# Software Development Life Cycle (SDLC)

## Purpose

This document explains the **Software Development Life Cycle (SDLC)** from a **DevOps and production operations perspective**.

SDLC is not a theoretical model for exams.

It is the **end-to-end flow of how software is planned, built, delivered, operated, and improved in real organizations**.

DevOps exists to optimize SDLC.

---

## What Is SDLC?

The Software Development Life Cycle is a structured process that defines:

* How software is planned
* How it is developed
* How it is tested
* How it is released
* How it is maintained

From idea to retirement.

---

## Core SDLC Phases (Modern View)

> Plan → Design → Build → Test → Release → Deploy → Operate → Improve

Older models stop at “deploy”.

Real SDLC continues **as long as the application exists**.

---

## 1. Planning

### What happens

* Business requirements are defined
* Scope and priorities are decided
* Risks are identified

### Outputs

* Requirements
* Backlog
* Architecture direction

### DevOps impact

* Feasibility of automation
* Operational cost awareness
* Early reliability considerations

---

## 2. Design

### What happens

* System architecture is designed
* Technology choices are made
* Data flows are defined

### DevOps impact

* Scalability decisions
* HA vs FT tradeoffs
* Stateless vs stateful design

Bad design creates permanent operational pain.

---

## 3. Build (Development)

### What happens

* Code is written
* Dependencies are added
* Artifacts are produced

### DevOps impact

* Reproducible builds
* Version control discipline
* Dependency management

This phase feeds CI pipelines.

---

## 4. Test

### What happens

* Functional tests
* Integration tests
* Security checks

### DevOps impact

* Automated testing
* Shift-left security
* Fast feedback

Untested software becomes operational debt.

---

## 5. Release

### What happens

* A version is approved
* Change is documented
* Release artifacts are tagged

### DevOps impact

* Versioning strategy
* Release traceability
* Rollback readiness

Release ≠ deploy.

---

## 6. Deploy

### What happens

* Software is pushed to environments
* Traffic is shifted

### DevOps impact

* CI/CD pipelines
* Blue-green / rolling deployments
* Zero-downtime strategies

Deployment must be **repeatable and reversible**.

---

## 7. Operate

### What happens

* Application runs in production
* Users generate traffic

### DevOps impact

* Monitoring
* Logging
* Incident response

This phase consumes most engineering time.

---

## 8. Improve

### What happens

* Incidents are reviewed
* Performance is tuned
* Automation is added

### DevOps impact

* Blameless postmortems
* Reliability improvements
* Reduced manual work

This closes the SDLC loop.

---

## SDLC Models (Reality Check)

### Waterfall

* Linear
* Rigid
* Slow feedback

Rare in modern DevOps environments.

### Agile

* Iterative
* Incremental
* Fast feedback

Most common today.

### DevOps Model

* Continuous
* Automated
* Operations-aware

SDLC never truly ends.

---

## How DevOps Maps to SDLC

| SDLC Phase | DevOps Contribution          |
| ---------- | ---------------------------- |
| Plan       | Feasibility & cost awareness |
| Design     | Reliability & scalability    |
| Build      | CI pipelines                 |
| Test       | Automated testing            |
| Release    | Versioning & approvals       |
| Deploy     | CD pipelines                 |
| Operate    | Monitoring & on-call         |
| Improve    | Continuous optimization      |

DevOps is the **execution engine of SDLC**.

---

## Why This Matters for Your Home Lab

Every lab in this repository should map to:

* One or more SDLC phases

Examples:

* Linux labs → Operate
* CI/CD labs → Build/Test/Deploy
* Monitoring labs → Operate/Improve

If a lab does not fit SDLC, it is incomplete.

---

## Key Takeaway

SDLC is not a process document.

It is a **living loop** that defines how software survives in production.

DevOps exists to make this loop:

* Faster
* Safer
* More reliable