---
title: "SysNetS Lab - Research"
layout: textlay
excerpt: "SysNetS Lab -- Research"
sitemap: true
permalink: /research/
---

# Research

SysNetS Lab focuses on ensuring the security and privacy of wireless communication protocols (e.g., cellular networks-4G/5G, Bluetooth, VoWiFi, vehicular, WiFi, and IoT) with respect to their design and implementation. The aim is to develop tools that systematically analyze real-world systems and widely used protocols using formal verification, program analysis, machine learning, natural language processing, and software testing techniques. Furthermore, with the advent of the next generation of networks (6G and beyond), the lab’s future goal is to ensure the resilience (reliability, adaptability, and security) of future network generations and develop protocols and systems that are robust and secure by design.

Here are some themes and domains that we currently work on:


## LLM-based Protocol Analaysis:

### CellularLint: A Systematic Approach to Identify Inconsistent Behavior in Cellular Network Specifications (Usenix Security 2024)

In recent years, there has been a growing focus on scrutinizing the security of cellular networks, often attributing security vulnerabilities to issues in the underlying protocol design descriptions. These protocol design specifications, typically extensive documents that are thousands of pages long, can harbor inaccuracies, underspecifications, implicit assumptions, and internal inconsistencies. 
![]({{ site.url }}{{ site.baseurl }}/images/respic/CellularLint.png){: style="width: 950px; float: left; margin: 5px 15px 0px 0px;"}
In light of the evolving landscape, we introduce CellularLint–a semi-automatic framework for inconsistency detection within the standards of 4G and 5G, capitalizing on a suite of natural language processing techniques. Our proposed method uses a revamped few-shot learning mechanism on domain-adapted large language models. Pre-trained on a vast corpus of cellular network protocols, this method enables CellularLint to simultaneously detect inconsistencies at various levels of semantics and practical use cases. In doing so, CellularLint significantly advances the automated analysis of protocol specifications in a scalable fashion. In our investigation, we focused on the Non-Access-Stratum (NAS) and the security specifications of 4G and 5G networks, ultimately uncovering 157 inconsistencies with 82.67% accuracy. After verification of these inconsistencies on 3 open-source implementations and 17 commercial devices, we confirm that they indeed have a substantial impact on design decisions, potentially leading to concerns related to privacy, integrity, availability, and interoperability.

### SPEC5G: A Dataset for 5G Cellular Network Protocol Analysis (AACL 2023)
5G is the 5th generation cellular network protocol. It is the state-of-the-art global wireless standard that enables an advanced kind of network designed to connect virtually everyone and everything with increased speed and reduced latency. Therefore, its development, analysis, and security are critical. However, all approaches to the 5G protocol development and security analysis, e.g., property extraction, protocol summarization, and semantic analysis of the protocol specifications and implementations are completely manual. 
![]({{ site.url }}{{ site.baseurl }}/images/respic/spec5g.png){: style="width: 950px; float: left; margin: 5px 15px 0px 0px;"}
To reduce such manual effort, in this paper, we curate SPEC5G the first-ever public 5G dataset for NLP research. The dataset contains 3,547,586 sentences with 134M words, from 13094 cellular network specifications and 13 online websites. By leveraging large-scale pre-trained language models that have achieved state-of-the-art results on NLP tasks, we use this dataset for security-related text classification and summarization. Security-related text classification can be used to extract relevant security-related properties for protocol testing. On the other hand, summarization can help developers and practitioners understand the high level of the protocol, which is itself a daunting task. Our results show the value of our 5G-centric dataset in 5G protocol analysis automation. We believe that SPEC5G will enable a new research direction into automatic analyses for the 5G cellular network protocol and numerous related downstream tasks. Our data and code are publicly available.

## Secure Protocol Design and Defense:

### TIMESAFE: Timing Interruption Monitoring and Security Assessment for Fronthaul Environments (arXiv 2024)

