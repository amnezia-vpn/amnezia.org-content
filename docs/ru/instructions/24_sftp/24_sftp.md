# Создание файлового хранилища SFTP


### Откройте главный экран Amnezia

 Внизу кликните на значок настроек.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_1.png)

Далее перейдите в раздел “Серверы”

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_2.png)

Выберете сервер, чтобы создать на нем файловое хранилище.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_3.png)


Выберете вкладку "Сервисы", \
Во вкладке "Сервисы" выберете “SFTP”.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_4.png)

Далее нажмите “Установить”

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_5.png)

После успешной установки вы увидите экран с настройками и данные для подключения к файловому хранилищу. \
Хост - это IP вашего сервера, порт обычно 22 или 222, логин и пароль.  \
С помощью этих данных можно получить доступ к файловому хранилищу через любой SFTP-клиент.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_6.png)

В данном случае мы подключимся к хранилищу через [FileZilla]. 

Установите приложение. На первом же экране добавьте данные в строку как на скриншоте. 

В случае с FileZilla добавьте к вашему IP строку sftp://, получится такой формат - sftp://199.10.20.171, 
внесите эти данные в строку “Хост”, остальные данные добавляем как есть. Нажмите “Быстрое соединение”
  
![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/instructions/24_sftp/img/sftp_ru_7.png)

Далее в окне “Удаленный сайт” появится директория, а в статусе подключение “Список каталогов извлечен” - это значит, что подключение прошло успешно и вы можете пользоваться файловым хранилищем с помощью FileZilla. 



> Вы можете пользоваться файловым хранилищем с помощью FileZilla и других сторонних приложений, а можете [смонтировать директорию] для хранилища на вашем компьютере.  

Если у вас остались вопросы, обратитесь к [FAQ], в наш [телеграм чат] или к [другим разделам инструкции]

[about-int-link]: /about
[FAQ]: ../faq
[телеграм чат]: https://t.me/amnezia_vpn
[другим разделам инструкции]: ../instructions
[смонтировать директорию]: ../instructions/24_sftp
[FileZilla]: https://filezilla-project.org/