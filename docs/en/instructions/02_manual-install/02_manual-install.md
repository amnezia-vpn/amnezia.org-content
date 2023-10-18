# Manual installation
## Buy a server if you don't have one

To create your own VPN, buy a virtual VPS server. For step-by-step instructions on how to buy a VPS from some of the popular hosting providers, see [How to run your VPN with Amnezia].  

If your connection data has been shared with you in the form of a [file], [text key], or [qr code], you do not need to buy a server, please refer to the relevant instructions .

> Amnezia works with any server running Ubuntu (officially supported version is 22.04), Debian 11 is also supported.


&nbsp;

### Установите приложение Amnezia

On the first screen, the application will ask for your connection details.  These are the details of your VPS server. Hosting providers will send them to your mail after you buy a VPS.  In the email you will find :

- **IP** : 192.565.ххx.xxx
- **Username**: root  (or other)
- **Password или SSH-key** : 2f9legf2...

Install the Amnezia app


![instruction 1](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_1.png)

> If you purchased VPS for Amnezia from Inferno solution, instead of IP login and password you may be sent a key in the form of text in the following format VPN:///ue34nf\feh......
In this case, please refer to the instructions [Connect via text key].



&nbsp;

### Choose the data type you have.

In these instructions we will look at connecting via IP, username and password, so choose "Configure your server.

![instruction2](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_2.png)

&nbsp;

### Choose the data type you have.

In these instructions we will look at connecting via IP, username and password, so choose "Continue".

> If you changed the port, specify it with a colon after the IP. 
> If your connection data does not include a login, leave root as the default. 
> Instead of a password, you can use an SSH key.


![instruction3](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_3.png)

&nbsp;

### Self-configuration of VPN

Scroll down, select "Set up VPN by yourself", click "Continue".

![instruction4](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_4.png)

&nbsp;

### Select the VPN protocol

OpenVPN, WireGuard and IKEv2 are VPN protocols, each will add traffic encryption and provide access to blocked sites.  We recommend using them only in low censorship regions where VPN applications and VPN protocols are not blocked.  

ShadowSocks is a protocol that masks traffic as http traffic.  However, ShadowSocks cloaking is detected by firewalls by traffic analysis systems in some countries with high level of Internet censorship, so to protect your VPN from blocking we recommend to use Cloak additionally.

AmneziaWG is a fork of Wireguard-GO protocol with blocking protection. Its distinctive feature is changed Jank packet sizes and Magic header names, by which DPI system usually recognises WireGuard protocol. These parameters can also be changed in the settings. Ideal balance between cloaking and speed.    

OpenVPN over Cloak is OpenVPN with additional Cloak traffic masking. It will allow you to visit blocked sites and add VPN traffic cloaking to http traffic. Traffic analysis systems will not be able to recognise that you are using a VPN. Your VPN will be protected from blocking even in regions with the highest level of censorship.

More detailed description of all protocols and traffic masking can be found [here].

> If your region has a high level of censorship, blocked all non-government-controlled sites, commercial and non-commercial VPNs, we advise you to use OpenVPN over Clock from the first connection.

![instruction5](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_5.png)

&nbsp;

### Wait for Amnezia to configure your VPN.

![instruction5](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_6.png)

Click on the **“Connect”** button.


![instruction6](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/02_manual-install/img/mi_en_7.png)


Now you can share your connection with other people, add and remove protocols, select exclusion sites, set your own DNS and much more... 
If you still have questions, check out the [FAQ], our [Telegram chat] or [other sections of the manual]

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[How to run your VPN with Amnezia]: ../instructions/0_starter-guide
[here]: ../instructions/09_about_protocols
[FAQ]: ../faq
[Telegram chat]: https://t.me/amnezia_vpn_en
[other sections of the manual]: ../instructions
[file]: ../instructions/04_file-connection
[key in text]: ../instructions/03_text-key-connection
[QR code]: ../instructions/05_qr-code_connection
[text key]: ../instructions/03_text-key-connection
