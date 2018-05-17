## TCP, QUIC, MPTCP and MP-QUIC  
### Arguments
- File sizes: 10KB, 100KB, 500KB, 1MB, 10MB, 50MB, 100MB.  
- Link characteristics: bandwidth, delay, jitter, pakcet loss.  
### Tasks  
1. TCP vs QUIC  
   - Over a single link.  
   - Three types of link: Good link, Not so good link and vary bad link.  
   - Based on WiFi and LTE respectively. So six lines in total.  
   - QUIC-Go.  
2. MPTCP vs MPQUIC  
3. MPTCP vs MPQUIC with Link Broken  
4. MPTCP vs MPQUIC with Recovering Link  

## Notes  
- RTT: 
In telecommunications, the round-trip delay time (RTD) or round-trip time (RTT) is the length of time it takes for a signal to be sent plus the length of time it takes for an acknowledgement of that signal to be received.  
- UDP: User Datagram Protocol. With UDP, computer applications can send messages to other hosts on an Internet Protocol network. Prior communications are not required in order to set up communication channels or data paths. UDP has no handshaking dialogues, guarantee of delivery, ordering or duplicate protection, so it is unreliable.  
- QUIC: Quick UDP Internet Connections. QUIC supports a set of multiplexed connections between two endpoints over UDP and was designed to provide security protection equivalent to TLS/SSL, along with reduced connection and transport latency, and bandwidth estimation in each direction to avoid congestion.  
- TCP vs QUIC:  
   - Connection handshake: TCP required a 3-way handshake to establish a connection, and, on top of that, you also need to negotiate the TLS connection. QUIC is built on top of UDP so it requires 1 packet to establish the connection, including TLS. Actually, if the client and the server have spoken in the past, then we are talking about a zero-handshake connection ¨C that happens 75% the time.  
   - Multiplexing: the communication between the client and the server is multiplexed and this overcomes the head-of-line blocking issues that are common with TCP connections.