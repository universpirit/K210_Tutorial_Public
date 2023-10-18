# K210 Tutorial
Copyright © 2023 宏宇創新有限公司，保留所有權利； Universpirit Innovation Limited. All rights reserved.
___________
## Table of content
- [x] [Setup](https://github.com/universpirit/K210_Tutorial_Public/tree/main#setup)
- [ ] [Syntax](https://github.com/universpirit/K210_Tutorial_Public/tree/main#syntax)
- [ ] [Program Body](https://github.com/universpirit/K210_Tutorial_Public/tree/main#program-body)
- [ ] [Peripherals](https://github.com/universpirit/K210_Tutorial_Public/tree/main#peripherals)
___________
## Setup
### Windows
#### Step 1 - USB driver
1. Windows 10
   <p>系統會自動安裝USB驅動<br>The system will automatically install the required USB driver</p>
2. Windows 8
   1. 打開[USB驅動](/Setup/Windows/USB%20driver/driver21228_Setup.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
      Click [USB driver](/Setup/Windows/USB%20driver/driver21228_Setup.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
   2. 解壓縮檔案<br>
      Unzip the file
   3. 運行檔案```CDM21228_Setup```並選擇```是```以使用系統管理員權限<br>
      Execute ```CDM21228_Setup``` and choose ```Yes``` to run it with admin's right
   4. 點選下一步完成安裝，途中需要選擇```I accept this argeement```<br>
      Finish the installation, you need to choose ```I accept this argeement``` in one of the steps
#### Step 2 - MaixPy IDE
1. 打開[MaixPy IDE](Setup/Windows/MaixPyIDE/maixpy-ide-windows-0.2.5.exe.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
   Click [MaixPy IDE](Setup/Windows/MaixPyIDE/maixpy-ide-windows-0.2.5.exe.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
2. 解壓縮檔案<br>
   Unzip the file
3. 運行檔案```maixpy-ide-windows-0.2.5```並完成安裝，途中需要選擇```是```以使用系統管理員權限<br>
   Execute ```maixpy-ide-windows-0.2.5``` and finish the installation, you need to choose ```Yes``` to run it with admin's right
#### Step 3 - K210 firmware
1. 打開[k210_fimware](Setup/Windows/K210%20firmware/k210_firmware.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
   Click [k210_fimware](Setup/Windows/K210%20firmware/k210_firmware.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
2. 解壓縮檔案<br>
   Unzip the file
3. 使用USB Type-C線接駁MaixNano至電腦<br>
   Connect MaixNano to your computer via a USB Type-C cable
4. 開啟```kflash_gui```<br>
   Run ```kflash_gui```
5. 更改至下列設定<br>
   Change the setting as follows<br>
   [<img src="/img/for%20setup/kflash_gui_setting.PNG" width="400">](#)
6. 按```下載```<br>
   Press ```Download```
#### Step 4 - First Connection
1. 開啟```MaixPy IDE```<br>
   Run ```MaixPy IDE```
2. 使用USB Type-C線接駁MaixNano至電腦<br>
   Connect MaixNano to your computer via a USB Type-C cable
3. 更改設定：```Tools```&rarr;```Select Boards```&rarr;```Sipeed Maix Bit (with Mic)```<br>
   Modifying the setting as: ```Tools```&rarr;```Select Boards```&rarr;```Sipeed Maix Bit (with Mic)```
4. 按左下角的[<img src="/img/for%20setup/MaixPy_link_connection_icon.PNG" width="20">](#)鏈接至MaixNano<br>
   Click [<img src="/img/for%20setup/MaixPy_link_connection_icon.PNG" width="20">](#) at the bottom right corner to connect to MaixNano
5. 選擇適當的```COM port```<br>
   Select the appropriate ```COM port```<br>
   [<img src="/img/for%20setup/MaixPy_serial_port_selection.PNG" width="210">](#)
6. 按左下角的[<img src="/img/for%20setup/MaixPy_start_program_icon.PNG" width="20">](#)運行程序<br>
   Click [<img src="/img/for%20setup/MaixPy_start_program_icon.PNG" width="20">](#) at the bottom right corner to run the program
7. 拔除USB Type-C線前，請先斷開MaixPy IDE與MaixNano之間的鏈接<br>
   Before unplugging the USB Type-C wire, please first disconnect the connection between MaixPy IDE and MaixNano<br>
   [<img src="/img/for%20setup/MaixPy_stop_program_icon.PNG" width="22">](#) &rarr; [<img src="/img/for%20setup/MaixPy_break_connection_icon.PNG" width="22">](#)

### Mac OS
#### Step 1 - USB driver
1. <p>系統會自動安裝USB驅動<br>The system will automatically install the required USB driver</p>
   
#### Step 2 - MaixPy IDE
1. 打開[MaixPy IDE](Setup/Windows/MaixPyIDE/maixpy-ide-windows-0.2.5.exe.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
   Click [MaixPy IDE](Setup/Windows/MaixPyIDE/maixpy-ide-windows-0.2.5.exe.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
2. 解壓縮檔案<br>
   Unzip the file
3. 運行檔案```maixpy-ide-mac-0.2.5_2```，需要在```安全與隱私性```選擇```仍要打開```以運行軟件<br>
   Execute ```maixpy-ide-mac-0.2.5_2```, you need to go to ```Privacy & Security``` and select ```Open Anyway``` to run the software<br>
   [<img src="/img/for%20setup/unauthorized_app_warn_mac.png" width="210">](#)<br>[<img src="/img/for%20setup/unauthorized_app_setting_mac.png" width="350">](#)[<img src="/img/for%20setup/unauthorized_app_open_anyway_mac.png" width="349">](#)
#### Step 3 - K210 firmware
1. 打開[k210_fimware](Setup/Windows/K210%20firmware/k210_firmware.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
   Click [k210_fimware](Setup/Windows/K210%20firmware/k210_firmware.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
2. 解壓縮檔案<br>
   Unzip the file
3. 使用USB Type-C線接駁MaixNano至電腦<br>
   Connect MaixNano to your computer via a USB Type-C cable
4. 開啟```kflash_gui```<br>
   Run ```kflash_gui```
5. 更改至下列設定<br>
   Change the setting as follows<br>
   [<img src="/img/for%20setup/kflash_gui_setting_mac.jpg" width="400">](#)
6. 按```下載```<br>
   Press ```Download```
#### Step 4 - First Connection
1. 開啟```MaixPy IDE```<br>
   Run ```MaixPy IDE```
2. 使用USB Type-C線接駁MaixNano至電腦<br>
   Connect MaixNano to your computer via a USB Type-C cable
3. 更改設定：```Tools```&rarr;```Select Boards```&rarr;```Sipeed Maix Bit (with Mic)```<br>
   Modifying the setting as: ```Tools```&rarr;```Select Boards```&rarr;```Sipeed Maix Bit (with Mic)```<br>
   [<img src="/img/for%20setup/MaixPy_board_selection_mac.png" width="550">](#)
4. 按左下角的[<img src="/img/for%20setup/MaixPy_link_connection_icon.PNG" width="20">](#)鏈接至MaixNano<br>
   Click [<img src="/img/for%20setup/MaixPy_link_connection_icon.PNG" width="20">](#) at the bottom right corner to connect to MaixNano
5. 選擇適當的```COM port```<br>
   Select the appropriate ```COM port```<br>
   [<img src="/img/for%20setup/MaixPy_serial_port_selection_mac.png" width="210">](#)
6. 按左下角的[<img src="/img/for%20setup/MaixPy_start_program_icon.PNG" width="20">](#)運行程序<br>
   Click [<img src="/img/for%20setup/MaixPy_start_program_icon.PNG" width="20">](#) at the bottom right corner to run the program
7. 拔除USB Type-C線前，請先斷開MaixPy IDE與MaixNano之間的鏈接<br>
   Before unplugging the USB Type-C wire, please first disconnect the connection between MaixPy IDE and MaixNano<br>
   [<img src="/img/for%20setup/MaixPy_stop_program_icon.PNG" width="22">](#) &rarr; [<img src="/img/for%20setup/MaixPy_break_connection_icon.PNG" width="22">](#)
___________
## Syntax
> 將於課堂上更新...<br>Will be released during lessons...
___________
## Program Body
> 將於課堂上更新...<br>Will be released during lessons...
___________
## Peripherals
> 將於課堂上更新...<br>Will be released during lessons...
___________
