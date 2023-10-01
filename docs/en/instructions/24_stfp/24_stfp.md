# Creating an STFP file store


&nbsp;

### Open the Amnezia home screen

On the home screen at the bottom, click on the settings icon (far right).

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_1.png)

Next, go to the "Servers" section

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_2.png)

Select a server to create file storage on it

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_3.png)


Select the Services tab, 
On the Services tab, select "STFP".

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_4.png)


Next, click "Install"

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_5.png)

After successful installation, you will see a screen with settings and data for connecting to the file storage. 
Host is the IP of your server, port is usually 22 or 222, login and password.  With this data you can access the 
file storage through any SFTP client.

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_6.png)

In this case we will connect to the storage via [FileZilla]. 
Install the application. On the first screen add data to the string as on the screenshot. 
In case of FileZilla, add sftp:// string to your IP, the format will be sftp://199.10.20.171, add this data to the 
"Host" line, the rest of the data will be added as it is. Click "Quick connect"
  
![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_7.png)

Next, the directory will appear in the "Remote Site" window, and in the connection status "Directory list 
extracted" - this means that the connection was successful and you can use the file storage with FileZilla. 

![instruction 1](https://raw.githubusercontent.com/Aftershock669/amnezia-open-docs/master/docs/ru/instructions/24_stfp/img/stfp_en_8.png)

> You can use file storage using FileZilla and other third-party applications, or you can [mount a directory] for storage on your computer. 

[amnezia-site-ext-link]: https://amnezia-web-nx1r.vercel.app
[about-int-link]: /about
[mount a directory]
[FileZilla]