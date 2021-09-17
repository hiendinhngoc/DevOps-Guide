1. Intro to network devices
  - **Layer 1 devices**:
    - The Open Systems Interconnection (OSI) model was developed as a way to help disparate computing systems communicate with each other.
    - OSI reference model has 7 layers:
      - Layer1 - Physical
      - Layer2 - Data Link
      - Layer3 - Network
      - Layer4 - Transpot
      - Layer5 - Session
      - Layer6 - Presentation
      - Layer7 - Application
    - Analog modem(modulator/demodulator)
      - was developed to take the digital signal coming from a digital node and convert it to an analog signal (modulating the signal) to be placed on the wire. In return, it would accept an analog signal from the wire and convert it (demodulating the signal) to a digital signal that the node could understand.
      - modems provide for a single connection to a network
    - Hub
      - A hub functions as a concentrator/repeater in that it doesn't care where the signal comes from or where it is going. It takes the electrical signal that arrives on a port and replicates that signal out all of the othere ports.
      - It may have just a few ports, or many ports(not very common in morden networking)
  - **Layer 2 devices**
    - Switch:
      - A switch utilizes an application-specific integrated circuit (ASIC) chip. The chip has specific programing that allows the switch to learnwhen a device is on the network and which ports it is connected to via that device's Layer 2 MAC address.
      - A switch may have just a few ports or many ports
      - A switch can be very simple, or it can be highly complex and programmable.
      - A switch will only communicates with the local network devices.
    - Wireless access point(WAP)
      - A WAP is a specific type of network bridge that connects (bridges) wireless network segments with wired network segments. The most common type of WAP bridges 802.11 wireless network segments with 802.3 Ethernet network segments.
      - A WAP will only communicates with local network devices.
  - **Layer 3 devices**
    - Multilayer switch (MLS)
      - An MLS provides normal Layer 2 network switching services, but it will also provide Layer 3 or highter OSI model services.
      - The most common MLS is a Layer 3 switch.
      - An MLS is a highly programmable and complex network device.
      - An MLS may have just a few ports or many ports.
    - Router
      - A router is the most common network device for connecting different networks together utilizing the OSI model's Layer 3 logical network information.
      - The router uses software programming for decision making as compared to the switch's use of an ASIC chip. The router uses this programing to keep track of differenct networks and what it considers to be the best possible route to reach those networks.
      - A router can communicate with both local and no-local network devices.
  - **Security Devices**
    - Firewall
      - A firewall can be placed on routers or hosts(software based) or can be its own device.
      - It runctions at multiple layers of the OSI model(specifically at layers 2,3,4 and 7)
      - It blocks packets from entering or leaving the network:
        - Via stateless inspecion: the firewall will examine every packet against a set of rules. Once the packet matches a rule, the rule is enforced, and the specified action is taken.
        - Via statefull inspection: the firewall will only examine the state of the connection between networks. Spefically, when a connection is made from an internal network to an external network, the firewall will not examine any packets returning from the external connection. As a general rule, external connections are not allowed to be initiated with the internal network.
      - It is the first line of defense in protecting the internal network from outside threats(consider it the police force of the network)
    - Intrusion detection system (IDS)
      - An IDS is a passive system designed to identify when a network breach or attack against the network is occuring(Usually designed to inform a network administrator when a breach or attack has occcurred through log files, SMS, and/or an email notification)
      - An IDS cannot prevent or stop a breach or attack on its own.
      - It receives a copy of all traffic and evaluates it against a set of standards.
        - Signature based: evaluates network traffic for known malware or attack signatures.
        - Anomaly based: evaluates network traffic for suspicious changes.
        - Policy based: evaluates network traffic against a specific declared security policy.
      - May be deployed at the host level(Host-base intrusion detection system (HIDS))
    - Intrusion prevention system (IPS)
      - An IPS is an active system designed stop a breach or attack from succeeding in damaging the network
        - Usually designed to perform an action or set of actions to stop the malicious activity.
        - will inform a network administrator through the use of log files, SMS, and/or email notification.
      - All traffic on the network segment flows throught the IPS to either enter or leave the segment(Like the IDS, all traffic is evaluated against the set of standards)
      - The best placement on the network is between a router(with a firewall) and the destination network segment
      - It is programmed to make an active reponse to the situation
        - Block the offending IP address
        - Close down the vulerable interface
        - Terminate the network session
        - Redirect the attack
        - Plus more
    - Virtual private network(VPN)
      - A VPN concentrator will allow for many more secure VPN connections to a network.
  - **Optimization and performance devices**
    - Load balancer
      - A load balancer may also be called a content switch or content filter
      - A network applicance that is used to load balnce between multiple hosts that contain the same data-spreading out the workload for greater efficiency(Commonly used to distribute the requests (workload) to a server farm among the various servers, helping to ensure that no single server gets overloaded)
    - Proxy server
      - A proxy server is an appliance that requests resources on befalf of client machines
      - It is often used to retrieve resources from outside untrustred networks on befalf of the requesting client
      - It hides and protectes the requesting client
      - It can also be utilized to filter allowed content
      - It can increase network perormance by caching commonly requested Web pages.
2. Networking services and applications
3. DHCP in the network
4. Introducing Network Address Tranlation(NAT)
5. WAN technologies
6. Network cabling
7. Network topologies
8. Network infrastructure implementations
9. Introduction to IPv4
10. Introduction to IPv6
11. Special IP networking concepts
12. Introduction to routing concepts
13. Introduction to routing protocols
14. Basic Elements of Unified Comunicaitons
15. Visualization technologies
16. Storage Area Networks(SAT)
17. Basic Cloud Concepts
18. Implementing a basic network
19. Analyzing monitoring reports
20. Network monitoring
21. Supporting configuration management
22. The impotance of network segmentation
23. Applying patches and updates
24. Configuring switches
25. Wireless LAN infrastructure
26. Risk and security related concepts
27. Common network vulnerabilities
28. Common network threats
29. Network hardening techniques
30. Phisical network security control
31. Firewall basics
32. Network Access Control
33. Basic forensic concepts
34. Network troubleshooting methodology
35. Troubleshooting connectivity with utilities
36. Troubleshooting wireles networks
37. Troubleshooting cooper wire networks
38. Troubleshooting fiber cable networks
39. Troubleshooting common network issues
40. Common WAN components and issues
41. The OSI networking reference model
42. The transport layer plus ICMP
43. Basic network concepts
44. Introduction to wireless network standards
45. Introduction to wire network stardards
46. Security policies and other documents
47. Introduction to safty practice
48. Rack and Power management
49. Cable management
50. Basics of change management
51. Common networking protocols
