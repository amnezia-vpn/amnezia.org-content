# Automatic installation

## Install the Amnezia app

On the first screen, the application will ask for your connection details, which are your VPS server's data. If you don't have a VPS server, refer to the [How to Start Your VPN with Amnezia] instructions, where examples of instructions for purchasing hosting and choosing the necessary settings are collected.
After purchasing a VPS, hosting providers will send you the server's IP, user name or ID, and password to your email. These details look something like this: 
- 
- **IP** : 192.565.ххx.xxx
- **Username** : root  (or other)
- **Password or SSH-key** : 2f9legf2...

Select "I have data to connect".


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_1.png)

>If you purchased VPS for Amnezia from Inferno solution, instead of IP login and password you may be sent a key in the form of text in the following format VPN:///ue34nf\feh......
>In this case, please refer to the instructions [Connect via text key]

 

&nbsp;

## Choose the data type you have.

In these instructions we will look at connecting via IP, username and password, so choose "Configure your server".


![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_2.png)

&nbsp;

## Add connection data

Enter IP login and password from VPS-server, click "Continue".

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_3.png)


If you changed the port, specify it with a colon after the IP. 

If your connection data does not include a login, leave root as the default. 

Instead of a password, you can use an SSH key.



## Select the level of internet control in your region

Selecting **Extreme** level of control will install OpenVPN in conjunction with Cloak. This will allow you to visit blocked sites and add cloaking of VPN traffic as http traffic. Traffic analysis systems will not be able to recognise that you are using a VPN. Your VPN will be protected from blocking even in regions with the highest level of censorship. 

If you select **Medium or High** level of control, AmneziaWG will be installed. This is a fork of the WireGuard-GO protocol with blocking protection. Its distinctive feature is modified Junk packets sizes and Magic headers names, by which the DPI system usually recognises the WireGuard protocol, these parameters can also be changed in the settings. Ideal balance between masking and speed.

Selecting **Low** control level will install WireGuard without traffic masking. Suitable for regions where VPN applications and VPN protocols are not blocked. Increases user privacy and additionally encrypts traffic.



![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_4.png)

>  If in your region all non-government-controlled sites and almost all commercial and non-commercial VPNs are blocked, we recommend to choose **Extreme** level of control from the first connection, and do not install other protocols, because otherwise IP address of your VPS can be recognized and blocked by analysis systems, and you will not be able to use it in the future.


&nbsp;

**Wait for Amnezia to configure your VPN**.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_5.png)

Click on the **“Connect”** button. 

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/01_auto-install/img/ai_en_6.png)

Now you can share your connection with other people, add and remove protocols, select sites for which you want or don't want to use VPN, set your own DNS and much more... 

If you still have questions, check out [Telegram chat] or [other sections of the manual].

[How to Start Your VPN with Amnezia]: ../instructions/0_starter-guide
[file]: ../instructions/04_file-connection
[QR code]: ../instructions/05_qr-code_connection
[key in text]: ../instructions/03_text-key-connection
[FAQ]: ../faq
[Telegram chat]: https://t.me/amnezia_vpn_en
[other sections of the manual]: ../instructions
[Connect via text key]: ../instructions/03_text-key-connection
[text key]: ../instructions/03_text-key-connection