#### Python3: Network Packet Capture

This Python project is based on the packet sniffer tutorial by thenewboston.

https://www.youtube.com/watch?v=WGJC5vT5YJo

Our packet sniffer captures ethernet frames and displays the destination and source MAC addresses and the protocol being used.  Additionally, the packet inspector captures IP version, header length, protocol, time-to-live and source and destination IPs.  TCP and UDP segments capture the source and destination ports and flags.  Finally, the hex represenation of the data.

Usage:

```
$ time python3 packet_sniffer.py
```

Output:

```
Ethernet Frame: 
	 - Destination: 00:15:5D:00:24:0E, Source: AC:72:89:93:47:C0, Protocol: 8
	 - IPv4 Packet: 
		 - Version: 4, Header Length: 20, TTL: 64
		 - Protocol: 6, Source: 198.18.0.37, Target: 173.194.219.18
	 - TCP Segment:
		 - Source Port: 53272, Destination Port: 443
		 - Sequence: 148974719, Acknowledgment: 3970718633
		 - Flags:
			 - URG: 0, ACK: 1, PSH: 0, RST: 0, SYN: 0, FIN: 0
		 - Data:
			 \xd0\x18\x01\xbb\x08\xe1\x2c\x7f\xec\xac\x5b\xa9\x80\x10\x00\xed\xc3\x58\x00
			 \x00\x01\x01\x08\x0a\x00\x67\x1e\xc0\x23\xcb\xd0\xee
```

You must use python3 to run this program.


