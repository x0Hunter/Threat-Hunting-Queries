index=botsv2 EventCode=4688
| where match(process_name,"(?i)(cmd|powershell).exe$")
| where match(Process_Command_Line,"(?i)(-enc|-nop|hidden|invoke-webrequest|downloadstring|webclient|Iex|whoami|get-aduser)")
| table _time ComputerName process_name Process_Command_Line New_Process_Name
