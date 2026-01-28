# Repository Cloning and Local Setup

## Purpose
Define the standard procedure for cloning and working with the
xybyrnet operations portfolio repository on a local workstation.

This ensures documentation changes are made in a controlled,
traceable environment rather than ad-hoc edits on production hosts.

## Repository
- Name: xybyrnet-ops-portfolio
- Owner: devops-xybyrnet
- Visibility: Public
- Role: Documentation-first operations portfolio

## Standard Local Location
Repositories are cloned under:
~/repos/

This provides a predictable, non-intrusive workspace that keeps
home directories and production systems clean.

## Clone Procedure
From a local workstation:

git clone https://github.com/devops-xybyrnet/xybyrnet-ops-portfolio.git
cd xybyrnet-ops-portfolio

## Verification
A successful clone will contain the following top-level directories:

- architecture/
- operations/
- projects/
- audits/
- evidence/

Presence of these directories confirms the correct repository root.

## Rationale
Separating documentation workflows from live systems:
- reduces operational risk
- prevents accidental modification of production files
- improves auditability
- mirrors professional infrastructure practices

## Status
Standardized and in active use on PC3
