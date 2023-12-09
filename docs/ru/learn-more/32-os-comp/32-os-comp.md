
# Поддерживаемые операционные системы Linux для VPS   

# 
 
> Операционная система должна быть Linux с поддержкой виртуализации с KVM.

 >Рекомендуемая к установке OS Debian 11, Ubuntu 22.04. 

Ниже представлены другие варианты операционных систем поддерживаемые Amnezia.

### Debian

|               | Debian 12 | Debian 11 | Debian 10 |  
|---------------|:---------:|:---------:|:---------:|
| IKEv2         |    ✔*     |    ✔*     |    ✔*     |  
| AmneziaWG     |     ✔     |     ✔     |     ✔     |  
| WireGuard     |     ✔     |     ✔     |     —     |  
| OpenVPN       |     ✔     |     ✔     |     ✔     | 
| OpenVPN+Cloak |     ✔     |     ✔     |     ✔     |
| ShadowSocks   |     ✔     |     ✔     |     ✔     |

&nbsp;

### Ubuntu

|               | Ubuntu 22.04 | Ubuntu 20.04  | Ubuntu 18.04  | Ubuntu 16.04 |
|---------------|:------------:|:-------------:|:-------------:|:------------:|
| IKEv2         |      ✔*      |      ✔*       |      ✔*       |      ✔*      |
| AmneziaW      |      ✔       |       ✔       |       ✔       |      ✔       |
| WireGuard     |      ✔       |       ✔       |       —       |      —       |
| OpenVPN       |      ✔       |       ✔       |       ✔       |      ✔       |
| OpenVPN+Cloak |      ✔       |       ✔       |       ✔       |      ✔       |
| ShadowSocks   |      ✔       |       ✔       |       ✔       |      ✔       |

&nbsp;



### Fedora

|               | Fedora 26-29 | Fedora 30 |  
|---------------|:------------:|:---------:|
| IKEv2         |      ✔*      |    ✔*     |  
| AmneziaWG     |      ✔       |     ✔     |  
| WireGuard     |      —       |     ✔     |  
| OpenVPN       |      ✔       |     ✔     | 
| OpenVPN+Cloak |      ✔       |     ✔     |
| ShadowSocks   |      ✔       |     ✔     |

&nbsp;

### CentOS

|               | CentOS 7 |  
|---------------|:--------:|
| IKEv2         |    ✔*    |  
| AmneziaWG     |    ✔     |  
| WireGuard     |    —     |  
| OpenVPN       |    ✔     | 
| OpenVPN+Cloak |    ✔     |
| ShadowSocks   |    ✔     |

&nbsp;

(KVM)* рекомендуемый тип виртуализации. При виртуализации OpenVZ, работа WireGuard и AmneziaWG не поддерживается. 

✔* - IPSec (IKEv2)* в настоящий момент, AmneziaVPN 2.0.10 последняя рабочая версия. После перезагрузки сервера, требуется переустановка контейнера. 

Для Ubuntu 18.04 и Debain 10, возможно обновление ядра Linux по backport.

На всех ОС, кроме Ubuntu 22 / 20, Debian 12 / 11, рекомендуется выполнить предварительное обновление ОС, с последующей перезагрузкой сервера.

### Обновление Ubuntu / Debian
~~~
sudo apt update && sudo apt upgrade
~~~
Вариант для root
~~~
apt update && apt upgrade
~~~
Перезагрузка Ubuntu / Debian 
~~~
sudo reboot
~~~
Вариант для root 
~~~
reboot
~~~
### Обновление CentOS 7
~~~
sudo yum check-update && sudo yum update
~~~

Вариант для root 
~~~  
yum check-update && yum update**
~~~
 Перезагрузка CentOS 7
~~~  
sudo reboot
~~~  

Вариант для root
~~~  
reboot
~~~
### Обновление Fedora 26-30
~~~
sudo dnf check-update && sudo dnf update**
~~~
Вариант для root  

~~~
dnf check-update && dnf update
~~~
### Перезагрузка Fedora 26-30
~~~
sudo reboot
~~~
Вариант для root
~~~
reboot
~~~
[about-int-link]: /about
[FAQ]: ../faq 
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]:  ../instructions
[AmneziaWG]: https://github.com/amnezia-vpn/amnezia-wg
[Для Android]: https://github.com/amnezia-vpn/awg-android
[Для Windows]: https://github.com/amnezia-vpn/awg-windows
[Для MacOS и IOS]: https://github.com/amnezia-vpn/awg-apple
[Для Wireguard]: https://github.com/amnezia-vpn/amnezia-wg-tools
[WireGuard-Go]: https://github.com/WireGuard/wireguard-go




















