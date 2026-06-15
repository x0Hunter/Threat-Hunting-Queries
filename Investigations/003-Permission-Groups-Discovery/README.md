**T1069.001 - Permission Groups Discovery**

Scenario

During the investigation, Windows Event ID 4688 process creation logs revealed the execution of whoami.exe with the /groups parameter.

**Observed command**

whoami /groups

This command is used to display the security groups associated with the current user account.


**Affected Systems**
| Date | Time | Host |
|------|------|------|
| 2017-08-24 | 05:32:00 | wrk-btun.frothly.local |
| 2017-08-24 | 05:31:59 | wrk-btun.frothly.local |

## Investigation Artifacts

* 📊 [Attack Flow Diagram](./permission-groups-discovery.png)
* 🔍 [Splunk Searches](./splunk-search-permission.md)
* 📊 [Resault of Splunk Searches](./splunk.png)


MITRE ATT&CK Mapping
Command	Technique	Description
whoami /groups	T1069.001	Permission Groups Discovery: Local Groups
Description

The whoami /groups command displays the group memberships of the current user account.

Attackers may use this information to identify administrative privileges and determine potential privilege escalation opportunities.



References
MITRE ATT&CK T1069.001
Windows Event ID 4688
