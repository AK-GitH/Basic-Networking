# Network Topology Design Using GNS3

In this project, we use **GNS3**, a powerful network simulation tool, to build and experiment 
with two distinct network topologies named **Topology A** and **Topology B**. The 
goal is to understand how different network designs impact connectivity and fault tolerance.

## What We Are Doing:

- **Topology A**: This network design includes at least 15 end-user devices (like PCs) and 4 
  routers. The network uses **RIP or static routing** and is divided into at least 5 separate 
  subnets. However, there's a challenge: the design has a **single point of failure** — one 
  crucial router. If this router fails, communication between certain parts of the network will break down.
  
- **Topology B**: Similar to Topology A with the same number of devices and subnets, but 
  designed with **fault tolerance**. Here, if any one router is disabled, communication between 
  all subnets (except those directly dependent on the disabled router) will still continue. This design 
  demonstrates a more robust and resilient network setup.

## Communication Testing:

Both topologies allow any two hosts to communicate using different network protocols, such as 
**ping, TCP, and UDP**. This lets us experiment with various ways devices can exchange data in a 
simulated network environment.

This project introduces concepts like routing, subnetting, and network resilience, making it a great exercise 
for learning how real-world networks operate and how to plan for potential failures.
