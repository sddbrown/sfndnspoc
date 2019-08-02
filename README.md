# SafeNetworking DNS TAP MODE POC Skillet
Skillet to automate the deployment of a DNS based SafeNetworking POC in TAP Mode

#### Installation and usage
1. Get [Panhandler](https://panhandler.readthedocs.io/en/latest/overview.html) running on your local [docker](https://docs.docker.com/)
2. You need to import the skillet via a Panhandler repo. Add the skillet files either as-is or together with other skillets to a repo. If you have access to the original repo you can also import directly from [github](https://github.com/sddbrown/sfndnspoc.git)
add or If you can not access it create your own repo and push the archive that came along this readme. 

## What this Skillet will do
* Configure Syslog Profile for SafeNetworking Server
* Configure Interafce for TAP Mode - 
* Make Sure this is connected to your customers SPAN port and they are mirroring DNS traffic
* Configure TAP Zone 
* Configure Spyware Profile with DNS Alerting - You must have a DNS Security Subscription for this to work.
* Configure Forwarding profile for threat logs and URL categories (Malware, High-Risk and Phishing)
* Configure Rule to forward all mirrored traffic to SafeNetworking Server

#### This skillet is tested for SafeNetworking 4.0 and PAN-OS 9.0
