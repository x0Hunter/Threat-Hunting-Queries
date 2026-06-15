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

- [Attack-Flow](Investigations/001-Encoded-PowerShell/attack-flow.png)

- [IOCs](Investigations/001-Encoded-PowerShell/iocs.md)

- [MITRE Mapping](Investigations/001-Encoded-PowerShell/mitre-mapping.md)

- [Splunk Search](Investigations/001-Encoded-PowerShell/splunk_search.md)
