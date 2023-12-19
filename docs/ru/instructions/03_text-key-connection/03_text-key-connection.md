# Подключение через ключ в виде текста 


В этой инструкции мы рассмотрим вариант подключения через ключ в виде текста.

Ключ должен начинаться с **VPN:///** 

Не используйте ключи из публичных источников, они могли быть размещены с целью перехвата ваших личных данных. 

>**Минимальные системные требования для VPS:** \
>Операционная система - Linux, подходит Ubuntu 22.04 или Debian 11.\
>Виртуализация - KVM.\
>SSD - минимум 7 Гб.\
>Оперативная память (RAM) - рекомендуемая 2 Гб, но не меньше 1 Гб .\
>Предустановленное ПО и панель управления не требуются.

&nbsp;

## Установите приложение Amnezia

На первом экране приложение спросит ваши данные для подключения.\
Это данные VPS сервера.

Выберете "У меня есть данные для подключения" 


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_1.png)


## Выберете тип данных, который у вас есть. 

В этой инструкции мы рассмотрим подключение через ключ в виде текста, поэтому выбираем “Открыть файл конфига, ключ или QR-код”


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_2.png)

>Если ваши данные для подключения в другом формате, обратитесь к разделам подключение с помощью  [QR-кода], [файла], [ручная] или [автоматическая] установка.

Выберете "Ключ в виде текста". 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_3.png)


Скопируйте ключ и вставьте в строку  
![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_4.png)

На этом экране вы можете посмотреть содержимое ключа
Далее кликните “Подключиться”

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_5.png)

Дождитесь пока Amnezia настроит ваш VPN.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_6.png)


Нажмите на кнопку “Подключиться”. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/03_text-key-connection/img/tkc_ru_7.png)


Теперь вы можете делиться подключением с другими людьми, добавлять и удалять протоколы, выбрать сайты-исключения, установить собственный DNS и еще многое другое... 

Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции]


[QR-кода]: ../instructions/05_qr-code_connection
[FAQ]: /faq 
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]: ../instructions
[файла]: ../instructions/04_file-connection
[ручная]: ../instructions/02_manual-install
[автоматическая]: ../instructions/01_auto-install
