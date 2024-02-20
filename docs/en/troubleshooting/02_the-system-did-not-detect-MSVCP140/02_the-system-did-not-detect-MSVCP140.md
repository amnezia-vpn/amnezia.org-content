# System did not find MSVCP140.dll or MSVCP141.dll

When installing Amnezia VPN on Windows, an error "system did not find **MSVCP140.dll** or **MSVCP141.dll**" appears, what to do?

>**Solution**
>
>The **msvcp140.dll** file is one of the libraries included in the Microsoft Visual Studio 2015 components required to run some programs.
By default, it is located in the folders C:\Windows\System32\ and C:\Windows\SysWOW64\, but in some cases, it may also be needed in the folder with the executable file of the program being launched.
To fix this issue, install [these libraries]


[these libraries]: https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022
