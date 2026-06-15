**T1033 - System Owner/User Discovery**

Scenario

During threat hunting activities, process creation logs (Windows Event ID 4688) revealed execution of the whoami.exe utility with discovery-related parameters.

**Observed commands**

whoami /user

These commands are commonly used by attackers after gaining execution on a host to identify the current user context and enumerate security group memberships.

**Affected Systems**
| Date | Time | Host |
|------|------|------|
| 2017-08-24 | 06:17:17 | mercury.frothly.local |
| 2017-08-24 | 06:08:41 | venus.frothly.local |
| 2017-08-24 | 06:01:33 | wrk-klagerf.frothly.local |
| 2017-08-24 | 05:39:09 | wrk-btun.frothly.local |


**Command	Purpose**
whoami /user	Identify current user account

- 📊 [Attack Flow Diagram](./investigations/002-System-Owner-User-Discovery/attack-flow.png)

- 🔍 [Splunk Searches](./investigations/002-System-Owner-User-Discovery/splunk_search.md)
