# K210 Tutorial
Copyright © 2023 宏宇創新有限公司，保留所有權利； Universpirit Innovation Limited. All rights reserved.
___________
## Table of content
- [x] [Setup](https://github.com/universpirit/K210_Tutorial_Public/tree/main#setup)
- [ ] [Syntax](https://github.com/universpirit/K210_Tutorial_Public/tree/main#syntax)
- [ ] [Program Body](https://github.com/universpirit/K210_Tutorial_Public/tree/main#program-body)
- [ ] [Peripherals](https://github.com/universpirit/K210_Tutorial_Public/tree/main#peripherals)
- [ ] [Robot Control](https://github.com/universpirit/K210_Tutorial_Public/tree/main#robot-control)
___________
### Reminder
1. 蘋果電腦用戶請攜帶有USB type-c轉USB的轉接頭<br>
   Macbook user please bring along a USB type-c to USB adapter
2. 上課前請先跟從以下指示下載及安裝適當的軟件<br>
   Please follow the instructions below to download and install the required software before the lesson
3. 上課前請先將電腦的電量充滿<br>
   Please fully charge the computer before the lesson
___________
## Setup

### Windows

<details>
<summary>按此打開 Click here</summary>

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

</details>

### Mac OS

<details>
<summary>按此打開 Click here</summary>

#### Step 1 - USB driver
1. <p>系統會自動安裝USB驅動<br>The system will automatically install the required USB driver</p>
   
#### Step 2 - MaixPy IDE
1. 打開[MaixPy IDE](Setup/Mac%20OS/MaixPyIDE/maixpy-ide-mac-0.2.5_2.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
   Click [MaixPy IDE](Setup/Mac%20OS/MaixPyIDE/maixpy-ide-mac-0.2.5_2.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
2. 解壓縮檔案<br>
   Unzip the file
3. 運行檔案```maixpy-ide-mac-0.2.5_2```，需要在```安全與隱私性```選擇```仍要打開```以運行軟件<br>
   Execute ```maixpy-ide-mac-0.2.5_2```, you need to go to ```Privacy & Security``` and select ```Open Anyway``` to run the software<br>
   [<img src="/img/for%20setup/unauthorized_app_warn_mac.png" width="210">](#)<br>[<img src="/img/for%20setup/unauthorized_app_setting_mac.png" width="381">](#)[<img src="/img/for%20setup/unauthorized_app_open_anyway_mac.png" width="379">](#)
#### Step 3 - K210 firmware
1. 打開[k210_fimware](Setup/Mac%20OS/K210%20firmware/kflash_gui_v1.8.1_macOS.zip)並點選右邊的[<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#)下載<br>
   Click [k210_fimware](Setup/Mac%20OS/K210%20firmware/kflash_gui_v1.8.1_macOS.zip) and press [<img src="/img/for%20setup/github_download_icon.PNG" width="14">](#) on the right to start downloading
2. 解壓縮檔案<br>
   Unzip the file
3. 使用USB Type-C線接駁MaixNano至電腦<br>
   Connect MaixNano to your computer via a USB Type-C cable
4. 開啟```kflash_gui```，需要在```安全與隱私性```選擇```仍要打開```以運行軟件<br>
   Run ```kflash_gui```, you need to go to ```Privacy & Security``` and select ```Open Anyway``` to run the software<br>
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

</details>

___________
## Syntax

<table>
<tr>
<td> 類別 Type </td> <td> c / c++ </td> <td> python </td>
</tr>
<tr>
<td> 循環 Loop </td>
<td>

```c
while(1)
{
//...
}

for(int i=0;i<6;i++)
   printf("%d\n",i);
printf("end\n");
```

</td>
<td>

```python
while True:
   #...
   pass

for x in range(6):
   print(x)
else:
   print("end")
```

</td>
</tr>
<tr>
<td> 分支 Branching </td>
<td>

```c
if(a==0)
{
   //...
}
else if(a==1)
{
   //...
}
else
{
   //...
}

switch(a)
{
   case 0:
      //...
      break;
   case 1:
      //...
      break;
   default:
      //...
      break;
}
```

</td>
<td>

```python
if a==0:
   #...
   pass
elif a==1:
   #...
   pass
else
   #...
   pass
```

</td>
</tr>
<tr>
<td> 運算 operation </td>
<td>

```c
int a = 0;
int b = 1;
while(1)
{
   printf("%d ",b);
   b += a;
   a = b-a;
   // + - * / %
}
```

</td>
<td>

```python
a,b = 0,0
while True:
   a,b = b,a+b
   # + - * / %
```

</td>
</tr>
<tr>
<td> 邏輯運算 logical operation </td>
<td>

```c
//比較 comparison
a==0
a>0
a<0
a>=0
a<=0
a!=0
a<>0 //?

//邏輯運算 logical operation
!(a==0)
a>1 && a<=3
a>1 && a<=3 && a!=2
a>1 || a<=3
a>1 || a<=3 || a!=2
a>1 && a<=3 || a!=2   // 9 / 3(3) = ?
(a>1 && a<=3) || a!=2 // (9/3)x3 = 9
a>1 && (a<=3 || a!=2) // 9/(3x3) = 1
```

</td>
<td>

```python
#比較 comparison
a==0
a>0
a<0
a>=0
a<=0
a!=0
a<>0

#邏輯運算 logical operation
not(a==0)
a>1 and a<=3
a>1 and a<=3 and a!=2
a>1 or a<=3
a>1 or a<=3 or a!=2
a>1 and a<=3 or a!=2
(a>1 and a<=3) or a!=2
a>1 and (a<=3 or a!=2)
```

</td>
</tr>
<tr>
<td> 1D Array/List </td>
<td>

```c
int num_list[3];

for(int i=0;i<3;i++)
   num_list[i] = i;

for(int i=0;i<3;i++)
   printf("%d ",num_list[i]);
//Output:
//1 2 3
```

</td>
<td>

```python
num_list = []

for i in range(3):
    num_list.append(i)

for num in num_list:
   print(num)
#Output:
#1
#2
#3
print(num_list)
#Output:
#[0, 1, 2]
```

</td>
</table>

___________
## 程序主體 Program Body

<table>
<tr>
<td> 類別 Type </td> <td> c / c++ </td> <td> python </td> <td> 用途 Use </td>
</tr>
<tr>
<td>標頭檔 Header Files<br>程序庫 Library</td>
<td>

```c
#include "sensor.h"
#include "image.h"
#include "time.h"
```

</td>
<td>

```python
import sensor, image, time

#import part of the whole header library
from fpioa_manager import fm
from machine import UART, Timer, PWM
from Maix import GPIO
```

</td>
<td>讓電腦知道程序碼的調用範圍及位置<br>To let the computer know what and where are pieces of program to be used</td>
</tr>
<tr>
<td>全域變量 Global Variable</td>
<td>

```c
int led = 13;
```

</td>
<td>

```python
led_pin = 13
```

</td>
<td>整個程序的函數都能調用的變量<br>All function of the program could access these variables</td>
</tr>
<tr>
<td>準備步驟 Preparation Block<br>初始化 Initialization</td>
<td>

```c
void setup()
{
   Serial.begin(9600);
   pinMode(led,OUTPUT);
}
```

</td>
<td>

```python
fm.register(led,fm.fpioa.GPIO0)
led_r=GPIO(GPIO.GPIO0,GPIO.OUT)
```

</td>
</td>
<td>變量、函數及傳感器等初始化設定(只執行一次)<br>Initialization for variables, functions, sensors, etc. (Only execute once)</td>
</tr>
</tr>
<tr>
<td>執行步驟 Execution Block<br>無限循環 Infinite Loop</td>
<td>

```c
void loop()
{
   digitalWrite(led,HIGH);
   delay(1000);
   digitalWrite(led,LOW);
   delay(1000);
}
```

</td>
<td>

```python
while True:
   led_r.value(1)
   time.sleep_ms(1000)
   led_r.value(0)
   time.sleep_ms(1000)
```

</td>
</td>
<td>主程序本體，通常包括讀取傳感器、算法運行及執行器控制等<br>Main program body. Usually composed of data reading for sensors, algorithm running, actuator control, etc.</td>
</tr>
</tr>
</tr>
<tr>
<td> </td>
<td> </td>
<td> </td>
</tr>
<tr>
<td>全部<br>All together</td>
<td>

```c
#include "sensor.h"
#include "image.h"
#include "time.h"

int led = 13;

void setup()
{
   Serial.begin(9600);
   pinMode(led,OUTPUT);
}

void loop()
{
   digitalWrite(led,HIGH);
   delay(1000);
   digitalWrite(led,LOW);
   delay(1000);
}
```

</td>
<td>

```python
import sensor, image, time

#import part of the whole header library
from fpioa_manager import fm
from machine import UART, Timer, PWM
from Maix import GPIO

led_pin = 13

fm.register(led,fm.fpioa.GPIO0)
led_r=GPIO(GPIO.GPIO0,GPIO.OUT)

while True:
   led_r.value(1)
   time.sleep_ms(1000)
   led_r.value(0)
   time.sleep_ms(1000)
```

</td>
<td>/</td>
</tr>
</table>

___________
## Peripherals
### GPIO (General Purpose Input/Output)

<details>
<summary>詳細解釋 Detailed Explanation</summary>

>**GPIO (通用輸入/輸出)**是一種用於與外部設備進行**數位通訊的介面**。 它是許多嵌入式系統和單晶片中常見的功能之一。
>GPIO允許處理器或微控制器的接腳在不同的模式下進行輸入或輸出操作。 <br>
>作為**輸入**，GPIO引腳可以**接收**來自外部設備 (例如感測器或開關)的訊號。 <br>
>作為**輸出**，GPIO引腳可以**發送**訊號給外部設備 (例如LED燈或驅動器)。
>透過編程，開發人員可以配置GPIO引腳的工作模式 (輸入或輸出) 以及其他屬性 (例如上拉/下拉電阻、中斷功能等)。 然後，他們可以使用適當的程式碼讀取輸入引腳的狀態或控制輸出引腳的電平。 這使得嵌入式系統能夠與外界進行交互，並與各種外部設備進行通訊。
>GPIO的靈活性和通用性使其在許多應用中廣泛應用，例如嵌入式系統、物聯網設備、感測器介面、控制器、機器人等。

>**GPIO (General Purpose Input/Output)** is an interface used for **digital communication with external devices**. It is one of the common features found in many embedded systems and single chips.
>GPIO allows the pins of a processor or microcontroller to operate as input or output in different modes.<br>
>As **inputs**, GPIO pins can **receive signals** from external devices such as sensors or switches.<br>
>As **outputs**, GPIO pins can **send signals** to external devices (such as LED lights or drivers).<br>
>Through programming, developers can configure the GPIO pin's operating mode (input or output) and other attributes (such as pull-up/pull-down resistors, interrupt capabilities, etc.). They can then use appropriate code to read the status of an input pin or control the level of an output pin. This enables embedded systems to interact with the outside world and communicate with various external devices.
>The flexibility and versatility of GPIO make it widely used in many applications, such as embedded systems, IoT devices, sensor interfaces, controllers, robots, etc.
</details>

#### 電壓、電流、電阻  Voltage;Current;Resistance [^1]
[<img src="https://stemextreme.com/wp-content/uploads/2021/01/Screen-Shot-2021-01-07-at-8.52.38-PM-768x474.png" width="400">](#)

- 微處理器的 **接腳(GPIO)** 可以設定為 **輸出** 或 **輸入**
   - 輸出：控制電壓高低 (控制水位高低)
   - 輸入：檢測電壓高低 (檢測水位高低)
[^1]: https://stemextreme.com/2021/01/08/common-circuit-terminology/

#### 數字、模擬 Digital;Analog [^2]
[<img src="https://cdn.sparkfun.com/assets/learn_tutorials/2/1/5/analog_vs_digital.png?_gl=1*1l43nsr*_ga*MTgzMTkyMDQ2OC4xNjk3NzA4NjUz*_ga_T369JS7J9N*MTY5NzcwODY1My4xLjAuMTY5NzcwODY1My42MC4wLjA." width="400">](#)

- 接腳的輸出輸入也可以分兩種情況：**數字** 或 **模擬**
   - 數字 (digital)：只有 **高** 或 **低** (二進制的0或1)
   - 模擬 (analog)：可以是高至低間的 **任意位置** (任意電壓)
[^2]: https://learn.sparkfun.com/tutorials/logicblocks--digital-logic-introduction/what-is-digital-logic

#### GPIO
- 通常只使用 **電壓**
- 電子儀器間的 **溝通媒介** (類似人類的五官)

### PWM (Pulse Width Modulation)

<details>
<summary>詳細解釋 Detailed Explanation</summary>

>PWM (脈寬調變) 是一種電子訊號調變技術，用於控制電子設備的輸出功率。 它透過改變訊號的脈衝寬度來控制平均輸出電壓或功率的比例。 PWM通常用於控制各種電子設備，如馬達驅動器、LED調光、電源控制等。<br>
>在PWM中，訊號週期固定，但脈衝寬度可以根據需要進行調整。 脈衝寬度的比例決定了輸出訊號的平均功率。 例如，如果脈衝寬度佔總週期的一半，那麼輸出訊號的平均功率也將是輸入功率的一半。<br>
>PWM的工作原理是透過快速地開關輸出訊號來實現。 輸出訊號在每個週期內以高頻率的脈衝序列形式出現，脈衝的寬度根據所需的輸出功率進行調整。 透過改變脈衝的寬度和週期，可以實現對輸出訊號的精確控制。<br>
>PWM在電子領域應用廣泛，特別是在需要對電力進行精確控制的場景中。 它具有高效、可靠和精確的特點，因此被廣泛應用於調光、馬達速度控制、音訊放大器和直流-直流轉換器等領域。

>PWM (Pulse Width Modulation) is an electronic signal modulation technology used to control the output power of electronic equipment. It controls the ratio of the average output voltage or power by changing the pulse width of the signal. PWM is commonly used to control various electronic devices, such as motor drivers, LED dimming, power control, etc.<br>
>In PWM, the signal period is fixed, but the pulse width can be adjusted as needed. The ratio of pulse widths determines the average power of the output signal. For example, if the pulse width is half the total period, the average power of the output signal will be half the input power.<br>
>The working principle of PWM is to quickly switch output signals. The output signal appears in the form of a high-frequency pulse sequence in each cycle, and the width of the pulses is adjusted according to the required output power. By changing the width and period of the pulse, precise control of the output signal can be achieved.<br>
>PWM is widely used in the electronic field, especially in scenarios where precise control of power is required. It is efficient, reliable and accurate, so it is widely used in fields such as dimming, motor speed control, audio amplifiers, and DC-DC converters.

</details>

#### 從數字到模擬 Digital to Analog [^3]
[<img src="https://www.thomsonlinear.com/ds_images/images_relaunch/What-is-PWM-585x400.jpg" width="400">](#)

- 透過高頻率的 **開關** (數字輸出 0/1)去 **模仿** 低到高之前的 **任意輸出** (模擬輸出)
- 例子：
   - 看看你眼前的電腦/手機屏幕
   - 馬達速度控制

[^3]: https://www.thomsonlinear.com/en/support/tips/what-is-pwm

### UART

<details>
<summary>詳細解釋 Detailed Explanation</summary>

>UART (通用非同步收發傳輸器) 是一種常見的串行通訊協議，用於在電子設備之間傳輸資料。 UART透過將資料位元依照順序逐位元傳送，並使用起始位元和停止位元來標識資料的開始和結束，實現了可靠的資料傳輸。<br>
>UART通常由兩個設備組成：發送器 (Transmitter) 和接收器 (Receiver)。 發送器將要傳輸的資料位元依照特定的時序傳送到接收器，接收器則會將接收到的資料進行解碼和處理。<br>
>UART的資料傳輸速率 (波特率) 可以根據需求進行設定。 常見的波特率包括9600、19200、38400、57600和115200等。 資料傳輸時，UART使用逐位的方式，依照設定的波特率將每個位元傳送或接收。<br>
>UART是一種非同步通訊協議，意味著發送器和接收器的時鐘不同步。 在每個資料位元組之間，UART使用起始位元來指示資料傳輸的開始，並使用停止位元來指示資料傳輸的結束。 通常，UART也可以使用奇偶校驗位元來偵測和修正資料傳輸過程中的錯誤。<br>
>UART廣泛應用於各種電子設備和系統中，例如電腦、嵌入式系統、感測器、模組和通訊介面等。 它是一種簡單、可靠且易於實現的串行通訊協議，適用於中距離資料傳輸。

>UART (Universal Asynchronous Transceiver Transmitter) is a common serial communication protocol used to transmit data between electronic devices. UART achieves reliable data transmission by transmitting data bits bit by bit in sequence and using start bits and stop bits to mark the beginning and end of data.<br>
>UART usually consists of two devices: transmitter (Transmitter) and receiver (Receiver). The transmitter transmits the data bits to be transmitted to the receiver in a specific timing sequence, and the receiver decodes and processes the received data.<br>
>The data transfer rate (baud rate) of UART can be set according to needs. Common baud rates include 9600, 19200, 38400, 57600 and 115200, etc. When transmitting data, UART uses a bit-by-bit method to transmit or receive each bit according to the set baud rate.<br>
>UART is an asynchronous communication protocol, which means that the clocks of the transmitter and receiver are not synchronized. Between each data byte, the UART uses a start bit to indicate the beginning of the data transfer and a stop bit to indicate the end of the data transfer. Typically, UARTs can also use parity bits to detect and correct errors during data transmission.<br>
>UART is widely used in various electronic devices and systems, such as computers, embedded systems, sensors, modules and communication interfaces, etc. It is a simple, reliable and easy-to-implement serial communication protocol suitable for medium-distance data transmission.

</details>

#### 通訊協議 Communication Protocal
- 通訊協議是電子儀器間的 **溝通語言**
- 只有使用同一種語言時，雙方才能順利溝通
   - UART (Universal Asynchronous Transceiver Transmitter) 是其中一種較簡單易用的通訊協議

#### UART
- 速度 (Baud rate)
   - 相同速度才能溝通
   - 慢速：訊息表達需要較長時間；但比較穩定，不易出錯
   - 快速：訊息表達只需較短時間；但較易出錯
   - 通常用115200 (bit per second)
- Tx & Rx
   - Tx : 發送器 (Transmitter) 如人的嘴巴或肢體語言
   - Rx : 接收器 (Receiver) 如人的耳朵或眼睛
   - Tx對著Rx才能順利溝通

### Camera -> Image

<details>
<summary>詳細解釋 Detailed Explanation</summary>

>在電腦科學中，影像 (Image) 是由像素 (Pixel) 組成的二維圖形。 每個像素代表影像中的一個點，它包含了顏色和亮度等資訊。 圖像可以是靜態的 (如照片、繪畫) 或動態的 (如影片)。<br>
>計算機科學中的影像通常使用數字表示，每個像素由數字編碼來表示其顏色和亮度。 常見的影像格式包括點陣圖 (Bitmap) 和向量圖 (Vector)。 點陣圖使用像素陣列表示影像，每個像素的顏色資訊儲存在影像的特定位置。 向量圖使用數學公式和幾何圖形來描述圖像，它可以無損地縮放和調整大小。<br>
>影像處理是電腦科學中與影像相關的研究領域。 它涉及到對影像進行獲取、處理、分析和呈現等操作。 影像處理技術廣泛應用於電腦視覺、圖形學、醫學影像、影像壓縮、模式識別等領域。<br>
>總結來說，電腦科學中的圖像是由像素組成的二維圖形，用於表示靜態或動態的視覺資訊。 影像可以使用數位表示，並透過影像處理技術進行獲取、處理和分析。

>In computer science, an image is a two-dimensional graphic composed of pixels. Each pixel represents a point in the image, which contains information such as color and brightness. Images can be static (such as photos, or paintings) or dynamic (such as movies).<br>
>Images in computer science are often represented numerically, with each pixel being numerically encoded to represent its color and brightness. Common image formats include Bitmap and Vector. Bitmap uses an array of pixels to represent an image, with the color information of each pixel stored at a specific location in the image. Vector graphics use mathematical formulas and geometric shapes to describe images, and they can be scaled and resized losslessly.<br>
>Image processing is an image-related research field in computer science. It involves the acquisition, processing, analysis, and presentation of images. The image processing technology is widely used in computer vision, graphics, medical imaging, image compression, pattern recognition, and other fields.<br>
>In summary, images in computer science are two-dimensional graphics composed of pixels, used to represent static or dynamic visual information. Images can be digitally represented and acquired, processed, and analyzed through image processing technology.<br>

</details>

#### 三原色 Primary Colours [^4]
[<img src="https://i.imgur.com/4oF9Skq.png" width="600">](#)

- RGB
   - 紅綠藍是 **色光三原色** ，是光線的三原色
   - 越混合越接近白色
   - 對應人眼3種視錐細胞，其中對綠色最敏感
   - 討論主動發出光線時所使用的概念
   - 如：
      - 電筒
      - 屏幕
- CMY
   - 青藍洋紅黃是**色彩三原色**，是顏料的三原色
   - 越混合越接近黑色
   - 討論吸收或反射光線時所使用的概念
   - 如：
      - 印刷
      - 染色

[^4]: https://hackmd.io/@careylin73/aboutcolors

#### 色深 Colour Depth [^5]
[<img src="https://www.diyphotography.net/wp-content/uploads/2019/11/bit-depth-colour.jpg" width="600">](#)

- 將單一種 **原色** 的 **深淺程度** 分級
- 分級越多便越細緻 (越高色深)
- 將三種原色混合便成為人眼看見的其他彩色

[^5]: https://www.diyphotography.net/what-does-bit-depth-even-mean-and-does-it-matter/

#### 解析度 Resolution [^6]
[<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTF__XHIygdDmBKy55DzFX_NTAQS07U6fAErw&usqp=CAU" width="600">](#)

- 描述圖像像素的多少
- 越高越清晰、細節越豐富
- 常見的Full HD、 2k、 4k便是解析度的一種標準
- 這次攝像頭的解析度會用QVGA

[^6]: https://guidelines.pr1mer.tech/05-IconsImages/Image-Size-and-Resolution
___________
## Robot Control
> 將於課堂上更新...<br>Will be released during lessons...
___________
