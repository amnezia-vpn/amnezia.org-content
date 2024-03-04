# Error Codes

## Error 100: UnknownError

Unknown error - can occur under various circumstances.

> **Solution:**
>- Restart the application.
>- Try clearing the application cache.
>- Try removing the server or protocol and reconnecting.
>- If the error persists, send logs to the email support@amnezia.org or to [Telegram chat]

## Error 101: InternalError

Internal error - can occur due to incorrect operation of QT libraries or under other circumstances.

> **Solution:**
>- Restart the application.
>- Try clearing the application cache.
>- Try removing the server or protocol and reconnecting.
>- If the error persists, send logs to the email support@amnezia.org or to [Telegram chat]

## Error 102: NotImplementedError

The error may occur if you create a settings backup file and then try to restore settings from this backup in an older version of the application.
Protocols configured in newer versions of Amnezia may not be compatible with the older version and vice versa.

> **Solution:**
>- Try changing the settings.
>- Check if the protocol is supported by your version of the application. For example, AmneziaWG is not supported by versions of the application older than 3, and OpenVPN over Cloak installed on versions of the application older than 2.1.2 will not work on newer versions.
>- More detailed information can be found in the [table of supported protocols for versions 4 and newer] and [for versions 2.1.2-3.1.0]

## Error 200: ServerCheckFailed

Occurs when trying to add a new server.

>**Solution:**
>
>**Check if the server meets Amnezia requirements:**
>
>Supported processor architecture - x86-64 \
>Operating system - Linux, suitable for Ubuntu 22.04 or Debian 11 \
>Virtualization - KVM \
>SSD - minimum 7 GB \
>Random-access memory (RAM) - at least 1 GB \
>Preinstalled software and control panel are not required

## Error 201: ServerPortAlreadyAllocatedError

This error means that the port needed by the protocol in Amnezia is already in use by other software.

>**Solution:**
>
>**Some protocols can change the port:**
>- For OpenVPN, the default is a port randomizer, the recommended range is 30000-50000, but you can change it to any other port.
>- For WireGuard, the default is to use a port randomizer, the recommended range is 30000-50000, but you can change it to any UDP port.
>- IKEv2 by default uses ports 500 and 4500, which cannot be changed.
>- OpenVPN over Cloak by default uses port 443, it can be changed, but we do not recommend doing so, as port 443 is a web traffic port, VPN traffic can be detected on other ports even if web site masking is used.
>- For AmneziaWG, a port randomizer is also used, the recommended range is 30000-50000, it can also be changed to any other UDP port manually.
>
>**Check if you have other software installed that uses the protocol port.**
>For **Windows**, you can see which ports are already in use by other programs as follows:
>- Press **Win+R**,
>- type **cmd** into the box, press **Enter**,
> - enter the command below
> ~~~ 
   >netstat -a 
  > ~~~
> press **Enter**
The console will display a list of ports in use along with the application or service using them,
you can save this list in a file **netstat -a** > **name.txt**, by default it will be saved in (C:\\User\Username*\) ,
where Username is the username.
>
> For **Linux** we need the netstat utility, if you don't have it, you can install it with the following commands:
>
>    - for RedHat and CentOS -
>   ~~~
> sudo yum install net-tools
>  ~~~
> - for Fedora 22+ -
> ~~~
> dnf install net-tools
> ~~~
>
>- for Debian/Ubuntu -
> ~~~ 
> sudo apt-get install net-tools
> ~~~
>In the console, type
>  ~~~
>  $ netstat -pnltu
>  ~~~
> Similar to Windows, the console will display a list of ports in use along with which application or service is using them.\
> Check that the necessary ports for the protocols are open on your server. This can be viewed in the control panel menu of the virtual server in the browser. If this data is not available, send a request to the hosting support service.\
> Connect to your server via SSH, or open the server console through the website and enter **“sudo apt install lsof psmisc”** there, then try the installation again. \
> If this does not help, try setting up the server with an earlier version of Amnezia (for example, version 2.1.2)



## Error 202: ServerContainerMissingError

The error means that the server container is missing.
Occurs when the application fails to connect to the server or when changing settings.
It can also occur when manually deleting the container on the server without using the application.

> **Solution:**
>
> - Re-add the server.

## Error 203: ServerDockerFailedError

Error: Docker container server failure.
Occurs during the installation of a VPN container or when changing protocol settings.
May occur when removing the server container or protocol without using the application.

