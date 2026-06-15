T1033 - System Owner/User Discovery
Scenario

During threat hunting activities, process creation logs (Windows Event ID 4688) revealed execution of the whoami.exe utility with discovery-related parameters.

Observed commands:

whoami /user
whoami /groups

These commands are commonly used by attackers after gaining execution on a host to identify the current user context and enumerate security group memberships.

Detection Logic
[Splunk Query](./Investigations/001-System-Owner-User-Discovery/splunk_search.md)


The following commands were identified:

Command	Purpose
whoami /user	Identify current user account
whoami /groups	Enumerate local and domain group memberships

