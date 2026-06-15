**##T1033 - System Owner/User Discovery**
Scenario

During threat hunting activities, process creation logs (Windows Event ID 4688) revealed execution of the whoami.exe utility with discovery-related parameters.

**Observed commands**

whoami /user

These commands are commonly used by attackers after gaining execution on a host to identify the current user context and enumerate security group memberships.


**Command	Purpose**
whoami /user	Identify current user account

- 📊 [Attack Flow Diagram](./investigations/002-System-Owner-User-Discovery/attack-flow.png)

- 🔍 [Splunk Searches](./investigations/002-System-Owner-User-Discovery/splunk_search.md)
