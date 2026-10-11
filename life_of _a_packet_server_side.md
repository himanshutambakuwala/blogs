# Life of a packet from NIC to Application and Back

As network engineer, I spend a lot of time working on the network elements in the system. 
The designing, developing and debugging of network issues ( including proving it's not 
network's fault :-) ) has helped building and growing skills in network domain. But, the 
fact is networking does not start or stop at network elements.

The network packet, as we all know, originates and terminates from/to an application, like 
a browser, on a laptop or a server (commonly referred as compute). A server is not 
merely a passive recipient of network data; it is a complex packet-processing computer 
where a single inbound or outbound flow crosses hardware PHY/MAC silicon, PCIe buses, DMA 
memory controllers, top/bottom-half kernel interrupt architectures, Netfilter hooks, protocol 
state engines, and application socket queues. Understanding the precise journey of a packet 
across these subsystems is essential for diagnosing non-obvious performance degradation, 
host-level packet drops, CPU starvation, and mysterious latency spikes.
