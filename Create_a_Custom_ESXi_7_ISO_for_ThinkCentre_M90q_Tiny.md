Create a Custom ESXi 7 ISO for a Lenovo ThinkCentre M90q Tiny Core i9-10900T




```
PS E:\ISOs\esxi>  Add-EsxSoftwareDepot ".\VMware-ESXi-7.0U2a-17867351-depot.zip"

Depot Url
---------
zip:E:\ISOs\esxi\VMware-ESXi-7.0U2a-17867351-depot.zip?index.xml


PS E:\ISOs\esxi> Add-EsxSoftwareDepot ".\Net-Community-Driver_1.2.2.0-1vmw.700.1.0.15843807_18835109.zip"

Depot Url
---------
zip:E:\ISOs\esxi\Net-Community-Driver_1.2.2.0-1vmw.700.1.0.15843807_18835109.zip?index.xml


PS E:\ISOs\esxi> Get-EsxImageProfile

Name                           Vendor          Last Modified   Acceptance Level
----                           ------          -------------   ----------------
ESXi-6.7.0-20211104001-stan... VMware, Inc.    26/10/2021 0... PartnerSupported
ESXi-6.7.0-20211104001-usbnic  cowlan.co.uk    11/12/2021 1... PartnerSupported
ESXi-7.0U2a-17867351-no-tools  VMware, Inc.    09/04/2021 0... PartnerSupported
ESXi-7.0U2a-17867351-standard  VMware, Inc.    29/04/2021 0... PartnerSupported


PS E:\ISOs\esxi> New-EsxImageProfile -CloneProfile "ESXi-7.0U2a-17867351-standard" -name "ESXi-ThinkCentre"

cmdlet New-EsxImageProfile at command pipeline position 1
Supply values for the following parameters:
(Type !? for Help.)
Vendor: Cowlan.co.uk

Name                           Vendor          Last Modified   Acceptance Level
----                           ------          -------------   ----------------
ESXi-ThinkCentre               Cowlan.co.uk    29/04/2021 0... PartnerSupported


PS E:\ISOs\esxi> Add-EsxSoftwarePackage -ImageProfile "ESXi-ThinkCentre" -SoftwarePackage "net-community"

Name                           Vendor          Last Modified   Acceptance Level
----                           ------          -------------   ----------------
ESXi-ThinkCentre               Cowlan.co.uk    11/12/2021 1... PartnerSupported


PS E:\ISOs\esxi> Export-ESXImageProfile -ImageProfile "ESXi-ThinkCentre" -ExportToISO -filepath ESXi-7.0U2a-17867351-ThinkCentre.iso

```
