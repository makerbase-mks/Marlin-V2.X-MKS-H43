# Marlin-V2.X-MKS-H43
This reponsotory was downloaded from https://github.com/MarlinFirmware/Marlin/tree/bugfix-2.0.x, and added the support of MKS H43. This is for the convenience of users to clone and compile their own boards, especially before marlin officially incorporates the MKS H43 function. More infomation about MKS H43, please refer to https://github.com/makerbase-mks/MKS-H43.

## How to config
1. Using VSCode to open this Marlin source, and modify the motherboard type on the "platformio.ini" according to yours, just like:
```
default_envs = mks_robin_nano35
```
2. Config the MKS DWIN
- Open the "Configuration.h" file, find "DGUS_LCD_UI_MKS" and enable it,
- Open the "Configuration_adv.h" file, find "LCD_SERIAL_PORT", and configure the serial port number used to connect to H43. Please make sure that "LCD_SERIAL_PORT" should be different with the "SERIAL_PORT" in "Configuration.h", as "SERIAL_PORT" is used to communicate with the PC. And the baudrate should be set to 115200 by default.

3. There are two types of UI themes: green-theme-UI and blue-theme-UI, they can be config from "Configuration.h":

| UI THEME | H43 firmware version | Mainboard Marlin configuration |
| ------ | ------ | ------ |
| blue-theme-UI | V1.30 | In "Configuration.h" //#define USE_MKS_GREEN_UI |
| green-theme-UI  | V1.31 | In "Configuration.h" #define USE_MKS_GREEN_UI |

![](https://github.com/makerbase-mks/MKS-H43/blob/main/Images/BLUE_GREEN.png)


After config other options according to your machine, compile the source code, and update your motherboard. Then you can use the MKS H43 to display and touch!


## Note
- Thank you for using MKS products. If you have any questions during use, please contact us in time and we will work with you to solve it.
- For more product dynamic information and tutorial materials, you can always follow MKS's Facebook/Twitter/Discord/Reddit/Youtube and Github. Thank you!
- MKS Github: https://github.com/makerbase-mks  
- MKS Facebook: https://www.facebook.com/Makerbase.mks/  
- MKS Twitter: https://twitter.com/home?lang=en  
- MKS Discord: https://discord.gg/4uar57NEyU
- MKS Reddit: https://www.reddit.com/user/MAKERBASE-TEAM/ 

![mks_link](https://user-images.githubusercontent.com/12979070/149612087-01c6384c-beed-4d39-b0ba-d137c0cb7d31.png)

