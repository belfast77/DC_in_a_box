# DC_in_a_box

Im building a portable datacenter in a box as I always wanted an Canonical Orange Box* but couldn't afford the £8k price tag.

### Whats inside the Box
![alt text](https://pbs.twimg.com/media/EQC15pWWoAAClq5?format=jpg&name=small "DC in a Box")
![alt text](https://pbs.twimg.com/media/EQC16YZXUAQu6lQ?format=jpg&name=small "DC in a Box")
![alt text](https://pbs.twimg.com/media/ETJJsCOXsAUMb92?format=jpg&name=small "DC in a Box")
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/BoxUpgrade2.PNG)
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/BoxUpgrade1.PNG)
### Hardware Layout
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/Hardware.png)
### vCenter 
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/BoxUpgrade3.PNG)
### VMs
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/DC_IN_A_BOX.PNG)


## Components
Keter 221474 Technicians Tool Box
https://www.amazon.co.uk/gp/product/B00PC5EO28/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

NETGEAR GS308 8-Port Gigabit Ethernet Network Switch
https://www.amazon.co.uk/gp/product/B07PWHGQSS/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

2 X Intel SKULL CANYON i7 Gaming NUC NUC6I7KYK Barebone Kit
https://www.amazon.co.uk/gp/product/B01FWIUZ7W/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

4 X Samsung MZ-V7E500BW 970 EVO 500 GB V-NAND M.2 PCI Express Solid State Drive 
https://www.amazon.co.uk/gp/product/B07CGGP7SV/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

2 X Crucial CT2K16G4SFD8266 32 GB Kit (16 GB x2) (DDR4, 2666 MT/s, PC4-21300, Dual Rank x8, SODIMM, 260-Pin)
https://www.amazon.co.uk/gp/product/B071H38422/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

GL.iNet GL-AR300M (Shadow) Mini VPN Travel Router
https://www.amazon.co.uk/gp/css/summary/edit.html/ref=dp_iou_view_this_order?ie=UTF8&orderID=026-8293968-0693919

```
Servers : 2 x Intel NUC ESXi Hosts
---------------------------------
4 x Samsung 970 EVO Plus 500 GB PCIe NVMe M.2 (SSD)| £102.42 = £409.68
2 x Crucial CT2K32G4SFD8266 64 GB Kit (32 GB x 2) (DDR4, 2666 MHz, SODIMM) Memory | £279.24 = £558.48
2 x Intel BOXNUC6i7KYK3 i7-6770HQ NUC Kit | £556.87 = £1,113.74
1 x Keter 221474 Technicians Tool Box £32.07 
1 x NETGEAR GS308 8-Port Desktop Gigabit Ethernet Switch | £19.49
1 x GL.iNet GL-AR300M (Shadow) Mini VPN Travel Router | £35.90

Total = £2,169.36

Servers : ThinkCentre ESXi Hosts
------
Lenovo ThinkCentre M90q Tiny Core i9-10900T  | £1089.96
Crucial RAM CT2K32G4SFD8266 64GB Kit (2x32GB) DDR4 | £266.39
1 x Crucial P5 2 TB CT2000P5SSD8 PCIe NVMe M.2  | £156.99

Total = £1,513.34

Pi Cluster
---------
3 x Official Raspberry Pi 4 USB-C PSU | £11.98 = £35.94
3 x RPI4-MODBP-4GB RASPBERRY PI 4 MODEL B, 4GB | £43.31 = £155.88
3 x TSRASPI10-16G.. MICROSD CARD, RASPBERRY PI BOARD | £25.65 = £76.96

Total = £309.80

Laptop
------
Lenovo ThinkPad P53 Core i7-9750H, 48GB Ram, 1TB NVMe M.2 SSD, 15.6 Screen, Quadro T1000 4GB, Laptop | £1299.96 
2 x Crucial CT2K16G4SFD8266 32 GB Kit (16 GB x 2) (DDR4, 2666 MT/s, SODIMM) |	£129.59 = £259.18

Total = £1,559.14

Total = £5,551.64
```
## Software
Red Hat OpenShift 4.9

Ansible Automation Platform 2.2

GitLab Community Edition 14.2.0

Redhat Satellite 6.10

VMware vSphere Hypervisor 6.7

VMware vCenter Server Appliance 6.7.0U1

VMware vRealize Log Insight 4.7.0 - Virtual Appliance via vCenter Server

Ansible AWX - Release 9.1.0

Puppet Enterprise - 2018.1

Katello - Version 1.21.0-RC5

## Upgrade

Upgraded the portable Lab with a Lenovo ThinkCentre M90q Tiny Core i9-10900T 64GB DDR4 & 1 TB M.2 NVMe. It's enough to run an installer-provisioned infrastructure cluster of #OpenShift on #vSphere7.

### New Layout

![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/BoxUpgrade1.PNG)


### Lenovo ThinkCentre M90q Tiny Core i9-10900T
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/BoxUpgrade2.PNG)

### CPU & Memory
![alt text](https://raw.githubusercontent.com/belfast77/DC_in_a_box/master/images/BoxUpgrade3.PNG)


## References
* https://www.zdnet.com/article/canonicals-cloud-in-a-box-the-ubuntu-orange-box/
