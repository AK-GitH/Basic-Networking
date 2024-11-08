# Network Topology Design Using GNS3

In this project, we will reconfigure two network topologies that were previously built using **GNS3**. These topologies will now use different routing protocols, and we will also explore how these protocols behave in real-world scenarios.

## Topology Overview:

- **Topology A**: Initially designed with basic routing, it will now be reconfigured to use **EIGRP (Enhanced Interior Gateway Routing Protocol)**.
  
- **Topology B**: Similarly, this topology will be reconfigured to use **OSPF (Open Shortest Path First)** for routing.

## Task Steps:

1. **Reconfigure Routing Protocols:**
    - **Topology A**: Change the routing protocol to **EIGRP**, which is a distance-vector routing protocol that uses metrics like bandwidth and delay to determine the best path.
    - **Topology B**: Change the routing protocol to **OSPF**, which is a link-state routing protocol that builds a topology map of the network and calculates the best path based on cost.

2. **Test the Behavior of Each Protocol:**
    - Remove single links or routers while the network is running (without restarting any devices). Observe how the network reacts and how the routing tables update in real time.
    - Use **Wireshark** to monitor and capture routing packets. These packets will help you understand how each protocol detects and reacts to network changes.
    - Take notes and screenshots as you observe the following:
      - Which routing messages are sent when changes are made (e.g., when a link goes down)?
      - What happens to the routers' routing tables?

3. **Connect the Two Topologies Using BGP:**
    - **BGP (Border Gateway Protocol)** will be used to connect Topology A and Topology B.
    - Create a link between the two topologies and configure **BGP** on the two routers at the ends of the link.
    - Configure each router with its own **AS (Autonomous System) number**. This allows the two topologies to exchange routing information.
    - Use **BGP redistribution** to allow routes from EIGRP and OSPF to be shared with the other topology. You only need to configure BGP on the routers at the ends of the link; no other routers need BGP configuration.

