# Проблемы с подключением к OpenVPN over Cloak.


**Решение:**

## Windows 


1. Проверьте, чтобы версии вашего приложения и протокола соответствовали друг-другу, так как OpenVPN over Cloak, установленный в версии 2.1.2 не работает в более новых версиях приложения и наоборот. 

2. Зайдите в "Сетевые адаптеры" и отключите адаптер TAP Adapter V9 (его создает Amnezia), затем удалите его, если адаптеров несколько, удалите их все. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_1.png)
![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_2.png)

3. Проверьте, чтобы у вас были включены DHCP службы на устройстве.  
 
 Инструкции с сайта Microsoft для разных версий.\
    [Windows 11] \
    [Windows 10] \
    [Windows 8.1 или 7] 
4. Установите любую из версий OpenVPN с 2.5.0 по 2.6.9 [отсюда]
5. Очистите кэш приложения AmneziaVPN
6. Попробуйте переустановить протокол
## Android

1. Проверьте, чтобы версии вашего приложения и протокола соответствовали друг-другу, так как OpenVPN over Cloak, установленный в версии 2.1.2 не работает в более новых версиях приложения и наоборот.

2. Нажмите кнопку "Exit" или “Закрыть приложение” в настройках Amnezia VPN, зайдите заново и попробуйте подключиться
3. Перезагрузите устройство
## IOS

1. Проверьте, чтобы версии вашего приложения и протокола соответствовали друг-другу, так как OpenVPN over Cloak, установленный в версии 2.1.2 не работает в более новых версиях приложения и наоборот.
2. Попробуйте подключиться к VPN не из приложения, а из системных настроек
   ![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_3.png)
   ![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_4.png)
3. Зайдите в системные настройки VPN, удалите профиль Amnezia VPN и попробуйте подключиться вновь
   ![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_5.png)
4. Проверьте, чтобы приложению Amnezia VPN были выданы права на передачу Wi-Fi и мобильных данных
5. Перезагрузите устройство
## Linux
1. Проверьте корректность времени на вашем устройстве. Системное время должно совпадать с выбранным часовым поясом.
2. Перезагрузите устройство

&nbsp;


[Как запустить свой VPN c помощью Amnezia]: ../instructions/0_starter-guide
[Windows 11]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_11
[Windows 10]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_10
[Windows 8.1 или 7]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_8.1_or_Windows_7
[отсюда]: https://community.openvpn.net/openvpn/wiki/Downloads