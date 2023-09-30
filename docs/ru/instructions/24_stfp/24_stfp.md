# Создание файлового хранилища STFP


&nbsp;

### Откройте главный экран Amnezia

 Внизу кликните на значок настроек (крайний правый).

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_1.png)

Далее перейдите в раздел “Серверы”

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_2.png)

Выберете сервер, чтобы создать на нем файловое хранилище

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_3.png)


Выберете вкладку Сервисы, 
Во вкладке Сервисы выберете  “STFP”.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_4.png)


Далее  нажмите “Установить”

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_5.png)

После успешной установки вы у видите экран с настройками и данные для подключения к файловому хранилищу. 
Хост - это IP вашего сервера, порт обычно  22 или  222, логин и пароль.  
С помощью этих данных можно получить доступ к файловому хранилищу через любой SFTP-клиент.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_6.png)

В данном случае Мы подключимся к хранилищк через FileZilla. 

Установите приложение. На первом же  экране  добавьте данные в строку как  на скриншоте. 

В случае с FileZilla добавьте к вашему  IP строку sftp://, получится такой формат - sftp://199.10.20.171, 
внесите эти данные в стрку “Хост”, остальные данные добавляем как есть. Нажмите “Быстрое соединение”
  
![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_7.png)

Далее в окне “Удаленный Сайт” появится директория,  а в статусе подключение “Список каталогов извлечен” - это значит, что подключение прошло успешно и вы можете пользоваться файловым хранилищем с помощью FileZilla. 

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_ru_8.png)

> Вы можете пользоваться файловым хранилищем с помощью FileZilla и других сторонних приложений, а можете [смонтировать директорию] для хранилища на вашем компьютере.  

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
