# Sensors Login Audit Logging

## Purpose
Capture hardware sensor state at each administrator login to support:
- thermal forensics
- incident review
- operational audits

## Design
- Implemented as a systemd **user** service
- Runs once per login (Type=oneshot)
- Produces no terminal output
- Appends timestamped sensor data to an XDG-compliant state directory

## Implementation Summary
- Service: sensors-login.service
- Command: sensors
- Timestamp format: ISO-8601
- Storage location:
  ~/.local/state/sensors/login.log

## Rationale
Thermal conditions are a common contributing factor to:
- unexpected system instability
- performance degradation
- container host anomalies

Capturing this data at login provides lightweight, repeatable evidence
without introducing runtime overhead or workspace noise.

## Status
Active on srv-base-xybyrnet
