# Автоматическая установка
## Купите сервер, если его у вас нет

Для создания собственного VPN, вам понадобится виртуальный сервер VPS. \
Пошаговые инструкции по покупке VPS у некоторых популярных хостинг-провайдеров можно найти в разделе [Как запустить свой VPN c помощью Amnezia].

Если с вами поделились данными для подключения в виде [файла], [ключа в виде текста], или [qr-кода], покупать сервер не нужно, обратитесь к соответствующим инструкциям.

>**Минимальные системные требования для VPS:** \
>Операционная система - Linux, подходит Ubuntu 22.04 или Debian 11.\
>Виртуализация - KVM.\
>SSD - минимум 7 Гб.\
>Оперативная память (RAM) - рекомендуемая 2 Гб, но не меньше 1 Гб.\
>Предустановленное ПО и панель управления не требуются.

&nbsp;

## Установите приложение Amnezia


На первом экране приложение спросит ваши данные для подключения. Это данные вашего VPS сервера. Хостинг-провайдеры отправят вам их на почту после покупки VPS. В письме вы найдете: 

- **IP** : 192.565.ххx.xxx
- **Username**: root  (или  другое)
- **Password или SSH-key** : 2f9legf2...

Выберете “У меня есть данные для подключения”.


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/01_auto-install/img/ai_ru_1.png)

> Если вы приобрели VPS для Amnezia у Inferno solution, вместо IP логина и пароля вам могут отправить ключ в виде текста в таком формате VPN:///ue34nf\feh.....
> В этом случае  обратитесь к инструкции  [Подключение через ключ в виде текста] 


&nbsp;

## Выберете тип данных, который у вас есть.

В этом руководстве мы рассмотрим вариант подключения через IP, логин и пароль, поэтому выбираем "Настроить ваш сервер". 


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/01_auto-install/img/ai_ru_2.png)

&nbsp;

## Добавьте данные для подключения

Внесите IP логин и пароль от VPS - сервера, нажмите  “Продолжить”.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/01_auto-install/img/ai_ru_3.png)


Если вы меняли port, укажите его через двоеточие после IP.

Если в ваших данных подключения нет логина, впишите root. 

Вместо пароля, вы можете использовать SSH-ключ.


&nbsp;

## Выберете уровень контроля интернета в вашем регионе

При выборе **Экстремального** уровня контроля будет установлен OpenVPN в связке с маскировкой Cloak, это позволит посещать заблокированные сайты и добавит маскировку VPN-трафика под http-трафик. Системы анализа трафика никак не смогут распознать, что вы используете VPN. Ваш VPN будет защищен от блокировок даже в регионах с самым высоким уровнем цензуры. 

При выборе **Среднего или Высокого** уровня контроля будет установлен протокол AmneziaWG. Это форк протокола WireGuard-GO с защитой от блокировок. Его отличительная особенность - это измененные размеры Junk-пакетов и названия Magic-заголовков, по которым, система DPI распознает протокол WireGuard. Эти параметры так же можно изменить в настройках. Идеальный баланс между маскировкой и скоростью.

При выборе **Низкого** уровня контроля будет установлен протокол WireGuard без маскировки трафика. Подойдет для регионов, где не блокируются VPN-приложения и VPN-протоколы. Повышает уровень приватности пользователя, и дополнительно шифрует трафик. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/01_auto-install/img/ai_ru_4.png)


>  Если в вашем регионе заблокированы все неподконтрольные государству сайты и практически все коммерческие и некоммерческие VPN, рекомендуем с первого подключения выбрать **Экстремальный** уровень контроля, и не устанавливать другие протоколы, так как в ином случае IP адрес вашего VPS может быть распознан и заблокирован системами анализа и вы не сможете использовать его в будущем.  

&nbsp;

Дождитесь пока Amnezia настроит ваш VPN.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/01_auto-install/img/ai_ru_5.png)

Нажмите на кнопку **“Подключиться”**.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/01_auto-install/img/ai_ru_6.png)

Теперь вы можете делиться подключением с другими людьми, добавлять и удалять протоколы, выбрать сайты-исключения, установить собственный DNS и еще многое другое... 
Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции].

[Как запустить свой VPN c помощью Amnezia]: ../instructions/0_starter-guide
[файла]: ../instructions/04_file-connection
[QR-кода]: ../instructions/05_qr-code_connection
[ключа в виде текста]: ../instructions/03_text-key-connection
[FAQ]: ../faq
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]: ../instructions
[Подключение через ключ в виде текста]: ../instructions/03_text-key-connection