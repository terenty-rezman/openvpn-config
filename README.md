# OpenVPN configuration multiple clients 

The task was to allow Windows Remote Desktop access from home pc to work pc. Home pc and work pc are located in their own separate networks with differnt ISPs and behind NAT. The solution is put them into one virtual LAN (VPN) so the Remote Desktop connetcion happens as if they were on the same LAN.

__3__ separate hosts involved to solve the problem:
* __server__ (virtual ip 10.8.0.1) is rented VPS server with public ip running Ubuntu 16.04 and OpenVPN server 
* __client1__ (virtual ip 10.8.0.2) is home pc running Windows 10 (openvpn client)
* __client2__ (virtual ip 10.8.0.3) is remote work pc running Window 8.1 (openvpn client)

# features 

with this config:
 * __all hosts see each other__
 * __all hosts have static ip__
