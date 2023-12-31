#  Смонтировать диск для SFTP хранилища 

Инструкцию “Как создать файловое хранилище” можно найти [здесь].  

Откройте главный экран Amnezia

 Внизу кликните на значок настроек.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_1.png)

Далее перейдите в раздел “Серверы”

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_2.png)


Выберете сервер с файловым хранилищем “SFTP”.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_3.png)


Выберете вкладку "Сервисы", \ 
Во вкладке "Сервисы" выберете “SFTP”.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_4.png)

Вы попадете в настройки файлового хранилища. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_5.png)

Перед тем, как смонтировать диск, установите [WinFsp] и [SSHFS-Win].


[WinFsp] 

 Перейдите по ссылке на гитхаб, пролистайте страницу до конца, выберете файл в формате **.msi**, как указано на скриншоте.


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_6.png)

[SSHFS-Win] 

Перейдите по ссылке на гитхаб, пролистайте страницу до раздела "Assets", выберете файл в формате .msi, как указано на скриншоте.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_7.png)

После установки нажмите “Смонтировать папку на устройство ”

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_8.png)

Amnezia смонтирует Диск на вашем устройстве, так вы получите доступ к хранилищу без сторонних приложений. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/25_sftp_mount_disk/img/sftpmd_ru_9.png)

Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции]

[about-int-link]: /about
[FAQ]: ../faq
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]: ../instructions 
[здесь]: ../instructions/24_sftp 
[WinFsp]: https://github.com/winfsp/winfsp/releases/tag/v2.0
[SSHFS-Win]: https://github.com/winfsp/sshfs-win/releases
