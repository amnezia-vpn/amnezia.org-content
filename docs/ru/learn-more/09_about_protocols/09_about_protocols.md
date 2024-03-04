# Описание протоколов

### О протоклах 

>Мы не рекомендуем использовать протоколы ОpenVPN, Wireguard, IKEv2 без маскировки трафика
в странах с высоким уровнем цензуры, так как ip-адрес вашего VPS может быть заблокирован.
Чтобы избежать блокировки  используйте только OpenVPN over Cloak.  

### OpenVPN  

Проверенный временем самый популярный VPN протокол. Использует собственный протокол
безопасности с SSL/TLS для шифрования и обмена ключами и поддерживает различные методы
аутентификации, что делает его подходящим для различных устройств и операционных систем.

Нормальное энергопотребление на мобильных устройствах. \
Гибкая настройка под потребности пользователя для работы с различными операционными системами и устройствами. \
Распознается системами анализ DPI, а значит подвержен блокировкам. \
Может работать как через сетевой протокол TCP, так и через UDP.


### ShadowSocks


Основан на прокси-протоколе SOCKS5, который защищает соединение с помощью шифра AEAD 
примерно по тем же принципам, что и туннель SSH. Соединение ShadowSocks сложно
идентифицировать потому что оно  практически идентично обычному соединению HTTPS.
Однако некоторые системы анализа трафика все-таки умеют распознавать соединение 
ShadowSocks, поэтому в странах с высоким уровнем цензуры мы рекомендуем использовать OpenVPN 
связке с Cloak.

Среднее энергопотребление на мобильных устройствах выше чем у OpenVPN. \
Возможна настройка протокола шифрования. \
Распознается некоторыми системами анализа DPI. \
Работает только через сетевой протокол TCP. 



###  OpenVPN over Cloak

Это связка из протокола OpenVPN и плагина Cloak, созданная специально для защиты от блокировок.
OpenVPN обеспечивает защищенное VPN-соединение, шифруя весь интернет-трафик между 
клиентом и сервером. 
Cloak защищает OpenVPN от обнаружения и  блокировок.  
Cloak может изменять метаданные пакетов таким образом, что он полностью маскирует VPN-трафик
под обычный web-трафик, а также защищает VPN от обнаружения методом Active Probing. Все это делает
его очень устойчивым  для обнаружения и блокировки.
Сразу после получения первого пакета данных Cloak аутентифицирует входящее соединение. В
случае сбоя аутентификации плагин  маскирует сервер под фейковый веб-сайт, а ваш VPN становится
незаметным для систем анализа. 
При высоком уровне интернет-цензуры в вашем регионе, советуем использовать с первого
подключения только OpenVPN over Cloak

Высокое энергопотребление на мобильных устройствах \
Гибкие настройки. \
Не распознается системами анализа DPI. \
Работает через сетевой протокол TCP. 

> Версии OpenVPN over Cloak установленные на версиях клиента младше 3, не совместимы с 
последующими версиями клиента. Если вы устанавливали OpenVPN over Cloak на 1 или 2 версии
 клиента, требуется переустановить протокол, что бы он работал на 3 и 4 версиях.

 ###  WireGuard

Относительно новый популярный VPN-протокол с упрощенной архитектурой. 
Обеспечивает стабильное VPN соединение, высокую производительность на всех устройствах. 
Использует жестко заданные настройки шифрования. WireGuard в сравнении с OpenVPN работает с  меньшей задержкой и лучшей пропускной способностью при передаче данных.

Низкое энергопотребление на мобильных устройствах. \
Минимальное количество настроек. \
Легко распознается системами анализа DPI,  подвержен блокировкам. \
Работает через сетевой протокол UDP.

###  IKEv2

Современный стабильный протокол. IKEv2 с уровнем шифрования IPSec. Передает данные через
фиксированные  UDP-порты 500 и 4500 защищая их надежными криптоалгоритмами 3DES и AES.
Позволяет очень быстро переключаться между сетями и устройствами. Благодаря своей
безопасности, стабильности и скорости работы, IKEv2, в настоящее время, является одним из лучших
решений VPN для мобильных устройств. Уязвим для обнаружения и блокировки. 

Низкое энергопотребление, на мобильных устройствах.  \
Минимальное количество настроек. \
Распознается системами анализа DPI. \
Работает только через сетевой протокол UDP.

###  AmneziaWG

Современная версия популярного VPN-протокола WireGuard. AmneziaWG опирается на фундамент, заложенный WireGuard, сохраняя упрощенную архитектуру и высокую производительность на всех устройствах.
WireGuard известен своей эффективностью, но у него есть проблемы с обнаружением из-за характерных сигнатур пакетов. AmneziaWG решает эту проблему за счет использования более совершенных методов обфускации, благодаря чему его трафик сливается с обычным интернет-трафиком.
Таким образом, AmneziaWG сохраняет высокую производительность оригинала, добавляя дополнительный уровень скрытности, что делает его отличным выбором для тех, кому нужно быстрое и незаметное VPN-соединение.

Доступно с AmneziaVPN на всех платформах. \
Низкое энергопотребление. \
Минимальное количество настроек. \
Не распознается системами DPI-анализа, устойчив к блокировке. \
Работает по сетевому протоколу UDP.


Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции]


[about-int-link]: /about
[FAQ]: ../faq 
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]:  ../instructions




















