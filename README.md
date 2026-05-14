GNS3_LAB_001

Author: Juliet Karanja

This project is about two VPCs connected to each other. Thy share the same network, connected by ethernet cables, 
VPC 1 at 192.168.1.2/24
VPC 2 at 192.168.1.1/24
 Assigned IPs with command for both VPC 1 & 2

PC2> ip 192.168.1.1/24
Checking for duplicate address...
PC1 : 192.168.1.1 255.255.255.0
 
PC1> ip 192.168.1.2/24
Checking for duplicate address...
PC1 : 192.168.1.2 255.255.255.0

Tested connection from VPC 2 to VPC 1 while using wireshark to capture traffic.

PC2> ping 192.168.1.2/24
84 bytes from 192.168.1.2 icmp_seq=1 ttl=64 time=2.428 ms
84 bytes from 192.168.1.2 icmp_seq=2 ttl=64 time=1.765 ms
84 bytes from 192.168.1.2 icmp_seq=3 ttl=64 time=2.051 ms
84 bytes from 192.168.1.2 icmp_seq=4 ttl=64 time=2.201 ms
84 bytes from 192.168.1.2 icmp_seq=5 ttl=64 time=1.924 ms

Here is the output and my understanding of it

