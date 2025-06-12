---
layout: page
title: Thesis Abstract
permalink: /abstract/
noindex: true
---



The increasing complexity of modern computing systems and their exposure to the world-wide web expose sensitive data to a range of security threats from remote adversaries. Bugs in software can lead to run-time attacks that gain direct access to sensitive data in memory. Furthermore, hardware and/or compiler optimizations can expose sensitive data to side-channel leakage, even in the absence of software bugs.

As business needs evolve, different usage scenarios, such as outsourced computation, have gained popularity, making the task of protecting data confidentiality more complex. This thesis investigates how confidentiality of sensitive data at run-time can be efficiently preserved through hardware-assisted mechanisms. I consider a range of usage scenarios and threat models, from protecting data sent to remote servers for outsourced computation by untrusted code, to protecting data processed locally from other vulnerable or malicious parts of the system.

Specifically, this thesis addresses: 1) (how) can we protect sensitive data sent to a remote server for outsourced computation efficiently? I tackle this by proposing BliMe, a novel architecture that relies on remote attestation and hardware-enforced data obliviousness to protect data processed by untrusted code, both from direct access and side-channel leakage. Next, I address the two following questions: 2) how to protect data from untrusted code in a local setting, for which I propose PBI, a novel hardware memory safety primitive that can be used to implement efficient and secure sandboxing and in-process isolation, and 3) how to reduce the overhead of side-channel protection to near-zero, for which I propose CacheSquash, a software-transparent hardware mechanism to effectively harden against transient attacks such as Spectre and Meltdown. 4) Finally, I address how to efficiently combine memory safety and side-channel protection mechanisms for data confidentiality. For this, I propose BLACKOUT, a hardware-software extension to CHERI that enforces data-oblivious computation on sensitive data, and inherits the memory safety properties of CHERI, all while introducing minimal overheads.