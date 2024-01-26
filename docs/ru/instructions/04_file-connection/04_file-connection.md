# Подключение через файл 


В данном случае мы рассмотрим вариант подключения через файл с конфгурацией.

Файл должен быть в формате  **.vpn**, **.conf** или **.ovpn**

Не используйте файлы из публичных источников, они могли быть размещены с целью перехвата ваших личных данных. 

>**Минимальные системные требования для VPS:** \
>Операционная система - Linux, подходит Ubuntu 22.04 или Debian 11.\
>Поддерживаемая архитектура процессора - x86-64 \
>Виртуализация - KVM.\
>Адрес сервера c интернет-протоколом IPv4  \
>SSD - минимум 7 Гб.\
>Оперативная память (RAM) - рекомендуемая 2 Гб, но не меньше 1 Гб.\
>Предустановленное ПО и панель управления не требуются. \
>Серверы на Reg.ru и Yandex Cloud не подходят для установки VPN с помощью Amnezia



&nbsp;

## Установите приложение Amnezia

На первом экране приложение спросит ваши данные для подключения. Это данные VPS сервера. 

Выберете "У меня есть данные для подключения" 


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/04_file-connection/img/fc_ru_1.png)


## Выберете тип данных, который у вас есть. 

В этой инструкции мы рассмотрим подключение через файл с конфигурацией, поэтому выбираем “Открыть файл настроек, ключ или QR-code”


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/04_file-connection/img/fc_ru_2.png)

>Если ваши данные для подключения в другом формате, обратитесь к разделам подключение с помощью  [QR-кода], [ключа в виде текста] , [ручная] или [автоматическая] установка.

Нажмите на “Файл с настройками подключения” и выберете файл на вашем устройстве.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/04_file-connection/img/fc_ru_3.png)

Здесь вы можете посмотреть содержимое файла
далее нажмите “Подключиться” 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/04_file-connection/img/fc_ru_4.png)

Дождитесь пока Amnezia настроит ваш VPN.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/04_file-connection/img/fc_ru_5.png)

Нажмите на кнопку “Подключиться” на главном экране.


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/04_file-connection/img/fc_ru_6.png)


Теперь вы можете делиться подключением с другими людьми, добавлять и удалять протоколы, выбрать сайты-исключения, установить собственный DNS и еще многое другое... 

Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции]


[about-int-link]: /about
[QR-кода]: ../instructions/05_qr-code_connection
[ключа в виде текста]: ../instructions/03_text-key-connection
[FAQ]: ../faq 
[телеграм чат]: ../https://t.me/amnezia_vpn
[другим разделам инструкции]: ../instructions
[ручная]: ../instructions/02_manual-install
[автоматическая]: ../instructions/01_auto-install


