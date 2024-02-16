# Installing VPN on Server

## Install the Amnezia Application

On the first screen, the application will ask for your connection details, which are the details of your VPS server. If you don't have a VPS server, refer to the [How to Start Your VPN with Amnezia] instructions, where examples of instructions for purchasing hosting and selecting the necessary settings are collected. After purchasing VPS hosting, providers will email you the IP data, username or ID, and password for the server. These data look something like this:

- **IP**: 192.565.xxx.xxx
- **Username**: root (or other)
- **Password or SSH-key**: 2f9legf2...

Select "I have connection details".

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_1.png)

> If you purchased VPS for Amnezia from Inferno solution, instead of IP login and password, you may receive a key in text format like this: VPN:///ue34nf\feh..... In this case, refer to the [Connection via Text Key] instructions.

## Choose the type of data you have.

In this guide, we will consider the option of connecting via IP, login, and password, so select "Configure your server".

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_2.png)

## Add connection data

Enter the IP, login, and password for the VPS server, then click "Continue".

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_3.png)

If you changed the port, specify it after the IP with a colon.

If your connection data does not include a login, enter root.

Instead of a password, you can use an SSH key.

## Choose the level of internet control in your region or switch to the tab with the protocol selection from the list.

> The protocol you choose can be removed or added to the application later.

When selecting **Extreme** level of control, OpenVPN will be installed with Cloak masking, allowing you to visit blocked sites and adding VPN traffic masking as HTTP traffic. Traffic analysis systems won't be able to recognize that you're using a VPN. Your VPN will be protected from blocking even in regions with the highest level of censorship.

When selecting **Medium or High** level of control, the AmneziaWG protocol will be installed. This is a WireGuard-GO protocol fork with protection against blocking. Its distinctive feature is modified sizes of Junk packets and names of Magic headers, by which the DPI system recognizes the WireGuard protocol. These parameters can also be changed in the settings. An ideal balance between masking and speed.

When selecting **Low** level of control, the WireGuard protocol will be installed without traffic masking. Suitable for regions where VPN applications and protocols are not blocked. It increases the user's privacy level and additionally encrypts traffic.

You can also learn more about protocols in the [protocol article on the site].
>If all non-government-controlled sites and practically all commercial and non-commercial VPNs are blocked in your region, we recommend selecting **Extreme** level of control from the first connection and not installing other protocols, as otherwise the IP address of your VPS may be recognized and blocked by traffic analysis systems, and you won't be able to use it in the future.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_4.png)

Wait for Amnezia to configure your VPN.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_5.png)

Click the **“Connect”** button.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_6.png)

Now you can [share your connection with others], [add and remove protocols], [select exception sites], [set your own DNS], and much more... If you have any questions, refer to the [FAQ], our [Telegram chat], or [other sections of the instructions].

[How to Start Your VPN with Amnezia]: ../instructions/0_starter-guide
[file]: ../instructions/04_file-connection
[QR code]: ../instructions/05_qr-code_connection
[text key]: ../instructions/03_text-key-connection
[FAQ]: ../faq
[Telegram chat]: https://t.me/amnezia_vpn
[other sections of the instructions]: ../instructions
[Connection via Text Key]: ../instructions/03_text-key-connection
[share your connection with others]: https://amnezia.org/en/instructions/10_sharing-connect
[add and remove protocols]: https://amnezia.org/en/instructions/11_installation-configuration-protocols
[select exception sites]: https://amnezia.org/en/instructions/21_split_tunneling
[set your own DNS]: https://amnezia.org/en/instructions/06_change-dns
[protocol article on the site]: https://amnezia.org/en/instructions/09_about_protocols
