要點整理
- 網路協議套組 (Internet Protocol Suite - IPS)是網路的基礎通訊架構，常通稱TCP/IP協定套組，簡稱TCP/IP
- TCP/IP提供點對點的連結機制，規範資料如何封裝、定址、傳輸、路由以及在目的地如何接收的標準
- TCP/IP最早發源於美國國防部(DoD)的ARPA網專案，因此也稱作==Dod 模型== (Dod Model)
- TCP/IP採取協定堆疊的方式，將通訊過程抽象化為四層，各分層依功能實作不同通訊協定

---

DoD模型
- 應用層 (Application Layer)

>DHCP，DNS，FTP，HTTP，HTTPS，POP，SMTP，SSH，Telnet，SNMP
- 傳輸層 (Transport Layer)

>TCP，UDP，TLS/SSL，DCCP
- 網路層 (Internet Layer)

>IP (IPv4，IPv6)，ICMP，ICMPv6，IGMP，OSPF，IPsec，RIP
- 連結層 / 網路存取層 (Link Layer / Network Access Layer)

>ARP，PPP，Tunnels (L2TP)，MAC (Ethernet，FDDI，DSL，ISDN)