5G and beyond cellular systems embrace the disaggregation of Radio Access Network (RAN) components, exemplified by the evolution of the fronthual (FH) connection between cellular baseband and radio unit equipment. Crucially, synchronization over the FH is pivotal for reliable 5G services. In recent years, there has been a push to move these links to an Ethernet-based packet network topology, leveraging existing standards and ongoing research for Time-Sensitive Networking (TSN). However, TSN standards, such as Precision Time Protocol (PTP), focus on performance with little to no concern for security. This increases the exposure of the open FH to security risks. Attacks targeting synchronization mechanisms pose significant threats, potentially disrupting 5G networks and impairing connectivity.
![]({{ site.url }}{{ site.baseurl }}/images/respic/timesafe.png){: style="width: 450px; float: left; margin: 5px 15px 0px 0px;"}
In this paper, we demonstrate the impact of successful spoofing and replay attacks against PTP synchronization. We show how a spoofing attack is able to cause a production-ready O-RAN and 5G-compliant private cellular base station to catastrophically fail within 2 seconds of the attack, necessitating manual intervention to restore full network operations. To counter this, we design a Machine Learning (ML)-based monitoring solution capable of detecting various malicious attacks with over 97.5% accuracy.

**Protocol noncompliance checking**


**Systematic implementation analysis**

**Formal analysis of protocol standards**

**System Security Policies:**
Studying security policies of large-scale systems is crucial for identifying vulnerabilities and mitigating risks like data breaches and unauthorized access.
![]({{ site.url }}{{ site.baseurl }}/images/respic/security.jpg){: style="width: 250px; float: left; margin: 5px 15px 0px 0px;"}
A systematic analysis of security policies not only enhances the resilience of systems but also ensures compliance with regulations and industry-recommended practices.
Our research endeavors focus on conducting comprehensive security analyses of modern digital systems. We scrutinize the authentication, authorization, and access control mechanisms within systems involving millions of users —such as banking— to ensure the highest standard of protection for users and business assets. Our findings pave the way for the development of effective remedies, ensuring the integrity and trustworthiness of digital systems in various operational contexts.

**Quantum Security:**
![]({{ site.url }}{{ site.baseurl }}/images/respic/quantum-computing.png){: style="width: 250px; float: right; margin: 0px 10px"}
In the rapidly evolving landscape of quantum computing, the field of quantum security emerges as a crucial component to safeguard users’ communication. Central to these security measures are quantum key distribution and post-cryptographic technologies. Researchers are actively crafting new protocols in these domains, poised for deployment in the near future. While numerous research works and commercial products leveraging these technologies exist, practical implementations still face challenges in fully harnessing the potential of quantum mechanics under adversarial scenarios. Our laboratory adopts a pragmatic approach, delving into the comprehensive understanding of secure quantum communication in diverse scenarios. Our focus is on the development of efficient and end-to-end secure solutions grounded in the principles of key security principles proven to be secure over decades of research works. Through these endeavors, we aim to contribute to the robustness of quantum security in real-world applications.


**Mobile Networked Systems:** Next Generation (NG) Mobile Networks are designed to solve diverse application requirements (throughput, latency, safety, trust, and more) under one architecture. Our lab is mainly engaged in research and development of fundamental technologies behind NG mobile networks. Our aim is to enable novel network protocols for efficient, safe and secure mobile communications.

![]({{ site.url }}{{ site.baseurl }}/images/respic/CELL_SITES.jpeg){: style="width: 70%; float: center; margin: 10px"}


<!-- ### ... and more. -->

<!-- Our overarching goal is to explore and understand new quantum states of electronic matter on the atomic scale. To do so, we use and develop novel spectroscopic-imaging scanning tunneling microscopy (SI-STM) tools to visualize the relevant quantum mechanical degrees of freedom.

Our goal is to build instruments and develop techniques that enable us to address the questions we find most interesting. This is possible thanks also to Milan's broad background with different research themes and technologies: he learned his trade in [Seamus Davis’ SI-STM lab](http://davisgroup.lassp.cornell.edu/) and with [Felix Baumberger](http://dpmc.unige.ch/gr_baumberger/index.html), and later moved as an [ETH fellow](http://www.ethfellows.ethz.ch/) to [Andreas Wallraff’s qudev lab](http://www.qudev.ethz.ch/) where he investigated coupled cavity arrays in circuit QED. We further have group members with different background and interests, working together on physics and instrumentation.


