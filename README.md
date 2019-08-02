# sfndnspoc
Skillet to automate the deployment of a DNS based SafeNetworking POC in TAP Mode

1.) Configure Syslog Profile for SafeNetworking Server
2.) Configure Interafce for TAP Mode - Make Sure this is connected to your customers SPAN port and they are mirroring DNS traffic
3.) Configure TAP Zone 
4.) Configure Spyware Profile with DNS Alerting - You must have a DNS Security Subscription for this to work.
5.) Configure Forwarding profile for threat logs and URL categories (Malware, High-Risk and Phishing)
6.) Configure Rule to forward all mirrored traffic to SafeNetworking Server

This skillet is tested for SafeNetworking 4.0 and PAN-OS 9.0
