# Task3.3

## Routing settings

<details>
  <summary>picture</summary>

  ![3.3](assets/3.3.png)

</details>

- Configured routing tables on ISP1, ISP2, and ISP3 routers:
  - added route on ISP1:
    - net `12.23.89.0/24`, next hop `33.12.89.66`
    - net `33.12.89.192/26`, next hop `33.12.89.2`
  - added route on ISP2:
    - net `10.89.23.0/24`, next hop `33.12.89.1`
    - net `12.23.89.0/24`, next hop `33.12.89.130`
  - added route on ISP3:
    - net `10.89.23.0/24`, next hop `33.12.89.65`
    - net `33.12.89.192/26`, next hop `33.12.89.129`

- Checked the connection between the computers with `ping` command and the packet route with `tracert`:
  - ![ping](assets/3.3.3.ping1.png)
  - ![ping](assets/3.3.3.ping2.png)
  - ![ping](assets/3.3.3.ping3.png)

## Optional. Rip

- On routers ISP1, ISP2 and ISP3 I configured the RIP protocol, for which I specified a list of directly connected networks in class format:
  - on ISP1: net `10.0.0.0`, `33.0.0.0`
  - ![rip.isp1](assets/3.3.5.rip.isp1.png)
  - on ISP2: net `33.0.0.0`
  - ![rip.isp2](assets/3.3.5.rip.isp2.png)
  - on ISP3: net `12.0.0.0`, `33.0.0.0`
  - ![rip.isp3](assets/3.3.5.rip.isp3.png)

- Checked the connection between the computers with `ping` command and the packet route with `tracert`:
  - ![ping](assets/3.3.6.ping1.png)
  - ![ping](assets/3.3.6.ping2.png)
  - ![ping](assets/3.3.6.ping3.png)

## File pkt

- [task3.3.pkt](task3.3.pkt)
- [task3.3rip.pkt](task3.3rip.pkt)
