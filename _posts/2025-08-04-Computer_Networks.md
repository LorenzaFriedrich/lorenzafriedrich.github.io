---
title: CS 6250 - Computer Networks
date: 2025-08-04 12:36:00 +0800
categories: [GaTech OMSCS, Computer Networks]
tags: [python]     # TAG names should always be lowercase
description: Overview of Computer Networks   
---
# Welcome
#### Note
For all OMSCS courses - I will provide pseudocode and video links, but I need to keep code in a private repository to uphold the honor code, descriptions, notes, etc are below.

## Individual Assignments 
I lost most of my notes (sadly) when I pulled my notes from obsidian. This course has two exams that are multiple choice, open book quizzes and 5 projects. 
It's a good course! super comprehensive, the absolute best resource is the Jim Kurose videos and text books. Below is a high level overview of whats covered in the course projects. If I am able to recover my notes I'll add them, if I end up revisiting my code, I'll add psuedocode in here as well. 

### Distance Vector
In the lectures, you learned about Distance Vector (DV) routing protocols, one of the two 
classes of routing protocols. DV protocols, such as RIP, use a fully distributed algorithm to find 
shortest paths by solving the Bellman-Ford equation at each node. In this project, you will 
develop a distributed Bellman-Ford algorithm and use it to calculate routing paths in a network. 
This project is similar to the Spanning Tree project, except that we are solving a routing 
problem, not a switching problem.  
### Spanning Tree Protocol
In this project, you will add to those concepts by developing a distributed 
algorithm that can run on an arbitrary layer 2 topology. We will simulate the communications 
between the switches with Messages.
### SDN Firewall
In this project, you will use Software Defined Networking (SDN) principles to create a configurable firewall using 
an OpenFlow enabled Switch. The Software Defined Networking (OpenFlow) functionality allows you to 
programmatically control the flow of traffic on the network. 
### BGP Hijacking

In this project I explored a vulnerability of the Border Gateway Protocol (BGP). 
Specifically, your goal is to recreate a BGP Hijacking attack where a “rogue” AS (autonomous 
system) hijacks a prefix from another AS, thereby “stealing” traffic. I reviewed a Simple BGP Hijacking on a customized topology and an Advanced BGP Hijacking on a customized topology 
All materials and code is in github private repo 
### BGPM
In this project we will use the BGPStream tool and its Python interface PyBGPStream to 
understand the BGP protocol and interact with BGP data. The goal is to gain a better 
understanding of BGP and to experience how researchers, practitioners, and engineers have 
been using BGPStream to gain insight into the dynamics of the Internet. 
In this task you will measure the growth over time of Autonomous Systems and advertised 
prefixes. The growth of unique prefixes contributes to ever-growing routing tables handled by 
routers in the Internet core
- Task 1A: Unique Advertised Prefixes Over Time 
This task will use cache files from the rib_files subdirectories. These are RIB files, so you will pass “rib-file" in your call to set_data_interface_option(). Using the data from cache files, measure the number of unique advertised prefixes over time.
- Task 1B: Unique Autonomous Systems Over Time 
This task will use cache files from the rib_files subdirectories. These are RIB files, so you will 
pass “rib-file" in your call to set_data_interface_option(). Using the data from the 
cache files, measure the number of unique Autonomous Systems over time
- Task 1C: Top-10 Origin AS by Prefix Growth 
- Task 2: Routing Table Growth: AS-Path Length Evolution Over Time 
- Task 3: Announcement-Withdrawal Event Durations 
- Task 4: RTBH Event Durations 
This task will use cache files from the update_files_blackholing subdirectories. These are update files, so you will pass “upd-file" in your call to set_data_interface_option(). Using the data from the cache files, we will identify events where prefixes are tagged with a Remote Triggered Blackholing (RTBH) community and measure the time duration of the RTBH events by completing the function rtbh_event_durations().



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


