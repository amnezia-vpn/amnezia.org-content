# Creating an SFTP file store


### Open the Amnezia home screen

At the bottom, click on the settings icon.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_1.png)

Next, go to the "Servers" section

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_2.png)

Select a server to create file storage on it

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_3.png)


Select the Services tab, \
On the Services tab, select "SFTP".

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_4.png)


Next, click "Install"

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_5.png)

After successful installation, you will see a screen with settings and data for connecting to the file storage. \
Host is the IP of your server, port is usually 22 or 222, login and password. \
With this data you can access the file storage through any SFTP client.

![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_6.png)

In this case we will connect to the storage via [FileZilla]. 

Install the application. On the first screen add data to the string as on the screenshot. 

In case of FileZilla, add sftp:// string to your IP, the format will be sftp://199.10.20.171, add this data to the 
"Host" line, the rest of the data will be added as it is. Click "Quick connect"
  
![](https://raw.githubusercontent.com/amnezia-vpn/amnezia.org-content/master/docs/en/instructions/24_stfp/img/stfp_en_7.png)

Next, the directory will appear in the "Remote Site" window, and in the connection status "Directory list 
extracted" - this means that the connection was successful and you can use the file storage with FileZilla. 


> You can use file storage using FileZilla and other third-party applications, or you can [mount a directory] for storage on your computer. 

 If you still have questions, please refer to the [FAQ], our [Telegram chat] or [other sections of the manual]



[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[mount a directory]: ../instructions/24_stfp
[FileZilla]: https://filezilla-project.org/
[FAQ]: ../faq
[Telegram chat]: https://t.me/amnezia_vpn_en
[other sections of the manual]: ../instructions