> **Solution:**
>
> - Re-add the server.

## Error 204: ServerCancelInstallation

Error: Server installation canceled.
May occur when the server installation is canceled by the user.

> **Solution:**
>
> If you did not cancel the server installation or want to initiate the server installation again, try restarting the server installation from the beginning or contact support via [Telegram chat] or email us at support@amnezia.org.

## Error 205: ServerUserNotInSudo

Indicates that the server user does not have sudo privileges.
Occurs during the installation of a VPN container or when adding a configuration file.

> **Solution:**
>
> - Add the user to the Sudo group. Use visudo if the sudo package is already installed.
> - Add the user and install the sudo package if the sudo package is not installed.
> - Try setting up the server as root instead of a regular user.
> - Try removing the password requirement for executing sudo commands.
> - Contact hosting support.

## Error 206: ServerPacketManagerError

Server package manager error. Occurs during the installation of a server container.
Indicates that the package manager is busy, occurring after 30 attempts to install packages. The cause may be package updates.

> **Solution:**
> - Wait for the package updates to finish, or enter the following command in the command line:
>~~~
> sudo apt-get install <any_utility> 
>~~~
> - Switch the package manager to another task, try restarting the server.

Package manager corruption is also possible.
> - To resolve this issue, contact hosting support.

## Error 300: SshRequestDeniedError

Occurs when incorrect data is entered while adding a new server.

> **Solution:**
>
> - Check the accuracy of the entered data.

## Error 301: SshInterruptedError

Occurs when adding a new server to the application, when connecting to the added server, or when changing server settings.

> **Solution:**
>
> - Check the stability of the internet connection, retry the operation as the issue is often related to internet connection stability.

## Error 302: SshInternalError

Occurs when adding a new server to the application, when connecting to the added server, or when changing server settings.

> **Solution:**
>
> - Try restarting the application and retry the operation.
> - Contact us via email at support@amnezia.org or [Telegram chat].

## Error 303: SshPrivateKeyError

Occurs when adding a new server to the application, when connecting to the added server, or when changing server settings.

> **Solution:**
>
> - Check the accuracy of the entered private key.

## Error 304: SshPrivateKeyFormatError

Occurs when adding a new server to the application, when connecting to the added server, or when changing server settings.

> **Solution:**
>
> - Check the format of the entered private key, it should be either **PEM** or **ED25519**.

## Error 305: SshTimeoutError

Occurs when adding a new server to the application, when connecting to the added server, or when changing server settings.
Various issues can lead to this error, such as incorrect port, IP, or SSH being blocked by a firewall.

> **Solution:**
>
> - Check the accuracy of the entered data, port, and IP.
> - Ensure that the device port is open.
> - Ensure that the server you are connecting to exists and has an active status in the hosting control panel.
> - SSH is not running on the server.

## SshSftpErrors

**Erorr 400: SshSftpEofError** \
**Erorr 401: SshSftpNoSuchFileError**\
**Erorr 402: SshSftpPermissionDeniedError**\
**Erorr 403: SshSftpFailureError**\
**Erorr 404: SshSftpBadMessageError**\
**Erorr 405: SshSftpNoConnectionError**\
**Erorr 406: SshSftpConnectionLostError**\
**Erorr 407: SshSftpOpUnsupportedError**\
**Erorr 408: SshSftpInvalidHandleError**\
**Erorr 409: SshSftpNoSuchPathError**\
**Erorr 411: SshSftpWriteProtectError**\
**Erorr 412: SshSftpNoMediaError**

> **Solution for the above SshSftpErrors:**
>
>- Restart Amnezia.
>- Try reconnecting.
>- Reinstall the server (VPS).
>- Contact support.

## Error 410: SshSftpFileAlreadyExistsError
(Sftp error: File does not exist)

The error occurs if the installation is not done as Root or if the Sudo user is not configured correctly.

> **Solution:**
>
>- Try installing as root.
>- If the first solution does not work, add the user (under which you want to install Amnezia) to the sudo group and allow sudo commands without a password.

## Error 501: OpenVpnConfigMissing

Error: OpenVPN configuration is missing.
Occurs when using the desktop version of the application.

> **Solution:**
>
>- Try clearing cache, restart the device, and reconnect.

## Error 502: OpenVpnManagementServerError

The error occurs during VPN connection setup in the desktop application.

> **Solution:**
>
>- Try clearing cache, restart the device, and reconnect.

## Error 503: ConfigMissing

