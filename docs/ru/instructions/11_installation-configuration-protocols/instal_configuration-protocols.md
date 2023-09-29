# Установка и настройка протоколов

### О протоколах 

Amnezia это мультипротокольный self-hosted VPN. Поддерживает настройку и установку всех современых безопасных VPN-протоколов с окрытым исходным кодом: 
OpenVPN, WireGuard, ShadowSocks, IKv2/IPsec и OpenVPN с плагином Cloak. Более подробное описание протоколов вы найдете в [этой] статье, 
а ниже мы расскажем как в два клика установить и настрйоить VPN-протоколы c помощью Amnezia.
&nbsp;

### Откройте главный экран  

На главном экране  внизу  кликните на название сервера, как на скриншоте. 

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_1.png)

Кликните на значок шестеренки справа от названия сервера 


![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_2.png)

Кликните на вкладку “Протоколы” 
Выберете протокол, который вы хотите установить .

Если протокол уже установлен, значек возле протокола поменяется на стрелку.  

В этом случае при нажатии на названии  протокола, вы попадете в меню его настроек . 

>Инструкция как изменить протокол, и подсоединиться к VPN с выбранным протоколом [здесь].

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_3.png)

Выберете протокол или плагин для изменения настроек.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_4.png)

### Настройка OpenVPN

Протокол  OpenVPN очень гибкий для настроек.
В нем можно поменять адрес подсети. 
Сетевой протокол 
Порт 
Выбрать метод  шифрования кода и хэша
TLS-auth добавляет еще одну подпись к HMAC к handshake-пакетам SSL/TLS, инициируя дополнительную проверку целостности пакетов. Пакет без подписи не будет обрабатываясь. 
Это обеспечит дополнительный уровень безопасности протокола SSL/TLS, защищая систему от некоторых видов атак. 
Block DNS request outside of VPN - предотвращает утечку адреса вашего  DNS-сервера.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_5.png)

В плагине Cloak  можно поменять шифрование и порт. 

А так же выбрать маскировку для тарфика. 
В эту графу можно вписать любой сайт и при попытке  обнаружения и перехвата  VPN-трафика  системами анализа DPI,  вместо VPN трафика будет  отображаться только  эта маскировка.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_6.png)

В настройках ShadowSocks можно изменить метод шифрования и порт. 

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/installation-configuration-protocols/img/icp_ru_7.png)

Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции]

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[Как запустить свой VPN c помощью Amnezia]: https://amnezia-web-nx1r.vercel.app
[файл]: /about
[QR-кода]: /about
[ключа в виде текста]: /about
[инструкции]: /about 
[FAQ]: /about 
[телеграм чат]: /about 
[другим разделам инструкции]: /about
[Ручной]
[Автоматической]
[QR-кода]
[файл]
[ключ в виде текста]
[здесь] : /about 
[этой]: /about 



















