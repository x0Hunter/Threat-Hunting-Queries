## Splunk Search

```spl
index=botsv2 sourcetype="WinEventLog" EventCode=4688
| where like(process_name,"%whoami.exe")
| where like(Process_Command_Line,"%/user%")
| table _time ComputerName process_name Process_Command_Line
```
