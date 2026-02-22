# Flipper Zero BadUSB HID Demo

> Defensive research and awareness only. Use responsibly and with authorization.

## Overview
This repository demonstrates how USB HID emulation can be abused to inject keystrokes on an **unlocked** workstation. The goal is to help defenders validate controls, improve user awareness, and test monitoring in a safe lab setting.

## Authorized use only
You may use this project **only** when all of the following are true:
- You own the system, or you have **explicit written authorization** from the system owner.
- You are operating within an agreed scope and timeframe.
- You are not collecting, transmitting, or storing credentials or personal data.

Do not use this on public devices, third party systems, or networks you do not control.

## What this demo does
- Demonstrates HID keystroke injection that launches a **local** process in a controlled environment.

## What this demo does not do
- No extraction of saved WiFi keys or passwords
- No data exfiltration or email sending
- No persistence
- No log tampering or trace deletion

## Safe lab setup
Recommended minimum setup:
- A dedicated VM or test PC
- A non production user account with no stored credentials
- Offline operation, or an isolated test network

## Mitigations and detection ideas
Defensive controls to consider:
- Restrict new USB devices where feasible
- Use endpoint protections that block untrusted HID devices
- Enforce short idle timeouts and screen lock policies
- Monitor for unusual command execution patterns, including suspicious PowerShell usage
- Train users to never leave workstations unlocked

## Disclaimer
This repository is provided for educational and defensive purposes. You are responsible for complying with applicable laws, policies, and authorizations.
