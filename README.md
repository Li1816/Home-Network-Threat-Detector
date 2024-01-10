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
![pi_hole1](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/a86436cc-9dc8-4446-93d9-ba3a53482ef2)

![pi_hole2](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/bc082801-99c1-4f18-8203-0f460fd67dfa)
**Secondly, it uses snort for singture detection IDS for network traffic inspection and alerting upon finding suspious traffic, displaying malware signture**
![Snort1](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/826a84d7-3748-45ff-be01-5e5313859b07)
![snort2](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/bc234aea-ab60-48f8-9b8d-8804da1ff1ba)
**Thirdly, it uses OPenMediaVault for monitoring cpu, memory, and disk usage. Storing authentcaiton and boot logs, and alerting upon unexpected login or cron-job**
![OMV1](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/c9f558f9-a228-472f-91ed-be42782f0012)
![OMV2](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/c5d46a08-fba8-4200-a943-9f7cf33b11a8)
**It uses Fail2Ban to implment account lock-out policies for access control**
![image](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/72b6667b-7e0d-4648-bf93-120766f03cf2)
**Lastly, it uses tailscale for on-home VPN. Ensuring I can have this even when in public network and prevent eversdropoing via the secure tunle created**
![TailScale1](https://github.com/Li1816/Home-Server-Network-Threat-Detector/assets/155325489/0c6cecfc-4a6e-4037-8c7d-b483e0d401ff)




