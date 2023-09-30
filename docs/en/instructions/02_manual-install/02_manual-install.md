# Manual installation
## Buy a server if you don't have one

To create your own VPN, buy a virtual VPS server. For step-by-step instructions on how to buy a VPS from some of the popular hosting providers, see [How to run your VPN with Amnezia].  

> Amnezia works with any server running Ubuntu (officially supported version is 20.04), Debian 10 is also supported.

 *If another Amnezia user has shared the connection data with you, you do not need to buy a server.

&nbsp;

### Установите приложение Amnezia

On the first screen, the application will ask for your connection details.  These are the details of your VPS server. Hosting providers will send them to your mail after you buy a VPS.  In the email you will find :

- **IP** : 192.565.ххx.xxx
- **Username**: root  (or other)
- **Password или SSH-key** : 2f9legf2...

Install the Amnezia app


![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_1.png)

> If you purchased VPS for Amnezia from Inferno solution, instead of IP login and password you may be sent a key in the form of text in the following format VPN:///ue34nf\feh......
In this case, please refer to the instructions [Connect via text key].

If other Amnezia users have shared the connection with you, please refer to the sections: connecting with a [QR code], [file] , or [key in text].    

&nbsp;

### Choose the data type you have.

In these instructions we will look at connecting via IP, username and password, so choose them.

![instruction2](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_2.png)

&nbsp;

### Choose the data type you have.

In these instructions we will look at connecting via IP, username and password, so choose "Continue".

> If you changed the port, specify it with a colon after the IP. 
> If your connection data does not include a login, leave root as the default. 
> Instead of a password, you can use an SSH key.


![instruction3](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_3.png)

&nbsp;

### Self-configuration of VPN

Scroll down, select "Set up VPN by yourself", click "Continue".

![instruction4](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_4.png)

&nbsp;

### Select the VPN protocol

A bit of information about the protocols to make it easier for you to make a choice. 

OpenVPN, WireGuard and IKEv2 are VPN protocols, each will add traffic encryption and provide access to blocked sites.  We recommend using them only in low-censorship regions where VPN applications and VPN protocols are not blocked.  

OpenVPN over ShadowSocks is a protocol bundle that masks traffic as http traffic. This option can be useful in cases where you don't want sites to know that you are using a VPN.  However, ShadowSocks cloaking is recognized by firewalls by traffic analysis systems in some countries with high level of Internet censorship, so to protect your VPN from blocking we recommend to use Cloak additionally.

OpenVPN over Cloak is OpenVPN with ShadowSocks protocol and additional Cloak traffic masking.  It will allow you to visit blocked sites and add VPN traffic masking to http traffic. Traffic analysis systems will not be able to recognize that you are using a VPN.  Your VPN will be protected from blocking even in regions with the highest level of censorship.  

More detailed description of all protocols and traffic masking can be found [here].

> If your region has a high level of censorship, blocked all non-government-controlled sites, commercial and non-commercial VPNs, we advise you to use OpenVPN over Clock from the first connection.

![instruction5](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_5.png)

&nbsp;

### Wait for Amnezia to configure your VPN.

![instruction5](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_6.png)

Click on the **“Connect”** button.


![instruction6](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/02_manual-install/img/mi_en_7.png)


Now you can share your connection with other people, add and remove protocols, select exclusion sites, set your own DNS and much more... 
If you still have questions, check out the [FAQ], our [Telegram chat] or other [sections of the manual]

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[How to run your VPN with Amnezia]: https://amnezia-web-nx1r.vercel.app
[QR code]
[file]
[key in text]
[here]
[FAQ]
[Telegram chat]
[sections of the manual]