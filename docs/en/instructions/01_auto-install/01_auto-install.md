# Automatic installation
## Buy a server if you don't have one

To create your own VPN, you will need a VPS server. 
For step-by-step instructions on how to purchase a VPS from some popular hosting providers, see [How to Start Your VPN with Amnezia].

> Amnezia works with any servers running Ubuntu (officially supported version is 20.04), Debian 10 is also supported.

If another Amnezia user has shared their connection data with you, you do not need to buy a server.

&nbsp;

### Install the Amnezia app

On the first screen, the application will ask for your connection details.  These are the details of your VPS server. Hosting providers will send them to your mail after you buy a VPS.  In the email you will find

- **IP** : 192.565.ххx.xxx
- **Username** : root  (or other)
- **Password or SSH-key** : 2f9legf2...

Select "I have data to connect".


![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_1.png)

> If you purchased VPS for Amnezia from Inferno solution, instead of IP login and password you may be sent a key in the form of text in the following format VPN:///ue34nf\feh......
>In this case, please refer to the instructions [Connect via text key]

>If other Amnezia users have shared the connection with you, please refer to the sections: connecting with a [QR code], [file] , or [key in text]..    


&nbsp;

### Choose the data type you have.

In these instructions we will look at connecting via IP, username and password, so choose them.


![instruction2](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_2.png)

&nbsp;

### Add connection data

Enter IP login and password from VPS-server, click "Continue".

![instruction2](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_3.png)


>If you changed the port, specify it with a colon after the IP. 
>If your connection data does not include a login, leave root as the default. 
>Instead of a password, you can use an SSH key.



![instruction3](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_4.png)

&nbsp;

### Select the level of control in your region

If you select a **high level of control**, OpenVPN will be installed in conjunction with Cloak and ShadowSocks protocol.  This will allow you to visit blocked sites and add cloaking of VPN traffic as http traffic. Traffic analysis systems will not be able to recognize that you are using a VPN.  Your VPN will be protected from blocking even in regions with the highest level of censorship. 

If you choose the **medium level of control**, OpenVPN will be installed in conjunction with ShadowSocks. ShadowSocks like Cloak masks traffic as http traffic.  However, ShadowSocks masking is recognized by traffic analysis systems in some highly censored countries, so we do not recommend using OpenVPN over ShadowSocks in regions where other VPNs are blocked.  

If you select **low level of control**, OpenVPN without traffic masking will be installed. Suitable for regions where VPN applications and VPN protocols are not blocked. Increases the level of user privacy, and additionally encrypts traffic.

If you choose to configure VPN yourself, you will be offered a list of protocols. For more details on how to configure it yourself, please read the manual configuration instructions.


![instruction4](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_5.png)

>  If in your region all non-government-controlled sites and almost all commercial and non-commercial VPNs are blocked, we recommend to choose High level of control from the first connection, and do not install other protocols, because otherwise IP address of your VPS can be recognized and blocked by analysis systems, and you will not be able to use it in the future.

&nbsp;

### Wait for Amnezia to configure your VPN.

![instruction5](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_6.png)

Click on the **“Подключиться”** button. 

![instruction6](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/01_auto-install/img/ai_en_7.png.png)

Now you can share your connection with other people, add and remove protocols, select sites for which you want or don't want to use VPN, set your own DNS and much more.... 

If you still have questions, check out the [FAQ], our [Telegram chat] or [other sections of the manual]..

[How to Start Your VPN with Amnezia]: ../instructions/starter-guide
[file]: /about
[QR code]: /about
[key in text]: /about
[FAQ]
[Telegram chat]
[other sections of the manual]
