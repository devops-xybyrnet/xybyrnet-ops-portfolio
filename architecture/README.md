# xybyrnet Architecture

## Purpose

xybyrnet is a **baseline Linux server architecture** designed to prioritize
stability, repeatability, and operational clarity while serving as a
learning platform for foundational system administration skills.

The primary goal is not abstraction or scale, but **mastery of fundamentals**
on a live system that evolves over time.

---

## Core Principles

### 1. Linux-First, Minimal by Design
- Ubuntu LTS as the base operating system
- No GUI on servers
- CLI-driven administration only
- Minimal installed packages

**Why:**  
Understanding the operating system itself is non-negotiable for long-term
operations competence.

---

### 2. Repeatable Architecture
- Identical baseline configuration across systems where possible
- Consistent directory structures
- Standardized user roles and permissions
- Configuration documented before automation

**Why:**  
Repeatability reduces cognitive load, error rates, and recovery time.

---

### 3. Observability Over Abstraction
- Native tools preferred (`journalctl`, `systemctl`, `df`, `uptime`)
- Logs preserved and reviewed
- System state is visible, not hidden behind dashboards

**Why:**  
Operators should understand what the system is doing without relying on
third-party tooling.

---

### 4. Automation Comes After Understanding
- Manual workflows are documented first
- Automation mirrors documented human actions
- Bash and Python favored for transparency

**Why:**  
Automation without understanding creates fragile systems.

---

### 5. Hardware-Agnostic Design
- Designed to run on older, reliable hardware
- No dependency on specialized CPUs or GPUs
- Containers inherit the same baseline assumptions as the core system

**Why:**  
Skills should transfer across environments, not depend on hardware.

---

## xybyrnet Core vs Projects

### xybyrnet Core
- Operating system
- Users and access control
- Networking
- Logging and auditing
- Backup and health checks

This layer changes **slowly**.

### Projects
- Bots
- Services
- Integrations
- Experiments

Projects are **disposable**.  
The core is not.

---

## What xybyrnet Is Not

- Not a cloud platform
- Not a Kubernetes-first system
- Not optimized for scale
- Not a product framework (yet)

xybyrnet exists to build **competence before complexity**.

---

## Evolution

xybyrnet is expected to evolve, but changes are:
- Intentional
- Documented
- Auditable

Learning is the output.  
Stability is the constraint.
