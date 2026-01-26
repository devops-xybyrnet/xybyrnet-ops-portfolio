# Audits

## Purpose

The audit system documents the **operational state, changes, and health** of xybyrnet over time.

Audits exist to provide:
- Accountability
- Traceability
- Proof of active system administration

This is a living record of how the system is actually operated.

---

## What Is Audited

Audits may include, but are not limited to:

- System health snapshots (uptime, load, disk, memory)
- Configuration changes
- Security-related events
- Backup verification
- Service state verification
- Access and authentication changes

Audits favor **simple, repeatable commands** over complex tooling.

---

## Audit Philosophy

- Audits are **manual-first**, automation-assisted
- Logs reflect reality, not best-case assumptions
- Failures are documented, not hidden
- Consistency matters more than frequency

An incomplete audit is better than no audit.

---

## Audit Sources

Audit data may be sourced from:

- `journalctl`
- `systemctl`
- `df`
- `uptime`
- Custom logging scripts
- Structured admin logs from jr-admin-ops

---

## Retention and Integrity

Audit records are:
- Version-controlled
- Timestamped
- Immutable once committed

This repository serves as the historical record.

---

## Relationship to Operations

Audits do not replace operations — they **validate** them.

Operational changes should result in audit entries.
