# Application Support and Maintenance

## Purpose

This document explains **application support and maintenance as it actually exists in production environments**.

Most DevOps and SRE work is not greenfield development.
It is the continuous responsibility of **keeping systems reliable, secure, and performant after deployment**.

Understanding this topic prevents unrealistic expectations about DevOps roles.

---

## What Is Application Support?

Application support is the discipline of:

* Monitoring running systems
* Responding to incidents
* Troubleshooting failures
* Restoring service quickly

Support work happens **after the application is live** and continues for its entire lifetime.

---

## What Is Application Maintenance?

Maintenance is the ongoing effort to:

* Improve stability
* Reduce operational risk
* Apply updates and fixes
* Adapt to changing requirements

Maintenance is proactive.
Support is reactive.

Both are unavoidable.

---

## Typical Support Responsibilities

### Incident Response

* Alerts fire
* Engineers investigate
* Service is restored

Key goals:

* Minimize downtime
* Reduce blast radius
* Communicate clearly

---

### Troubleshooting

Common activities:

* Log analysis
* Metric inspection
* Network debugging
* Configuration validation

Most incidents are caused by:

* Misconfiguration
* Resource exhaustion
* Dependency failures

---

### On-Call Duties

Production systems require:

* 24/7 availability
* Defined escalation paths
* Clear ownership

On-call is part of operational maturity.

---

## Typical Maintenance Responsibilities

### Patching and Updates

* OS updates
* Library upgrades
* Security patches

Unpatched systems are a security risk.

---

### Performance Optimization

* Resource tuning
* Query optimization
* Capacity planning

Performance issues often appear **after growth**.

---

### Technical Debt Reduction

* Refactoring
* Simplifying architecture
* Improving automation

Ignored debt becomes outages.

---

## DevOps Role in Support and Maintenance

DevOps engineers:

* Automate repetitive fixes
* Improve observability
* Harden deployment pipelines
* Reduce manual intervention

The goal is not to eliminate incidents.

The goal is to **make incidents boring and recoverable**.

---

## Incident Lifecycle (Real World)

1. Detection (monitoring or users)
2. Triage (impact assessment)
3. Mitigation (stop the bleeding)
4. Resolution (fix root cause)
5. Postmortem (learn and improve)

Skipping steps leads to repeated failures.

---

## Blameless Postmortems

Effective teams:

* Focus on systems, not people
* Document what happened
* Track corrective actions

Blame hides problems.

---

## Relationship with the Application Lifecycle

Support and maintenance primarily affect:

* Observe
* Fail
* Recover
* Improve

They close the feedback loop.

---

## Why This Matters for Your Home Lab

Your home lab should:

* Break intentionally
* Produce logs and alerts
* Require recovery

Labs that never fail teach nothing.

---

## Key Takeaway

Running software is harder than writing it.

Application support and maintenance are where:

* Engineering judgment is tested
* Automation proves its value
* DevOps maturity is measured

If you can support a system, you understand it.