
# SSH SFTP errors

***SshSftpEofError***\
***SshSftpNoSuchFileError***\
***SshSftpPermissionDeniedError***\
***SshSftpFailureError***\
***SshSftpBadMessageError***\
***SshSftpNoConnectionError***\
***SshSftpConnectionLostError***\
***SshSftpOpUnsupportedError***\
***SshSftpOpUnsupportedError***\
***SshSftpInvalidHandleError***\
***SshSftpNoSuchPathError***\
***SshSftpWriteProtectError***\
***SshSftpNoMediaError***
 
Решение: 
Попробуйте:

- Перезапустите Amnezia. 
- Попробуйте повторить подключение
- Переустановите сервер для VPN 
- Обратитесь в поддержку

***SshSftpFileAlreadyExistsError \
SftpError: File does not exist***

Ошибка возникает, когда пользователь производит установку не из под Root, 
либо некорректно настроил юзера Sudo. 

Решение:
- Попробовать произвести установку под Root
- Если п.1 не подходит, то добавьте пользователя (от имени которого, вы хотите установить Amnezia) в группу sudo и разрешите выполнять команды sudo без пароля.

[Как запустить свой VPN c помощью Amnezia]: ../instructions/0_starter-guide
[Windows 11]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_11
[Windows 10]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_10
[Windows 8.1 или 7]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_8.1_or_Windows_7
[ссылка на релизы]: https://github.com/amnezia-vpn/amnezia-client/releases