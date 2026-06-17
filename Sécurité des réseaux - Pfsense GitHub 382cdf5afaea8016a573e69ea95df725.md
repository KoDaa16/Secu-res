# Sécurité des réseaux - Pfsense GitHub

![image.png](image.png)

```bash
Site 1                                        Site 2
-----------                                   -----------
Pfsense1 :                                    Pfsense 2 :
WAN : DHCP                                    WAN : DHCP
LAN : 172.16.0.1/25                           LAN : 172.18.0.1/25
    |                                             |
    | 172.16.0.0/25                               |
    |                                             | 172.18.0.0/25
Routeur Linux                                     |
Vers PF1 : 172.16.0.126                           |
vers client : 172.16.0.254                    Client Linux 2
    |                                         IP : 172.18.0.10
    |172.16.0.128/25                          GW : 172.18.0.1
    |
Client Linux
IP : 172.16.0.129
GW : 172.16.0.254
```