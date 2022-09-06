# Software tools

## Information gathering

* [Censys](https://censys.io/) ([search censys](https://search.censys.io/)) scans publicly exposed certificate assets 
on the Internet and stores the details in a searchable database. Useful during passive reconnaissance for gathering 
ports and services listening on hosts and other data about a target.
* [Custom Word List Generator (CeWL)](https://github.com/digininja/CeWL) will crawl target websites and assemble a 
wordlist using interesting terms identified during the crawl, including e-mail addresses. These wordlists can then 
be used for further targeting, brute-forcing possible URLs, hostnames, or even as password cracking dictionaries.
CeWL is a command line tool with options for controlling the depth of the crawl, output file, user agent to send, 
length of words that it collects, and including e-mail addresses.
* [DirBuster](https://wiki.owasp.org/index.php/Category:OWASP_DirBuster_Project) is a Java application using 
dictionaries and wordlists to attempt to guess directories and filenames on websites. DirBuster is an inactive project 
that has been integrated into OWASP ZAP.
* [Fingerprinting Organizations with Collected Archives (FOCA)](https://github.com/ElevenPaths/FOCA) is a tool to 
mine documents for metadata and other hidden information.
* [Maltego](https://www.maltego.com/) uses transforms to automatically retrieve reconnaissance data from open-source 
and paid data sources based on search seeds, such as an e-mail address or domain name.
* [nslookup](https://linux.die.net/man/1/nslookup) makes DNS queries to find
hostnames from IP addresses and IP addresses from hostnames on a network.
* [Recon-ng](https://github.com/lanmaster53/recon-ng) is a framework for conducting reconnaissance. See 
[wiki](https://github.com/lanmaster53/recon-ng/wiki).
* [Shodan](https://www.shodan.io/) aids in gathering information about a target using passive techniques. 
Shodan scans Internet-facing assets and gathers information about open ports and identifiable services and 
allows for search of the results of those scans. Results without touching the targets.
* [theHarvester](https://github.com/laramies/theHarvester) is a command-line tool for OSINT.
* [Whois](https://linux.die.net/man/1/whois) is a service for looking up domain registration information and is 
not only a tool included with Linux, as referenced here. The tool is the client for the service.
* [WiGLE](https://wigle.net/) is a collection of public wardriving data that you can use to
look up SSIDs and BSSIDs to find out where they are according to GPS information in
the search database. This is good for passive information gathering in preparation for a wireless or physical 
pentest assessment.

## Vulnerability identification

* [Nessus](https://www.tenable.com/products/nessus) is a vulnerability scanner. Useful for network discovery 
using port scans and enumerate services from either an authenticated or nonauthenticated context. It then
compares that information to an extensive internal database of known vulnerabilities to
highlight potential or confirmed vulnerabilities on the identified services.
* [Nikto](https://cirt.net/Nikto2) is a web server vulnerability scanner. 
See [wiki](https://github.com/sullo/nikto/wiki)
* [Open Vulnerability Assessment Scanner (OpenVAS)](https://www.openvas.org/) is a free
vulnerability scanner and an open-source alternative to Nessus.
* [Security Content Automation Protocol (SCAP)](https://csrc.nist.gov/projects/security-content-automation-protocol) 
is a collection of specifications for exchanging content from security automation. This is
used in environments requiring compliance according to U.S. government specifications.
* [SearchSploit](https://www.exploit-db.com/searchsploit) is a tool that is included with
Kali Linux that can be used for searching exploit-db.

## Cloud

* [BloodHound](https://bloodhound.readthedocs.io/en/latest/) explores relationships between objects in Active Directory 
or Azure, and displays them graphically. Useful for identifying privilege escalation opportunities along an attack
path, but running the tool against an environment is noisy and potentially disruptive.
* [Cloud Custodian](https://cloudcustodian.io/docs/index.html) runs a series of scripts designed to audit the security 
of cloud environments. It uses YAML files with policies to define what it looks for and produces reports of likely 
issues found with permissions and other cloud configurations based on the policy used to run it. 
* [CloudBrute](https://github.com/0xsha/CloudBrute) is an enumeration tool for cloud environments. It supports 
multiple cloud providers and can identify buckets, applications, and storage based on domain information or other 
target keys supplied at runtime from an unauthenticated perspective. It can also help enumerate exposed ports
and HTTP/S services based on what it finds.
* [Gobuster](https://github.com/OJ/gobuster) can be used to enumerate Amazon S3 buckets; virtual hostnames for web 
servers; and DNS entries using fuzzing, filters, and different protocols and HTTP methods.
* [Pacu](https://rhinosecuritylabs.com/aws/pacu-open-source-aws-exploitation-framework/)
is an AWS security testing toolkit created by Rhino Security Labs. 
* [ScoutSuite](https://github.com/nccgroup/ScoutSuite) is a multiplatform cloud security auditing tool.
* [truffleHog](https://github.com/trufflesecurity/truffleHog) searches GitHub repositories for secrets (such as SSH 
or API keys), examining commit history and branches for accidental leaks of important information.

## Applications

* [Brakeman](https://brakemanscanner.org/) will take Rails source code, scan it, and produce a report of potential 
security issues.
* [Burp Suite](https://portswigger.net/burp) is a web security testing toolkit offered as a graphical application. 
Burp Suite allows you to proxy and intercept, tamper with, replay, and inject web traffic. It
offers plugins that automate attacks such as brute force, SQL injection, and attacks against session management. 
It can passively or actively crawl sites and highlight potential security issues as it goes, using a built-in 
vulnerability scanner.
* [The GNU Debugger](https://www.gnu.org/software/gdb/) is a free debugger. Useful for vulnerability research, 
reverse engineering, and exploit development. For example, it can be used to change a value sent from
an authentication function to the rest of the application, which could bypass authentication.
* [IDA](https://hex-rays.com/ida-free/) is a code disassembly and debugging tool. Useful when doing 
code analysis, reverse engineering, vulnerability research, and exploit development.
* [OWASP Zed Attack Proxy (ZAP)](https://www.zaproxy.org/docs/) is a free web application scanner, and functionally 
similar to Burp Suite, but offers a different array of features.
* [SQLmap](https://sqlmap.org/) attempts to automatically identify and exploit SQL
injection when supplied with a target URL.
* [w3af](http://w3af.org/) is a web application attack and audit framework 
designed to attempt to find and exploit vulnerabilities in web applications.
* [Wapiti](https://owasp.org/www-community/Automated_Audit_using_WAPITI) is a command-line tool that fuzzes web 
applications during a black box penetration test and attempts to identify SQL injections, XSS, file disclosure 
vulnerabilities, XXE, CRLF, etc.
* [WPScan](https://github.com/wpscanteam/wpscan) is a web application security scanner that focuses on 
WordPress installations. It attempts to identify insecure WordPress configurations and plugins based on versioning
data, username enumeration, known default passwords, exposed files, and a database of known vulnerabilities. 
It requires a license.

## Mobile

* [Android SDK](https://developer.android.com/studio/intro), the official Android API tools, including an IDE for 
developing Android applications. Useful for mobile application and device testing, including source code analysis.
* [APK Studio](https://github.com/vaibhavpandeyvpz/apkstudio) is an IDE designed for reverse engineering Android 
applications: decompile, recompile, sign, and install APKs for Android devices; edit and view code; and it includes 
a hex editor for binary files.
* [ApkX](https://github.com/b-mueller/apkx), a Python wrapper for multiple tools that extract Java source code from 
APK files. Useful for automating the process of extraction, decompilation, and conversion.
* [Drozer](https://github.com/FSecureLABS/drozer) is an Android security assessment framework, which acts as a 
third-party application that interacts with IPC endpoints for other applications and the underlying OS.
Useful for searching for security vulnerabilities by interacting with the target via provided modules.
* [Frida](https://frida.re/) is a mobile testing toolkit that can be used to inject scripts
into black box processes and gain insight into the operations of APIs, private code, and 
running functions during security testing of mobile devices.
* [The Mobile Security Framework (MobSF)](https://github.com/MobSF/Mobile-Security-Framework-MobSF) is a mobile 
pentesting framework that can target Android, iOS, and Windows devices.
* [Objection](https://github.com/sensepost/objection) is a mobile exploitation toolkit that aids in runtime
security testing without needing to jailbreak the device. 
* [Spooftooph](https://www.kali.org/tools/spooftooph/) is a Bluetooth testing tool designed to spoof or clone a 
Bluetooth device name, class, and address. It can be used to scan for Bluetooth
devices in a range, clone a device, and gather information sent to it.

## Network

* [Tcpdump](https://www.tcpdump.org/)
* [Wireshark](https://www.wireshark.org/download.html)
* [Ettercap](https://www.ettercap-project.org/) is an on-path tool for network traffic. It can
be used for ARP spoofing attacks, sniffing network traffic over a live connection, and applying
filters to modify that traffic in real time. Useful when having access to a network and needing to 
intercept or modify traffic between other network endpoints on the same subnet in order to further 
access.
* [Hping](http://www.hping.org/) is a command-line tool for generating TCP/IP packets.
While its functionality has been implemented in Nmap, hping3 is scriptable in the Tcl scripting language, and it 
can render packets into strings-based, human-readable descriptions for ease of writing scripts to perform 
low-level packet manipulation and analysis. It can also be used to spoof source IP addresses and generate large
amounts of traffic in order to explore various DDoS techniques (a very common use case during network pentesting).
* [Impacket](https://github.com/SecureAuthCorp/impacket) is a Python tool suite used for network protocol manipulation.
* [mitm6](https://github.com/dirkjanm/mitm6) intercepts DNS and DHCP queries from
a selected target and operates as a rogue DNS/DHCP server. This can then be used to
redirect victim traffic to other malicious resources or perform relay attacks when used
with tools like ntlmrelayx in Impacket.
* [Ncat](https://nmap.org/ncat/) is an implementation of the Netcat (nc) tool for Nmap. Useful for redirecting TCP and 
UDP ports to other sites, and supports SSL and proxy implementations with SOCKS.
* [Netcat (nc)](https://linux.die.net/man/1/nc) is a tool that is distributed with many
Linux distributions for tasks with TCP or UDP. It is scriptable using Bash, and can be used to transfer files to or
from target machines, implement bind or reverse shells, or directly test a service using a raw connection.
* [Nmap](https://nmap.org/) is a free pentest tool for network discovery and security testing.
* [ProxyChains](https://github.com/haad/proxychains) is useful for bridging networks by creating a
proxy tunnel for any other protocol.
* [Responder](https://github.com/lgandx/Responder) is a tool for responding to LLMNR,
NBT-NS, and MDNS requests and intercepting the resulting data from that exchange.
It can be used to gather Windows challenge hashes resulting from requests to nonexistent
services or other maliciously redirected requests.
* [Wireshark](https://www.wireshark.org/) is a graphical network traffic analyser. It can
be used against packet captures across many kinds of networks and enables deep protocol inspection, 
the ability to perform live packet captures, and analyze PCAPs from other sources. 
Capturing data requires access to the network in question.

## Wireless

* [Aircrack-ng](https://www.aircrack-ng.org/), a wireless test suite. Useful for capturing wireless traffic; replay 
traffic; crack WPA, WPA2 PSK, and WEP; and do attacks such as deauthentication, creating fake access points, and 
injecting packets.
* [EAPHammer](https://github.com/s0lst1c3/eaphammer) is designed for gaining access to wireless networks using 
evil twin attacks against WPA and WPA2 networks and networks using RADIUS. Useful for stealing RADIUS credentials 
with a malicious AP or AD credentials with a hostile portal. 
* [Fern](http://www.fern-pro.com/) is a Python tool for Wi-Fi security auditing and cracking. It can recover WEP, 
WPA, and WPS keys, and can be used for several types of Wi-Fi attacks (Reaver, chopchop, fragmentation attacks, etc.). 
It comes in a [free version onGitHub](https://github.com/savio-code/fern-wifi-cracker) and a paid 
professional version. It requires the aircrack-ng suite, Scapy, and Reaver.
* [Kismet](https://www.kismetwireless.net/) is a wireless security assessment tool that can
detect devices, sniff wireless traffic, and aid with wardriving. It supports Bluetooth and traditional wireless 
networks.
* [mdk4](https://github.com/aircrack-ng/mdk4) is a wireless testing tool used to 
inject frames on several operating systems. Useful for attacks like beacon flooding, denial of service and deauth
attacks, SSID probe and brute-forcing, packet fuzzing, etc.
* [Reaver](https://github.com/t6x/reaver-wps-fork-t6x) is a Wi-Fi brute-forcing tool
designed to attack WPS registrar PINs to get WPA/WPA2 passphrases and can be used for 
the offline pixie dust attack.
* [Wifite](https://github.com/derv82/wifite2) is a Python script for attacking wireless
networks. It can perform the offline pixie dust attacks and online PIN brute-forcing
against WPS networks; capture WPA handshakes and PMKID hashes; and perform
various WEP attacks, including fragmentation, chopchop, and replay attacks. It
requires the aircrack-ng suite for wireless capture, relay, and cracking.

## Authentication

* [Cain](https://web.archive.org/web/20190603235413/http://www.oxid.it/cain.html) is the cracking component of the 
Cain & Abel tool, originally created as a GUI application for Windows 2000 and earlier. 
It can crack passwords using brute force and dictionary attacks, and supports rainbow tables. Password
targets include WEP, NTLM and LM hashes, NTLMv2 hashes, MD5 hashes, SHA-1 and SHA-2 hashes, Cisco IOS and PIX hashes, 
and RADIUS and IKE PSK hashes. The tool is recognised as malware by most host security products. It is only useful 
when other crackers do not support the hash type or when rainbow tables would be faster than GPU-based attacks using 
dictionaries or rules-based brute force. Another tool that implements rainbow tables is RainbowCrack.
* [Hashcat](https://hashcat.net/hashcat/) is a GPU-based cracking engine designed for
brute-force and dictionary attacks using rules and filters. It is designed to target password
hashes and is considered to be the fastest method for password cracking. Useful with a hash that does not pass, or 
when auditing password strength based on a collection of hashes.
* [Hydra](https://github.com/vanhauser-thc/thc-hydra) is a tool for password spraying
and brute-forcing against live services, including HTTP, Oracle, Cisco, POP3, VNC, etc. 
* [John the Ripper (JtR)](https://www.openwall.com/john/) is an offline password cracking tool. For CPU-based cracking, 
JtR is one of the fastest tools for password recovery. JtR implements
different rule sets than other cracking tools, and these rule sets may recover passwords
where other cracking tools fail.
* [Medusa](https://github.com/jmk-foofus/medusa) is a tool similar to Hydra.
* [Patator](https://github.com/lanjelot/patator) is a password brute-forcing tool similar to Hydra and Medusa.

## Social engineering

* [BeEF](https://beefproject.com/) is an exploitation tool for client-side attacks (like XSS and session hijacking) 
against web browsers. It can be used in web-based social engineering attacks by generating and injecting JavaScript 
hooks into web content that allow for interacting with the target browser via a console provided by the BeEF
tool. This can be used to gain footholds on a hooked target, steal credentials, and execute other attacks within 
the context of the browser.
* [Call spoofing tools list](https://www.social-engineer.org/framework/se-tools/phone/caller-id-spoofing/) on the 
Social-Engineer blog. Local and regional laws may affect what is legally allowed
when it comes to caller ID spoofing, so be aware of these limitations as part of the scoping (if done in pentesting 
context).
* [The Social-Engineer Toolkit (SET)](https://github.com/trustedsec/social-engineer-toolkit) is an open-source Python 
toolkit for pentesting using social engineering. It has integrations with Ettercap, Metasploit, and other tools.

## Exploitation

* [Empire](https://www.powershellempire.com/) and its later version 
[BC-security Empire](https://github.com/BC-SECURITY/Empire) is a PowerShell exploitation framework. Many of the tools 
still work, and are still used in practice. 
These tools are very likely to be detected in advanced environments unless additional methods of concealment (using 
PowerPick or obfuscation techniques) are also used. The framework includes many PowerShell scripts and modules
designed for gathering credentials (running Mimikatz), discovery and reconnaissance, privilege escalation, lateral 
movement, and persistence, etc.
* [Immunity Debugger](https://www.immunityinc.com/products/debugger/) is useful for exploit development, malware 
analysis, and reverse engineering. It can graphically render functions and program flows, facilitates heap analysis, 
and implements a Python API for scriptability. The Mona Python plugin, for example, supports figuring out offsets 
for buffer overflows, identifying ROP chains, and exploring more.
* [Metasploit](https://www.metasploit.com/) is a pentesting framework that includes
many community-contributed modules for attack. It is useful for most phases of penetration testing, including 
reconnaissance, vulnerability identification, exploitation, and command and control.

## Steganography

* [Coagula](https://www.abc.se/~re/Coagula/Coagula.html) turns images into sounds. Useful for concealing data within 
sound files (data exfiltration), by bypassing data loss prevention tools or other security controls. Files can be
reassembled from the sound file using a tool such as Audacity, Spek, or Sonic Visualiser.
* [OpenStego](https://www.openstego.com/) is a steganography tool that can hide and
recover hidden data from files.
* [Snow](http://manpages.ubuntu.com/manpages/bionic/man1/stegsnow.1.html) is a steganography tool that hides data 
using the white space of ASCII messages.
* [Steghide](http://steghide.sourceforge.net/) can hide or retrieve data hidden inside image or audio files. The 
resulting file looks and sounds exactly like the original file from a human perspective. Data can be encrypted when 
hidden.
* [TinEye](https://tineye.com/) is a reverse image search tool. You can load or reference
an image and then search for it online.

## C2

* [Covenant](https://github.com/cobbr/Covenant) is a .NET C2 framework designed for collaboration during an attack 
operation.
* [SilentTrinity](https://github.com/byt3bl33d3r/SILENTTRINITY) is a modern, asynchronous, multiplayer & multiserver 
C2/post-exploitation framework powered by Python 3 and .NETs DLR.

## Post-exploitation

* [CrackMapExec (CME)](https://github.com/byt3bl33d3r/CrackMapExec) is designed to stealthily automate security 
testing of Active Directory environments. It uses native tools to "live off the land" as part of its tactic to remain
undetected and evade security controls that would otherwise block attack tools, and uses Impacket and PowerSploit to 
assess privilege issues and perform attack actions.
* [Mimikatz](https://github.com/gentilkiwi/mimikatz) is a tool used to extract authentication information from 
Windows systems. This includes Kerberos tickets, plaintext
passwords, password hashes, PIN codes, etc. It can be used for pass-the-hash and pass-the-ticket attacks, 
and Kerberoasting attacks by building golden tickets. Useful during post-exploitation, for gathering additional 
credentials for lateral movement or privilege escalation.
