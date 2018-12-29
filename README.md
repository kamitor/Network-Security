# Network-Security
Introduction by Nomaster - Part of the chaos dorf and freifunt community.

Questions you often get: Is this network secure? 
Well, the network is never secure, it's your computer who is suppose to be security..
# Introduction


Every computer has a MAC adress
IP Adress

Everything else 
Connection protocols *TCP UDP
Application protocols (HTTPS etc )


What you want to acomplish is a secret between the server and the client. 


Example:
IP                          MAC (burned into the device)
192.168.0.1                 06:01:02
fd00:1 

Example ARP spoofing; "Old school attack" however most networks would still be ready for this type of attack.
CLIENT ->> ROUTER 
CLIENT SAYS:  Who has IP?
ROUTER ->> CLIENT
ROUTER SAYS: IP is at MAC 


Spoof : Attacker sends unsolicited arp for router IP adress
Client learns attacks mac adress from this ip adress
client sends packets to attacker
attacker forwards packets and observers traffic.

DNS Hijacking;
Domain Name system translate host names to Ip adresses
CLient asks for an A to the DNS
The DNS replies with an IP. 
With an attack the IP 

Rogue Access Points
Wifi works like cabled network; When you make a wifi connection it looks like a cable connection. However, when you have multipule access points, like a large network your computer switches beacons seamlessly.

ATTACK on a 802.11 (wireless) connection
Attacker sends SSID from own access point
Client connects to attack's AP
Attacker forwards packets and observes traffic.
Countermeasures are certificates for access points to make sure that the connections are valid.


Conclusions:

Protocol definitions and standards are valuable
By learning how to attack, you learn how to defend yourself.

Use Let's encrypt certificates.

Look at traffic with tcpdump or wireshark
Show routing with traceroute or mtr
learn packet spoofing with Scapy

# counter measures

- Rate limiting
- USe HTTPS and check certificates
- Use WPA EAP and check certficiates. 
- Use Let's encrypt certificates


# where to start
- Get old pc with linux : who has raw access - With Arch 
Use TCP dump to see where
Kismit : give me a list of wireless beacons. Passive scanning, as long as you do passive scanning you will not interrupt anyone.


# Kismet
install with apt-get install kismet
If you have a large attack service: the more services, the more sofware you have installed, the larger the ability for a hacker to be able to attack you.

once the kismet server is started
open another terminal and say ip link show






Client 

# tools
