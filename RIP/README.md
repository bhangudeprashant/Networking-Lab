# RIP Lab

## Objective
Configure RIPv2 dynamic routing between routers in Cisco Packet Tracer.

## Topology
![Topology](topology.png)

## Commands Used

Router> enable
Router# configure terminal
Router(config)# router rip
Router(config-router)# version 2
Router(config-router)# network 192.168.1.0
Router(config-router)# network 10.0.0.0
Router(config-router)# no auto-summary
Router(config-router)# end

## Verification
Router# show ip route
Router# show ip protocols
Router# ping 192.168.2.1

## Result
Routes learned via RIP are shown with `R` in the routing table and end-to-end ping is successful.

## Packet Tracer File
[Download RIP_Protocol2.pkt](RIP_Protocol2.pkt)
