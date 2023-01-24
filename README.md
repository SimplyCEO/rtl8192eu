RTL8192EU
=========
Linux driver for Realtek **RTL8192EU** based on official's **TP Link TL - WN823N V3 Beta** v5.2.19.1 from 2018-05-08<br>
Supports monitor mode and frame injection for penetration testing abilities.

|   Support         |   Tested  |   Status  |   Description                                     |
|-------------------|-----------|-----------|---------------------------------------------------|
|   Monitor Mode    |   ✅      |   🔵      |   Tested and working.                             |
|   Frame injection |   ✅      |   🔵      |   Tested and working.                             |
|   Kernel 4.15+    |   ✅      |   🟠      |   Kernel 6.1.7 tested.                            |

|   Devices         |   Tested  |   Status  |   Description                                     |
|-------------------|-----------|-----------|---------------------------------------------------|
|   DWA-131         |   ❌      |   🟡      |   Waiting confirmation.                           |
|   GW-300S Katana  |   ❌      |   🟡      |   Waiting confirmation.                           |
|   TL-WN821N V6    |   ❌      |   🟡      |   Waiting confirmation.                           |
|   TL-WN822N V5    |   ❌      |   🟡      |   Waiting confirmation.                           |
|   TL-WN823N V3    |   ❌      |   🟡      |   Waiting confirmation.                           |

Build
-----
Make sure you have installed the following packages:

|   Package     |   URL                                             |
|---------------|---------------------------------------------------|
|   gcc         |   https://ftp.gnu.org/gnu/gcc/                    |
|   git         |   https://github.com/git/git                      |
|   make        |   https://ftp.gnu.org/gnu/make/                   |

Download and unpack this repo, or just clone with git:
```sh
git clone https://gitlab.com/KanuX/rtl8192eu.git
cd rtl8192eu/
 ```

Build the module:
 ```sh
make -$(nproc) && sudo make install
 ```
 
Load the module:
 ```sh
 sudo modprobe 8192eu
 ```

 Original TP Link driver
 -----------------------
 https://static.tp-link.com/2018/201805/20180514/TP-Link_Driver_Linux_series8_beta.zip
