# Encoded PowerShell Investigation

## Scenario

Suspicious PowerShell execution identified through Windows Event ID 4688 logs.

## Detection Logic

Encoded PowerShell commands were identified using process creation logs.

## Objectives

- Identify the payload
- Decode the command
- Extract IOC information
- Map activity to MITRE ATT&CK
- Create detection logic

## Findings

The PowerShell payload contained:

- AMSI bypass functionality
- RC4-style decryption routine
- HTTPS communication
- Remote payload retrieval

## Artifacts

- 📊 [Attack Flow Diagram](Investigations/001-Encoded-PowerShell/attack-flow.png)

- 🚨 [Indicators of Compromise](Investigations/001-Encoded-PowerShell/iocs.md)

- 🎯 [MITRE ATT&CK Mapping](Investigations/001-Encoded-PowerShell/mitre-mapping.md)

- 🔍 [Splunk Searches](Investigations/001-Encoded-PowerShell/splunk_search.md)
