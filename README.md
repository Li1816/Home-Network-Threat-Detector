# Home-Network-Threat-Detector

<p>This programs aims to imporve privacy, detect incicator of compromise, and esblishe secure VPN tunnel of Gonghan's family. It provides various security controls and functinolity by incoparting DNS-Sinkhole, IDS, System Health Montioring, Account lockout and VPN Tunneling. 

## Tools used:
- Pi-Hole: is used to serve as a DNS-Sinkhole for filetring out ads, trackers, and malious websites. 
- Snort: is used to as Intrusion Detection System for inspecting network traffic and alerting on Indicator of Compromise
- OpenMediaVault: is used to monitor system's CPU, Memory, Disk usage, and alerting via email when unexpected Authenticaion attmpt happens
- Fail2ban: is used as an account lock-out access control
- TailScale: is used for esblishing secure VPN tunneling connection to prevent evsdroping


## Controls Applied Walk-Through:

**Firstly, this program uses pi-hole as a DNS sinkhole for filtering out Ads, Trackers, and Malious Websites. It incorptrated block list and Cloudfare 1.1.1.2 for DNS query for additional malware fieltering**

**Secondly, it uses snort for singture detection IDS for network traffic inspection and alerting upon finding suspious traffic, displaying malware signture**

**Thirdly, it uses OPenMediaVault for monitoring cpu, memory, and disk usage. Storing authentcaiton and boot logs, and alerting upon unexpected login or cron-job**

**Lastly, it uses tailscale for on-home VPN. Ensuring I can have this even when in public network and prevent eversdropoing via the secure tunle created**





