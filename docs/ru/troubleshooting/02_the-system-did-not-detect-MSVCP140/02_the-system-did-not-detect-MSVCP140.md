# The system did not detect MSVCP140.dll

При установке Amnezia VPN на Windows появляется ошибка "система не обнаружила **MSVCP140.dll** или **MSVCP141.dll**", что делать?
### Решение


Файл **msvcp140.dll** — одна из библиотек, входящих в состав компонентов Microsoft Visual Studio 2015, необходимых для запуска некоторых программ. 
По умолчанию располагается в папках C:\Windows\System32\ и C:\Windows\SysWOW64\, но может быть необходим и в папке с исполняемым файлом запускаемой программы. 
Для того чтобы исправить эту проблему, установите [данные библиотеки] 


[Как запустить свой VPN c помощью Amnezia]: ../instructions/0_starter-guide
[Windows 11]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_11
[Windows 10]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_10
[Windows 8.1 или 7]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_8.1_or_Windows_7
[ссылка на релизы]: https://github.com/amnezia-vpn/amnezia-client/releases
[данные библиотеки]: https://learn.microsoft.com/ru-ru/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022