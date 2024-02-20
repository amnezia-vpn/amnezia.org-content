# Connection issues with OpenVPN over Cloak.


**Solution:**

>## Windows
>
>
>1. Check that the versions of your application and protocol match each other, as OpenVPN over Cloak installed in version 2.1.2 does not work in newer versions of the application and vice versa.
>
>2. Go to "Network Adapters" and disable the TAP Adapter V9 adapter (created by Amnezia), then remove it.
>
>![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_1.png)
>![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_2.png)
>
>3. Ensure that DHCP services are enabled on the device.
>
> Instructions from the Microsoft website for different versions.\
>    [Windows 11] \
>    [Windows 10] \
>    [Windows 8.1 or 7]
>4. Install any version of OpenVPN from 2.5.0 to 2.6.9 [here]
>5. Clear the cache of the AmneziaVPN application
>6. Try reinstalling the protocol
>## Android
>
>1. Check that the versions of your application and protocol match each other, as OpenVPN over Cloak installed in version 2.1.2 does not work in newer versions of the application and vice versa.
>
>2. Press the "Exit" or "Close application" button in the Amnezia VPN settings, then restart and try to connect again
>3. Reboot the device
>## iOS
>
>1. Check that the versions of your application and protocol match each other, as OpenVPN over Cloak installed in version 2.1.2 does not work in newer versions of the application and vice versa.
>2. Try connecting to the VPN not from the application, but from the system settings
    >   ![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_3.png)
    >   ![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_4.png)
>3. Go to system VPN settings, remove the Amnezia VPN profile, and try to connect again
    >   ![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/ru/troubleshooting/01_connection_problem_ovpn_cloak/img/ts_cpoc_ru_5.png)
>4. Ensure that the Amnezia VPN application has been granted permissions to use Wi-Fi and mobile data
>5. Reboot the device
>## Linux
>1. Check the correctness of the time on your device. System time should match the selected time zone.
>2. Reboot the device

&nbsp;


[How to set up your own VPN with Amnezia]: ../instructions/0_starter-guide
[Windows 11]: https://support.microsoft.com/en-us/windows/change-tcp-ip-settings-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_11
[Windows 10]: https://support.microsoft.com/en-us/windows/change-tcp-ip-settings-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_10
[Windows 8.1 or 7]: https://support.microsoft.com/en-us/windows/change-tcp-ip-settings-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_8.1_or_Windows_7
[here]: https://community.openvpn.net/openvpn/wiki/Downloads