**Scanning tunneling noise spectroscopy (STNS).** We have developed a novel cryogenic MHz amplifier that allows us to measure not only the average tunneling current, but also its fluctuation! This has many applications: one can detect the fluctuations of the electronic states, peculiar tunneling processes, and shot noise. We have used this instrument to discover charge trapping in the insulating layer of the cuprates, connected to the c-axis mystery, and to measure the doubling of the charge due to Andreev processes to the superfluid in a lead sample.


**Mott physics and high-temperature superconductivity.** Questions of interest include: (i), How does the Mott state collapse upon doping and how is this related to the complex phase diagram of high-temperature superconductors? (ii), What is the strange metal phase seen in correlated electron systems? Is this an exotic long-range entangled state? What is the mechanism of dissipation in that state? (iii), Why is the transition temperature in high-temperature superconductors so high? We have worked on iridates, rhodates, and cuprates.

**Nanofabricated "Smart Tips"**.
![]({{ site.url }}{{ site.baseurl }}/images/respic/SmartTip.png){: style="width: 250px; float: left; margin: 0px  10px"}
One of the  projects back from my job-proposal is to develop nanofabricated STM tips. The idea behind these “smart tips” is to use the technologies that were developed over decades in nanofabrication and make them available for scanning probe by using a nano-device instead of the traditional STM tungsten tip. One gains the flexibility of using different functionalities that are known from the fields of nanofabrication and mesoscopic physics. We are collaborating with the group Simon Groeblacher at TU Delft to realize this concept, benefitting from their unparalleled micro/nano fabrication know how.  A prototype of a smart tip is shown to the left. See publications in Microsyst Nanoeng, Nanotechnology, and PRB.

**Josephson STM.** Josephson STM has the ability to gain insight into spatial variations of the order parameter, or superfluid density. We have managed to, for the first time, use JSTM with atomic resolution on a quantum material.
We have used atomic-resolution Josephson scanning tunneling microscopy to reveal a strongly inhomogeneous superfluid in the iron-based superconductor FeTe0.55Se0.45. The results and their implications are published in Nature.

We also detected and investigated a quite particular YSR state in the same material.

**Ultra-stable SI-STM instrument.**  ![]({{ site.url }}{{ site.baseurl }}/images/respic/STMHead.png){: style="width: 250px; float: right; margin: 0px 10px"}
For SI-STM, having the most stable STM head is key. We have used finite element simulations, good choices in material science, and craftsmanship to build the most stable STM head in the world, to our knowledge. See publication in RSI.


**Strange Metals.** The strange metal phase might be the most mysterious phase of high-temperature superconductors. Here, the electrical resistivity grows linearly with temperature T in large areas of the phase diagram, with a mean free path that diminishes to a fraction of the interatomic distance. T-linear resistivity is often associated with quantum critical points and marginal-Fermi-liquid physics. In strange metals, the mystery seems to go even further: we deal with something that looks like a quantum critical phase over an extended range of the phase diagram instead of cumulating in a point. There exists no consistent theory for strange metals, leading to more adventurous new approaches including the holographic theories that use insights from gravity to explain strange metals (a recent textbook on this was written by our colleagues at Leiden University, Schalm and Zaanen).
We are part of the 'Strange Metal consortium NL' that includes the groups of Hussey, Golden, van Heumen, Zaanen, Schalm, Stoof and Vandoren. 

**Magnetic fluctuations and electron spin resonance.**
![]({{ site.url }}{{ site.baseurl }}/images/respic/SpinFluc.png){: style="width: 70%; float: center; margin: 10px"}

**Twisted bilayer graphene and other material with super-periodicities.**
We have proposed that artificial super-periodicities can lead to improved superconductivity, both because of increased density of states and because of phase space arguments (see image from our SciPost publication below). Perhaps for different reasons, twisted bilayer graphene has been shown to superconduct! We are investigate this material with the groups of Efetov, Baumberger, and van der Molen.

![]({{ site.url }}{{ site.baseurl }}/images/respic/SciPost.png){: style="width: 70%; float: center; margin: 0px"} -->