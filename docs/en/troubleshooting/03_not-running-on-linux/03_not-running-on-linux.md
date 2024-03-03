# Application does not start on Linux

## When attempting to launch the Amnezia VPN application on Linux Ubuntu/ Mint, nothing happens.

>**Solution**
>
> - Run the following command in the terminal:
>~~~
>sudo apt install libxcb-cursor0
>~~~
> - Restart the application.

If your Linux subsystem differs from SystemD,
use this guide: [GitHub]

[GitHub]:  https://github.com/M9snikFeed/amnezia-vpn-runit/blob/main/README.md