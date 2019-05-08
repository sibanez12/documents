
# Tutorial Program

* 9:00 am - 10:00 am P4 Language Overview
* 10:00 am - 10:30 am Collaborative Lab Exercises - Part I
* 10:30 am - 11:00 am Tea/Coffee Break
* 11:00 am - 12:30 pm Collaborative Lab Exercises - Part II
* 12:30 pm - 2:00 pm Lunch Break
* 2:00 pm - 3:15 pm Mini Research Workshop - Part I
* 3:15 pm - 3:45 pm Tea/Coffee Break
* 3:45 pm - 5:30 pm Mini Research Workshop - Part II

# Call for Participation

This tutorial will provide participants with a hands-on experience working with the P4 language ([www.p4.org](www.p4.org)). Attendees will learn how to express conventional and novel data-plane applications in the P4 language, and how to compile, execute, and evaluate P4 programs using Mininet, a network emulation framework.

# Important Dates

August 19, 2019

# Outline

The goal of the tutorial is two-fold:

1. We will emphasize aspects of data-plane programming that were glossed over in previous P4 tutorials, including the P4 langauge-architecture separation and stateful packet processing. Through a series of exercises, we will show them how to prototype network applications in the P4 language and compile them to programmable devices. By the end of the tutorial, attendees will be able to implement novel data-plane features in P4, and evaluate their programs using Mininet, a network emulation framework.
2. We will expose attendees to exciting new applications and future research directions within the P4 community.

More specifically, we plan to cover the following topics:
* P4 language overview and the language-architecture separation
* Hands-on training of P4 development environment
    * Compiler
    * Debugger
    * Behavioral model
    * Lab exercises
* Mini-workshop – invited talks focusing on the following categories
    * Emerging P4 applications
    * Future research directions
    * New P4 targets and tools
    * Teaching resources

# Audience Expectations and Prerequisites

Attendees will be expected to have basic familiarity with the P4 lanaguage. Attendees will also be expected to bring their own laptops. We will provide a VM image containing all the necessary packages and tools. The P4 specification is publicly available at the P4 website under an Apache license. Key development tools (front-end compiler and software switch capable of running P4 programs) are available as open-source tools (http://github.com/p4lang).

# Background

P4 (www.p4.org) is a programming language for describing how network packets should be processed on a variety of targets ranging from general-purpose CPUs to network processors, FPGAs, and custom ASICs [1]. P4 was designed with three goals in mind: (i) *protocol independence*: devices should not “bake in” specific protocols; (ii) *field re-configurability*: programmers should be able to modify the behavior of devices after they have been deployed; and (iii) *portability*: programs should not be tied to specific hardware targets. 

The P4 community has created – and continues to maintain and develop – a language specification, a set of open-source tools (compilers, debuggers, code analyzers, libraries, software P4 switches, etc.), and sample P4 programs with the goal of making it easy for P4 users to quickly and correctly author new data-plane behaviors. New ideas are being developed in P4, prototyped as new forwarding behaviors, and published at some of the top conferences in networking. Existing data-plane features typically realized in a fixed-function logic are also being authored in P4.

Recently, P4 evolved to embrace the functional and architectural heterogeneity of various targets while keeping the language core simple and clean. One manifestation of this change is the development of a Portable Switch Architecture (PSA). The PSA describes common capabilities of network switch devices which process and forward packets across multiple interface. This specification improves the portability and composability of a P4 program, allowing P4 consumers and target providers to reuse their code. Second, in the past year, there have been significant new developments on the control-plane API for P4 pipelines. This tutorial will introduce P4 Runtime, the silicon-independent and protocol-independent API that can be auto-generated from an unambiguous definition of a packet processing pipeline in P4. Third, P4 continues to be a transformative technology in networking, and an increasingly popular choice for developing novel data-plane designs. Examples include P4 programs that realize in-band network telemetry [4], path-condition-aware adaptive routing [5], a better NetFlow [6], L4 connection load-balancing [7], replicated storage systems [8], and fast failure detection and recovery [9]. There are also new P4 programmable targets available to the research community [10]. We believe there are many opportunities for academic researchers to help evolve the design of the language, discover new implementation techniques, and develop use cases.

# Organizers

**Stephen Ibanez** is a PhD Candidate at Stanford University working with Professor Nick McKeown. His research focuses improving the programmability of network devices in two key areas: traffic management and stateful packet processing. He leads the programmable traffic management sub-working group within P4.org. He has hosted numerous P4 related tutorials at venues including SIGCOMM and P4 Workshops, and he also leads the P4->NetFPGA community of developers and users.

**Changhoon (Chang) Kim** is CTO of Applications at Barefoot Networks and is also working actively for the P4 Language Consortium (P4.org). Before getting involved with P4.org and Barefoot, he worked at Windows Azure, Microsoft’s cloud-service division, and led engineering and research projects on the architecture, performance, and management of datacenter networks. Chang is interested in programmable networking, network monitoring and diagnostics, application acceleration, self-configuring/running networks, and debugging and diagnosis of large-scale distributed systems. Many of his engineering and research contributions — including In-band Network Telemetry, Tiny Packet Programs, VL2, Seawall, EyeQ, Ananta, and SEATTLE — are adopted in large production systems and services. He received a few awards, including best paper awards from top-notch conferences, including SIGCOMM, NSDI, and FAST.


# References

[1] Pat Bosshart, et al. "P4: Programming protocol-independent packet processors," ACM SIGCOMM CCR, 2014, 44(3): 87-95.

[2] http://p4.org/p4/p4-and-open-vswitch/

[3] https://github.com/blp/ovs-reviews/tree/p4

[4] Changhoon Kim, et al. “In-band Network Telemetry via Programmable Dataplanes,” demo at SIGCOMM 2015 and SOSR 2015.

[5] Naga Katta, et al. "HULA: Scalable Load Balancing Using Programmable Data-Planes," Proceedings of the ACM SOSR, 2016.

[6] Yuliang Li, et al. “FlowRadar: A Better NetFlow for Data Centers,” Proceedings of the USENIX NSDI, 2016.

[7] Miao, Rui, et al. "Silkroad: Making stateful layer-4 load balancing fast and cheap using switching asics." SIGCOMM, 2017.

[8] Xin Jin, et al. “NetChain: Scale-Free Sub-RTT Coordination,” Proceedings of the USENIX NSDI, 2018.

[9] Holterbach, Thomas, et al. "Blink: Fast connectivity recovery entirely in the data plane." Proceedings of the USENIX NSDI, 2019.

[10] Ibanez, Stephen, et al. "The P4->NetFPGA Workflow for Line-Rate Packet Processing." Proceedings of the ACM/SIGDA FPGA, 2019.

