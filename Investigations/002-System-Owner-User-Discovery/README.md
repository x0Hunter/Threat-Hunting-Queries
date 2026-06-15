**T1033 - System Owner/User Discovery** 

Scenario

During the investigation, Windows Event ID 4688 process creation logs revealed the execution of `whoami.exe`.

This command was used to gather information about the current user and security groups on the affected systems.

**Observed commands**

whoami /user

These commands are commonly used by attackers after gaining execution on a host to identify the current user context and enumerate security group memberships.
**Command	Purpose**
whoami /user	Identify current user account

- 📊 [Attack Flow Diagram](./user-discovery.png)

- 🔍 [Splunk Searches](./splunk-search.md)

- 🔍 [Result Of Splunk Searches](./splunk-user-discovery.png)


**Affected Systems**
| Date | Time | Host |
|------|------|------|
| 2017-08-24 | 06:17:17 | mercury.frothly.local |
| 2017-08-24 | 06:08:41 | venus.frothly.local |
| 2017-08-24 | 06:01:33 | wrk-klagerf.frothly.local |
| 2017-08-24 | 05:39:09 | wrk-btun.frothly.local |

