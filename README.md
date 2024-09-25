Router _1

Router>en

Router#config

Router#configure ter

Router#configure terminal 

Enter configuration commands, one per line.  End with CNTL/Z.

Router(config)#inter

Router(config)#interface fa0/0

Router(config-if)#ip address 172.17.10.1 255.255.255.0

Router(config-if)#no sh

Router(config-if)#no shutdown 



Router(config-if)#exit

Router(config)#inter

Router(config)#interface fa1/0

Router(config-if)#ip address 192.168.10.1 255.255.255.0

Router(config-if)#no sh

Router(config-if)#no shutdown 


Router(config-if)#ip dhcp excluded-address 192.168.10.1 192.168.10.10

Router(config)#ip dhcp excluded-address 172.17.10.1 172.17.10.10

Router(config)#ip dhcp excluded-address 172.17.10.254

Router(config)#ip dhcp excluded-address 192.168.10.254

Router(config)#ip dhcp pool LAN_POOL_CSE

Router(dhcp-config)#network 172.17.10.0 255.255.255.0

Router(dhcp-config)#default-r

Router(dhcp-config)#default-router 172.17.10.1

Router(dhcp-config)#exit

Router(config)#ip dh

Router(config)#ip dhcp p

Router(config)#ip dhcp pool LAN_POOL_EEE

Router(dhcp-config)#network 192.168.10.0 255.255.255.0

Router(dhcp-config)#de

Router(dhcp-config)#default-router 192.168.10.1

Router(dhcp-config)#end



Router#con

Router#conf

Router#configure ter

Router#configure terminal 

Enter configuration commands, one per line.  End with CNTL/Z.

Router(config)#ip route 0.0.0.0 0.0.0.0 ser2/0

Router(config)#interface ser2/0

Router(config-if)#ip address 20.20.20.1 255.255.255.252

Router(config-if)#clock rate 64000

Router(config-if)#no sh

Router(config-if)#no shutdown 

