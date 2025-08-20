---
title: CS 6250 - Computer Networks
date: 2025-08-04 12:36:00 +0800
categories: [GaTech OMSCS, Computer Networks]
tags: [python]     # TAG names should always be lowercase
description: Overview of Computer Networks   
---
# Welcome
#### Note
For all OMSCS courses - I will provide pseudocode and video links, but I need to keep code in a private repository to uphold the honor code. Descriptions, notes, etc are below.

# Individual Assignments

This course has two exams that are multiple-choice, open-book quizzes, and five projects. It’s a good course—super comprehensive—and the absolute best resource is the Jim Kurose videos and textbooks. Below is a high-level overview of what’s covered in the course projects. If I am able to recover my notes I’ll add them, and if I end up revisiting my code, I’ll include pseudocode here as well.

# Distance Vector

In the lectures, we covered Distance Vector (DV) routing protocols, one of the two main classes of routing protocols. DV protocols, such as RIP, use a fully distributed algorithm to find shortest paths by solving the Bellman-Ford equation at each node. In this project, I developed a distributed Bellman-Ford algorithm and used it to calculate routing paths in a network. This project is conceptually similar to the Spanning Tree project, except that here we solved a routing problem rather than a switching problem.

# Spanning Tree Protocol

This project built on the foundation of distributed algorithms by focusing on the Spanning Tree Protocol. The goal was to develop a distributed algorithm that could run on an arbitrary Layer 2 topology. We simulated communications between switches using messages, reinforcing the concepts of how switches prevent loops in a network while maintaining connectivity.

# SDN Firewall

In the SDN Firewall project, I applied Software Defined Networking (SDN) principles to create a configurable firewall using an OpenFlow-enabled switch. Leveraging SDN and OpenFlow functionality, I was able to programmatically control the flow of traffic across the network. This project highlighted the flexibility and programmability of SDN for managing and securing modern networks.

# BGP Hijacking

The BGP Hijacking project explored a well-known vulnerability of the Border Gateway Protocol (BGP). The goal was to recreate a BGP hijacking attack where a rogue Autonomous System (AS) hijacks a prefix from another AS, effectively “stealing” traffic. I worked through both a simple hijacking scenario on a custom topology and an advanced hijacking scenario on a more complex topology. All related code and materials are stored in a private GitHub repository.

# BGPM

In the BGPM project, I used the BGPStream tool along with its Python interface, PyBGPStream, to analyze BGP data and better understand the protocol in practice. The objective was to gain insight into how researchers, practitioners, and engineers use BGPStream to study the dynamics of the Internet. Several tasks were completed as part of this project. First, I measured the growth of unique advertised prefixes over time using RIB files from the rib_files subdirectories. Next, I measured the growth of unique Autonomous Systems over time using the same dataset. I also identified the top 10 origin ASes by prefix growth. Moving beyond prefix growth, I analyzed routing table growth by examining AS-path length evolution over time. Additional tasks included measuring announcement-withdrawal event durations and evaluating RTBH (Remote Triggered Blackholing) event durations using update files from the update_files_blackholing subdirectories. Together, these analyses provided a comprehensive view of BGP growth, dynamics, and mitigation mechanisms.

## Resources

### Text Books
- https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm

### Github Repo (private)
- https://github.com/LorenzaFriedrich
### Online materials
- https://www.cloudflare.com/learning/security/glossary/bgp-hijacking/
- https://www.cisco.com/c/en/us/td/docs/ios/iproute_bgp/command/reference/irg_book.html
- https://bgpstream.caida.org/
- https://shashi-prabh.github.io/teaching/computer_networks_2025/course_calendar.html


