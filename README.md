# Home-Network-Threat-Detector

<p>Preventing maliouse websites and imporiving qulity of life, the Network Threat Detector uses DNS Sinkhole, IDS, Automatically alerting, and VPN use these security contorl implmented on raspberry pi.

## Tools used:
- Python/Selenium: is used because each free games is dynamically generated using Javascript.
- Pandas: is used to store and organize all the data scraped.
- Pickle: is used to store and load cookies to avoid pop up alerts.
- Twilio:  is used to send a copy of the info to the user's phone. 
- Window Task Scheduler: is used so that this program can execute automatically.


## Controls Applied Walk-Through:

**Firstly, this program uses pi-hole as a DNS sinkhole for filtering out malious Ads, Tracking, and Websites. It incorptrated block list and Cloudfare 1.1.1.2 for DNS query for additional malware fieltering**

**Secondly, it uses snort for singture detection IDS for network traffic inspection and alerting upon finding suspious traffic, displaying malware signture**

**Thirdly, it uses OPenMediaVault for monitoring cpu, memory, and disk usage. Storing authentcaiton and boot logs, and alerting upon unexpected login or cron-job**

**Lastly, it uses tailscale for on-home VPN. Ensuring I can have this even when in public network and prevent eversdropoing via the secure tunle created**





