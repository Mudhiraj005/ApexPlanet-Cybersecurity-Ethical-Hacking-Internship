# Log Analysis

## Objective

Analyze the target system logs after the controlled exploitation phase to identify evidence of the simulated attack.

## Log Files Reviewed

The following log files on the Metasploitable 2 target machine were examined as part of the incident response investigation:

- /var/log/auth.log
- /var/log/messages
- /var/log/syslog
- /var/log/apache2/error.log

## Findings

### Authentication Log

The authentication log contained scheduled CRON session activity for the root user. No authentication events related to the UnrealIRCd exploitation were observed.

### System Log

The system log primarily contained normal system messages and periodic syslog "MARK" entries. No exploit-specific events were identified.

### Apache Log

The Apache error log contained only normal web server startup messages. No attack-related entries were recorded.

## Analysis

The UnrealIRCd 3.2.8.1 backdoor exploit bypasses normal authentication mechanisms. As a result, no direct evidence of the attack was present in the reviewed authentication or system logs.

The reviewed system logs did not contain direct evidence of the UnrealIRCd backdoor exploitation because the exploit bypasses the normal authentication process. The compromise was therefore detected by identifying the active Meterpreter session established during the controlled exploitation phase. The session was subsequently terminated and verification confirmed that no active sessions remained.

## Conclusion

Although no direct exploit entries were identified in the reviewed logs, the log analysis confirmed normal system operation and demonstrated the process of examining security-relevant log files during an incident response investigation. The Meterpreter session served as the primary indicator of compromise for this simulated attack.