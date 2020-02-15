![](https://github.com/mismailzz/CMAuditd_v2/blob/master/cmauditdv2.png)
# CMAuditd_v2
CMAuditd (version 2) is a free and open-source GUI designed to be used with Auditd, which is the userspace component to the Linux Auditing System. It provides more functionality and a better interface than its previous version.

Requirements
1. Auditd (Linux Utility) must be installed on your Linux (Debian) machine.
2. You have to create an auditd.log file, as it only contain the auditd logs because audit.log contanied the other log records. 

        root@cybermizz:~# nano /var/log/audit/auditd.log

        Also change the log file path from the auditd.conf file

        root@cybermizz:~# nano /etc/audit/auditd.conf

        For Example: change the log_file path to
        log_file = /var/log/audit/auditd.log

3. Run 
        
        root@cybermizz:~# python cmauditd.py
