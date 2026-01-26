# Audits

## Purpose

Audits in xybyrnet exist to create **accountability, visibility, and trust**
in a live operating system.

This directory documents **what is checked, when it is checked, and why**.
The actual logs may live elsewhere, but the audit standard lives here.

---

## What an Audit Means in xybyrnet

An audit is a **repeatable review of system state** to verify that:

- The system is healthy
- Security controls are intact
- Backups are occurring
- No unexpected changes have occurred

Audits are not reactive.
They are **routine and expected**.

---

## Audit Categories

### 1. System Health Audits
Focus: Availability and resource usage.

Typical checks:
- `uptime`
- Load averages
- Disk usage (`df -h`)
- Memory pressure
- Thermal status (where available)

Frequency:
- Daily (light)
- Weekly (review)

---

### 2. Security & Access Audits
Focus: Unauthorized access and configuration drift.

Typical checks:
- SSH access and authentication logs
- User accounts and permissions
- Firewall status
- Failed login attempts

Frequency:
- Daily review
- Immediate review on anomaly

---

### 3. Backup Verification Audits
Focus: Data survivability.

Typical checks:
- Backup job completion
- Timestamp verification
- Restore feasibility (spot checks)

Frequency:
- Daily verification
- Periodic restore testing

---

### 4. Change Audits
Focus: Intentional vs unintentional changes.

Typical checks:
- Configuration file changes
- Service restarts
- Package updates
- Manual interventions

Frequency:
- Logged at time of change
- Reviewed weekly

---

## Logging Standard

- All audits are timestamped
- Actions are logged with intent
- Logs favor clarity over verbosity
- Logs are version-controlled where appropriate

---

## Why Audits Matter

Audits demonstrate:
- Operational discipline
- Security awareness
- Professional habits
- Readiness for production environments

This audit framework mirrors real-world expectations
for junior system administrators and operations engineers.

---

## Evolution

Audit scope will expand as the system grows.

New audit categories are added only when:
- The system justifies them
- They can be performed consistently
