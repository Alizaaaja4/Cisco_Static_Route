# Cisco Static Route
Practice Simulation of Static Routing in Cisco Packet Tracer Application

Repository Title : Static Routing in Cisco Packet Tracer

Description : This simulation is an exercise to visualize the concept of routing using the static method. There are three rooms involved, each equipped with a computer, laptop, and switch. The connection between devices is established through two routers configured with static routing.

## Designed Network
![Design Cisco](https://github.com/Alizaaaja4/Cisco_Static_Route/blob/main/Dokumentasi%201.jpeg)

### Static Routing
Static routing is a method of sending data packets in a computer network that uses static routing tables as a reference to determine the route of the data packets

#### Change the Router Name
    Router> enable
    Router# configure terminal
    Router(config)# hostname [new name]
    
    ---- example :
    
    Router(config)# hostname RouterA
    RouterA(config)# exit
    RouterA# ....

#### Using Encryption
    Router> enable
    Router# configure terminal
    Router(config)# enable secret [name password]
    Router(config)# ....

#### Connect Device to Router
    Router> enable
    Router# configure terminal
    Router(config)# interface [ex: fa1/0]
    Router(config-if)# ip address [ip default] [subnetmask]
    Router(config-if)# no shutdown
    Router(config-if)# exit
    Router(config)# ....

#### Connect Router to Router (Static Methods)
    Router> enable
    Router# configure terminal
    Router(config)# ip route [ip destination] [subnetmask] [ip gateaway]
    Router(config)# exit
    Router# show ip route
