# Task3.4

## DHCP, DNS, NAT settings

<details>
  <summary>picture</summary>

  ![3.4](assets/3.4.png)

</details>

- I configured the DHCP Pool by specifying the starting address 10.89.23.10 and the Default Gateway address - the GE0 / 0 Router ISP1 interface address - 10.89.23.1.

- Checked the serviceability of the service by setting in the settings Client 1 and Client 2 DHCP:
  - ![dhcp](assets/3.4.3.dhcp1.png)
  - ![dhcp](assets/3.4.3.dhcp2.png)

- Configured DHCP on the Home Router and tested on Client 3:
  - ![dhcp](assets/3.4.4.dhcp3.png)

- I made dns record in the DNS server settings for web server1 and web server2 and turned on the DNS service.
  - ![dns](assets/3.4.6.dnsrecord.png)

- Added DNS server address `12.23.89.150` to DHCP servers settings and updated client settings.
- I checked this by pinging to the domain name
  - ![ping](assets/3.4.8.ping1.png)
  - ![ping](assets/3.4.8.ping2.png)

## Optional. Configure Port Forwarding on the Home Router

- Added Home server to the Home Office network and assigned it a static address: `192.168.0.100`

- Set up Port Forwarding on Home Router.

- Added an entry for DNS Server for Home Server:
  - name: `domain3.com`
  - type: `A-record`
  - address: `33.12.89.194`

- Checked in Desktop/Web Browser:
  - ![homeserv](assets/3.4.13.homeserv.png)

## File pkt

- [task3.4.pkt](task3.4.pkt)
