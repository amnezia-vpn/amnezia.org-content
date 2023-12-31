# Установка и настройка протоколов

### О протоколах 

Amnezia это мультипротокольный self-hosted VPN. Поддерживает настройку и установку всех современных безопасных VPN-протоколов с открытым исходным кодом: 
OpenVPN, WireGuard, ShadowSocks, IKv2/IPsec и OpenVPN с плагином Cloak. Более подробное описание протоколов вы найдете в [этой] статье, 
а ниже мы расскажем, как в два клика установить и настроить VPN-протоколы c помощью Amnezia.
&nbsp;

 Откройте главный экран  

На главном экране внизу кликните на название сервера, как на скриншоте. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_1.png)

Кликните на значок шестеренки справа от названия сервера 


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_2.png)

Кликните на вкладку “Протоколы”.
Выберете протокол, который вы хотите установить.

Если протокол уже установлен, значок возле протокола поменяется на стрелку.  

В этом случае при нажатии на названии протокола, вы попадете в меню его настроек.

>Инструкция как подключатся к разным протоколам [здесь].

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_3.png)

Выберете протокол или плагин для изменения настроек.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_4.png)

### Настройка OpenVPN

Протокол OpenVPN очень гибкий для настроек. /
В нем можно поменять адрес подсети, /
Сетевой протокол, /
Порт, /
Выбрать метод шифрования кода и хэша, /
TLS-auth добавляет еще одну подпись к HMAC к handshake-пакетам SSL/TLS, инициируя дополнительную проверку целостности пакетов. Пакет без подписи не будет обрабатываться. Это обеспечит дополнительный уровень безопасности протокола SSL/TLS, защищая систему от некоторых видов атак. /
Block DNS request outside of VPN - предотвращает утечку адреса вашего DNS-сервера.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_5.png)

В плагине Cloak можно поменять шифрование и порт. 

А также выбрать маскировку для трафика. 
В эту графу можно вписать любой сайт и при попытке обнаружения и перехвата VPN-трафика системами анализа DPI, вместо VPN трафика будет отображаться только эта маскировка.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_6.png)

В настройках ShadowSocks можно изменить метод шифрования и порт. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_7.png)

В настройках AmneziaWG можно изменить "Magic" заголовки и размеры "Junk" пакетов.     

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/11_installation-configuration-protocols/img/icp_ru_8.png)

Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат], или к [другим разделам инструкции]


[about-int-link]: /about
[этой]: ../instructions/09_about_protocols
[здесь]: ../instructions/14_protocol-change
[FAQ]: ../faq 
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]: ../instructions

















