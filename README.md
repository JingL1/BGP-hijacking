# BGP-hijacking-attacks

Gatech CS6250, 2020 Summer.
The demo creates the network topology based on Mininet, simulating attacks on Border Gateway Protocol (BGP) between AS.

## Description & Tools
- This interactive demonstration using a Mininet Topology and simulated prefixes/paths.
The demo creates the [**network topology**](fig2_topo.pdf), consisting of six ASes and their peering relationships. AS6 is the malicious AS that will mount the attack. 
- We will be simulating this network in `Mininet`. 
- Each router in AS runs a routing daemon (`quagga`), communicates with other ASes using BGP(bgpd),and configures its own is olated set of routing entries in the kernel (`zebra`). 
- Each AS router has multiple IP addresses, to connect to the hosts in the AS and to other routers.