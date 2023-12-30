
# Поддерживаемые операционные системы Linux для VPS   

# 
 
> Поддерживаются VPS сервера, с виртуализацией KVM, под управлением ОС Linux. \
> Рекомендуемые к установке на сервер ОС: Debian 11, Ubuntu 22.04. 

Ниже представлены другие варианты операционных систем, поддерживаемые AmneziaVPN. \
KVM - рекомендуемый тип виртуализации. При виртуализации OpenVZ, протоколы WireGuard и AmneziaWG не поддерживаются. 


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

✔* - Для IPSec (IKEv2) в настоящий момент, последняя рабочая версия - AmneziaVPN 2.0.10. После перезагрузки сервера, требуется переустановка контейнера. В случае downgrade-обновления, на версию AmneziaVPN более раннюю, чем 2.1.2, необходимо предварительно сделать backup настроек AmneziaVPN на устройстве.

—* - Для серверов с Ubuntu 18.04 и Debain 10, существует возможность обновление ядра Linux, с 4-й до 5-й версии, для поддержки протокола WireGuard.

— - Протокол не поддерживается.


> Для любых ОС на серверах, кроме Ubuntu 22 / 20, Debian 12 / 11, настоятельно рекомендуется выполнить предварительное обновление ОС, с последующей перезагрузкой сервера.

### Обновление Ubuntu / Debian
~~~
sudo apt update && sudo apt upgrade
~~~
Вариант, допустимый для root
~~~
apt update && apt upgrade
~~~
Перезагрузка 
~~~
sudo reboot
~~~
Вариант, допустимый для root
~~~
reboot
~~~
### Обновление CentOS 7
~~~
sudo yum check-update && sudo yum update
~~~

Вариант, допустимый для root
~~~  
yum check-update && yum update
~~~
 Перезагрузка 
~~~  
sudo reboot
~~~  

Вариант, допустимый для root
~~~  
reboot
~~~
### Обновление Fedora 26-30
~~~
sudo dnf check-update && sudo dnf update
~~~
Вариант, допустимый для root

~~~
dnf check-update && dnf update
~~~
 Перезагрузка 
~~~
sudo reboot
~~~
Вариант, допустимый для root
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




















