# Supported Linux Operating Systems for VPS

> **Minimum system requirements for VPS:** \
> Operating System - Linux, suitable for Ubuntu 22.04 or Debian 11. \
> Supported processor architecture - x86-64.\
> Virtualization - KVM. \
> Random Access Memory (RAM) - recommended 2 GB, but not less than 1 GB. \
> Pre-installed software and control panel are not required.

Below are other Linux OS options supported by AmneziaVPN.
KVM is the recommended virtualization type. WireGuard and AmneziaWG protocols are not supported with OpenVZ virtualization.

### Debian

|               | Debian 12 | Debian 11 | Debian 10 |  
|---------------|:---------:|:---------:|:---------:|
| IKEv2         |    ✔*     |    ✔*     |    ✔*     |  
| AmneziaWG     |     ✔     |     ✔     |     ✔     |  
| WireGuard     |     ✔     |     ✔     |    —*     |  
| OpenVPN       |     ✔     |     ✔     |     ✔     | 
| OpenVPN+Cloak |     ✔     |     ✔     |     ✔     |
| ShadowSocks   |     ✔     |     ✔     |     ✔     |

&nbsp;

### Ubuntu

|               | Ubuntu 22.04 | Ubuntu 20.04  | Ubuntu 18.04  | Ubuntu 16.04 |
|---------------|:------------:|:-------------:|:-------------:|:------------:|
| IKEv2         |     ✔*       |      ✔*       |      ✔*       |     ✔*       |
| AmneziaW      |      ✔       |       ✔       |       ✔       |      ✔       |
| WireGuard     |      ✔       |       ✔       |      —*       |      —       |
| OpenVPN       |      ✔       |       ✔       |       ✔       |      ✔       |
| OpenVPN+Cloak |      ✔       |       ✔       |       ✔       |      ✔       |
| ShadowSocks   |      ✔       |       ✔       |       ✔       |      ✔       |

&nbsp;

### Fedora

|               | Fedora 26-29 | Fedora 30 |  
|---------------|:------------:|:---------:|
| IKEv2         |     ✔*       |    ✔*     |  
| AmneziaWG     |      ✔       |     ✔     |  
| WireGuard     |      —       |     ✔     |  
| OpenVPN       |      ✔       |     ✔     | 
| OpenVPN+Cloak |      ✔       |     ✔     |
| ShadowSocks   |      ✔       |     ✔     |

&nbsp;

### CentOS

|               | CentOS 7 |  
|---------------|:--------:|
| IKEv2         |   ✔*     |  
| AmneziaWG     |    ✔     |  
| WireGuard     |    —     |  
| OpenVPN       |    ✔     | 
| OpenVPN+Cloak |    ✔     |
| ShadowSocks   |    ✔     |

&nbsp;

✔* - For IPSec (IKEv2) currently, the last working version is AmneziaVPN 2.0.10. After a server reboot, container reinstallation is required. In the case of a downgrade update to a version earlier than 2.1.2, make a backup of AmneziaVPN settings on the device beforehand.

—* - For servers with Ubuntu 18.04 and Debian 10, there is an option to update the Linux kernel from the 4th to the 5th version to support the WireGuard protocol.

— - Protocol not supported.

> For any OS on servers other than Ubuntu 22/20, Debian 12/11, it is strongly recommended to perform a pre-update of the OS with a subsequent server reboot.

### Update Ubuntu / Debian
~~~
sudo apt update && sudo apt upgrade
~~~
Acceptable for root:
~~~
apt update && apt upgrade
~~~
Reboot:
~~~
sudo reboot
~~~
Acceptable for root:
~~~
reboot
~~~
### Update CentOS 7
~~~
sudo yum check-update && sudo yum update
~~~
Acceptable for root:
~~~  
yum check-update && yum update
~~~
Reboot:
~~~  
sudo reboot
~~~
Acceptable for root:
~~~  
reboot
~~~
### Update Fedora 26-30
~~~
sudo dnf check-update && sudo dnf update
~~~
Acceptable for root:
~~~
dnf check-update && dnf update
~~~
Reboot:
~~~
sudo reboot
~~~
Acceptable for root:
~~~
reboot
~~~
[about-int-link]: /about





















