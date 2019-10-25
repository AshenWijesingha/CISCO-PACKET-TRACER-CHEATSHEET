#CISCO Packet Tracer  
-----------------------
This is a cheatsheet of the cisco packet tracer software.

#Basics:  

* For connecting different types of devices we use copper straight through connection
* For Same types of devices use cross over connection
* Use roll over only for CISCO connection
* Serial DTE and DCE connection (Serial Data Terminal Equipment and Serial Data communication equipment). DCE needs clock rate to be set but DTE doesn't.
* Router is considered as a PC so when connecting router with pc we use cross over
* Two types of ip: 
  1. DHCP (Dynamic Host Configuration Protocol)
  2. Static
* Router uses Routing table / a Software table for looking up addresses to pass data. This table is generated using protocol. 
* Router always prefer static over Dynamic if both options available
    
#Convention:

Generally, last host address of a subnetwork is used as a gateway address (i.e router ip)

#Commands in the CLI of router:

* Use `n` for escaping system config dialogue
* `Router>` prompt indicates user execution mode
* `en` enables Execution privilege mode indicated with a `Router#` prompt
* `config t` enables global config mode  `Router(config)#` 
* interface command `int <port>` example: `int fa0/0`
* set ip and subnet mask using  `ip address <ip address> <subnetmask>`  
  i.e: `ip address 192.168.1.126 255.255.255.128`
* rip configuration  `router rip` then to add network use `network <network address>`
* `show ip route`  to see routing table
* `show ip protocols` (in privilege mode) to see ip protocols
* ospf configuration `router ospf <process id>` then to add network use `network <network address> <wild card mask> area <id> `
* `show ip ospf neighbor` to see neighbor 
* `show ip ospf interface` for hello and dead interval 
