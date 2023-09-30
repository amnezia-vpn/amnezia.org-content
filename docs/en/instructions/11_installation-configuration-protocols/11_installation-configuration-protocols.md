# Installing and configuring protocols

### About the protocols

Amnezia is a multi-protocol self-hosted VPN. It supports configuration and installation of all modern secure open source VPN protocols: 
OpenVPN, WireGuard, ShadowSocks, IKv2/IPsec and OpenVPN with Cloak plugin. A more detailed description of the protocols can be found in [this] article, 
and below we will tell you how to install and configure VPN protocols with Amnezia in two clicks.
&nbsp;

### Open the Amnezia home screen 

On the main screen, click on the server name.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_1.png)

Click the gear icon to the right of the server name


![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_2.png)

Click on the "Protocols" tab 
Select the protocol you want to set . 
Instructions on how to change the protocol are [here].

If the protocol is already installed, the icon next to the protocol will change to an arrow.  

In this case, if you click on the name of the protocol, you will get to its settings menu.


![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_3.png)

Select a protocol or plug-in to change the settings.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_4.png)

### Configuring OpenVPN

The OpenVPN protocol is very flexible for customization.
You can change the subnet address in it. 
Network protocol 
Port 
Select the encryption method for the code and hash
TLS-auth adds another HMAC signature to SSL/TLS handshake packets, initiating additional packet integrity checking. 
A packet without a signature will not be processed. This will provide an additional layer of security to the SSL/TLS protocol, 
protecting the system from some types of attacks. Block DNS request outside of VPN - prevents your DNS server address from being leaked.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_5.png)

In the Cloak plugin you can change encryption and port. 

And also choose masking for traffic. 
You can enter any site in this box and when attempting to detect and intercept VPN traffic by DPI analysis systems, only this cloak will be displayed instead of VPN traffic.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_6.png)

In the ShadowSocks settings, you can change the encryption method and port.

> OpenVPN over ShadowSocks and OpenVPN over Cloak work only through the TCP network protocol,
> since ShadowSocks can only work through TCP.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/en/instructions/11_installation-configuration-protocols/img/icp_en_7.png)

If you still have questions, please refer to the [FAQ], our [Telegram chat] or [other sections of the manual]

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[this]
[here]
[FAQ]
[Telegram chat] 
[other sections of the manual]