The error indicates that the configuration is missing, occurring during VPN connection setup in the desktop application.

> **Solution:**
>
>- Try clearing cache, restart the device, and reconnect.

## Error 600: OpenVpnExecutableMissing

The error occurs when the OpenVPN executable file is missing, often encountered during VPN connection.

This means:
installation of files failed,
files were corrupted during installation,
or files are not found

> **Solution:**
>
>- Restart the device and reinstall the application.

## Error 601: ShadowSocksExecutableMissing

Error: ShadowSocks executable file is missing.

This means:
installation of files failed,
files were corrupted during installation,
or files are not found

> **Solution:**
>
>- Restart the device and reinstall the application.

## Error 602: CloakExecutableMissing

Error: Cloak executable file is missing.

This means:
installation of files failed,
files were corrupted during installation,
or files are not found

> **Solution:**
>
>- Restart the device and reinstall the application.

## Error 603: AmneziaServiceConnectionFailed

Error: Failed to connect to the Amnezia service.

This means that the AmneziaVPN-service (the service that installs Amnezia on your device) is damaged or removed.

> **Solution:**
>
>- Restart the device.
>- Reinstall the application.
>- On macOS, check if there is permission to use the AmneziaVPN-service.

## Error 604: ExecutableMissing

The error means that the executable file is missing.



## Error 700: OpenVpnAdaptersInUseError

OpenVPN adapters usage error.
May occur because another software is using OpenVPN adapter.
Occurs when connecting to OpenVPN.

> **Solution:**
>
>- Check if another VPN application connected to OpenVPN is enabled. Disable it.
>- Try restarting your device,
>- Restart the application.

## Error 701: OpenVpnUnknownError

Unknown OpenVPN error, occurs when connecting to OpenVPN.

> **Solution:**
>
>- Check if another VPN application connected to OpenVPN is enabled. Disable it.
>- Try restarting your device,
>- Restart the application

## Error 702: OpenVpnTapAdapterError

The error occurs due to issues with the OpenVpn TAP adapter.

> **Solution:**
>- Remove the OpenVPN TAP adapter and reconnect to VPN using the OpenVPN protocol.
>- If that doesn't help, install [OpenVPN 2.6].

## Error 703: AddressPoolError

Address pool error indicates that there are no addresses left for WireGuard and AmneziaWG configs. Amnezia supports up to 254 configurations for WireGuard.

> **Solution:**
>- If you are sure that fewer than 254 addresses are used, try removing WireGuard or AmneziaWG and reconnecting.
>- If not, use another server or protocol.

## Error 800: OpenSslFailed

Error may occur when connecting to VPN.

> **Solution:**
>
>- Try restarting your computer, reconnecting
>- If the error persists, contact our support in [Telegram chat], or email us at support@amnezia.org

## Error 802: ShadowSocksExecutableCrashed

Error: ShadowSocks executable file crashed.
May occur when connecting to VPN.

> **Solution:**
>
>- Try restarting your computer, reconnecting
>- If the error persists, contact our support in [Telegram chat], or email us at support@amnezia.org

## Error 803: CloakExecutableCrashed

Cloak executable file crash.
Error may occur when connecting to VPN.

> **Solution:**
>
>- Try restarting your computer, reconnecting.
>- If the error persists, contact our support in [Telegram chat], or email us at support@amnezia.org

## Error 900: ImportInvalidConfigError

Error indicates that the configuration file loaded is in an invalid format.

> **Solution:**
>
>- Check the format correctness. \
   For Amnezia, the format should be - ***.vpn***
>- Try creating or requesting a new config.
>- If the error persists, contact our support in [Telegram chat], or email us at support@amnezia.org

>If the above advice did not help, contact our support in [Telegram chat], or email us at support@amnezia.org

[Telegram chat]: https://t.me/amnezia_vpn_en
[Windows 11]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_11
[Windows 10]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_10
[Windows 8.1 или 7]: https://support.microsoft.com/ru-ru/windows/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%BE%D0%B2-tcp-ip-bd0a07af-15f5-cd6a-363f-ca2b6f391ace#WindowsVersion=Windows_8.1_or_Windows_7
[table of supported protocols for versions 4 and newer]: https://amnezia.org/en/learn-more/30_table-of-supported-devices/
[for versions 2.1.2-3.1.0]: https://en-docs.amnezia.org/guides/protocols-table-v2/
[OpenVPN 2.6]: https://community.openvpn.net/openvpn/wiki/Downloads 