
# Server errors

### ServerCheckFailed

Возникает при попытке добавить новый сервер.  

Решение:

- Проверьте что сервер соответствует требованиям Amnezia 


    Операционная система - Linux, подходит Ubuntu 22.04 или Debian 11
    Виртуализация - KVM
    Оперативная память (RAM) - рекомендуется 2 Гб, но можно и меньше
    Предустановленное ПО и панель управления не требуются

### ServerPortAlreadyAllocatedError

Эта ошибка означает, что порт, который нужен протоколу в Amnezia, уже используется другим ПО.

Решение:


1.  У некоторых протоколов можно поменять порт:
- OpenVPN по умолчанию использует 443 порт для TCP-протокола, и 1194 порт для UDP , можно поменять на любые другие порты.
- WireGuard по-умолчанию использует 51820 порт, можно поменять на любой UDP порт.
- IKEv2 по умолчанию использует порты 500 и 4500, их нельзя менять.
- OpenVPN over Cloak по-умолчанию использует 443 порт, его можно менять, но мы не рекомендуем этого делать, так как  443 порт - это порт веб-трафика, любой другой порт может выдать маскировку.
- AmneziaWG использует случайный порт для каждого пользователя, а так же меняет его при каждой новой попытке установить протокол, поэтому если выбраный порт занят, просто вернитесь на шаг  назад и потом снова кликните “Установить”, или поменяйте на любой другой UDP порт вручную .


2. Проверьте, что у вас не установлено другое ПО, использующее порт протокола.

   Для **Windows** можно посмотреть какие порты уже используются другими программами
    - Нажмите **Win+R**
    - введите в строку **cmd** нажмите **Enter**
    - внести команду 
   ~~~ 
   netstat!!! -a 
   ~~~
    нажмите **Enter**
      В консоли отобразится перечень используемых портов с указанием какое приложение или служба ими распоряжается,
      можно сохранить этот список в файле **netstat -a** > **имя.txt**, по умолчанию он сохранится в (C:\\User\Username*\) ,
      где  Username - имя пользователя.

   Для **Linux** нам понадобится утилита netstat, если у вас ее нет, ее можно установить следующими командами:

    - RedHat и CentOS - 
   ~~~
   sudo yum install net-tools
   ~~~
    - Fedora 22+ - 
   ~~~
   dnf install net-tools
   ~~~
   
    - Debian/Ubuntu - 
   ~~~ 
   sudo apt-get install net-tools
   ~~~
   

   В консоли наберите 
   ~~~
   $ netstat -pnltu
   ~~~
   По аналогии с Windows в консоли отобразится перечень используемых портов с указанием - какое приложение или служба ими распаряжается.


3. Проверьте, что на вашем сервере открыты необходимые для протоколов порты.  Это можно посмотреть в меню панели управления виртуальным сервером в браузере, если таких данных нет, отправьте запрос в службу поддержки хостинга.


4. Подключитесь к вашему серверу по SSH, или откройте консоль сервера через веб-сайт и пропишите там **“sudo apt install lsof psmisc”** , после чего повторите попытку установить.


5. Если это не помогло, попробуйте настроить сервер с более ранней версии Amnezia (2.1.2 )




### ServerContainerMissingError

Ошибка значит, что контейнер с сервером отсутствует. Возникает если приложение не подключается к серверу и при смене настроек. 
Может возникать при удалении контейнера на сервере вручную без использования приложения.

***Варианты решения*** 

Заново добавьте сервер. 

### ServerDockerFailedError

Ошибка: Сбой в работе Docker-контейнера сервера.
Появляется при установке контейнера с VPN или изменении настроек протокола.
Может возникнуть при удалении контейнера с сервером, или при удалении протокола без использования приложения.

Варианты решения:

Заново добавьте сервер.

### ServerUserNotInSudo

Обозначает, что пользователь сервера не имеет Sudo-прав.
Возникает при установке контейнера с VPN или при добавлении файла с конфигурацией.

***Варианты решения***

1. Добавьте пользователя в группу Sudo. 
- Через visudo, если пакет sudo уже установлен, 
- Добавьте пользователя и установите пакет sudo, если пакет sudo не установлен.
2. Попробуйте настроить сервер из под root, вместо обычного пользователя.
3. Попробуйте убрать пароль на выполнение sudo команд.
4. Обратитесь с службу поддержки хостинга. 


### ServerPacketManagerError

Ошибка диспетчера пакетов сервера возникает при установке контейнера с сервером. 
Обозначает, что менеджер пакетов занят, возникает после 30 попыток установить пакеты.

***Варианты решения***

Причиной возникновения может служить обновление пакетов. 
- Подождите, пока обновления пакетов закончится, или пропишите в командной строке 
~~~
- sudo apt-get install <любая_утилита> 
~~~
чтобы переключить менеджер пакетов на другую задачу.
- Попробуйте перезагрузить сервер

Также возможно повреждение менеджера пакетов. Чтобы решить эту проблему, обратитесь в службу поддержки хостинга.






[Как запустить свой VPN c помощью Amnezia]: ../instructions/0_starter-guide
[Windows 11]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_11
[Windows 10]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_10
[Windows 8.1 или 7]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_8.1_or_Windows_7
[ссылка на релизы]: https://github.com/amnezia-vpn/amnezia-client/releases