# windows_log_gaps
Identify log gaps in Windows Logs

This script will parse a Windows Event Log and search it for "gaps" in the Record ID sequence that might indicate an attacker or malware has tampered with your log.
This script runs locally, because of the time required for larger logs, it's recommended that for a "blue team" deploy that might be domain-wide, this is run in parallel, locally on all hosts in a domain.
Full write-up of the tool can be found here:
https://isc.sans.edu/forums/diary/25328/

By default, this script assesses the Security Event Log, which is most commonly tampered with.
