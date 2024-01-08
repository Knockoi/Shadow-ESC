# StarDrive   
## 語言選擇：
[English](https://github.com/Knockoi/E-Stick/blob/main/README.md) | [简体中文](https://github.com/Knockoi/E-Stick/blob/main/ReadmeCN.md) | [繁體中文](https://github.com/Knockoi/E-Stick/blob/main/ReadmeTC.md)
  
## 概述  
相較於一般的電動滑板控制器StarDrive有著更小的體積與超高的集成度，雖然面積只有信用卡大小，但控制能力絕不馬虎，可以控制60V 170A Peak 300A的電機。
  ![image](https://github.com/Knockoi/E-Stick/blob/main/Image/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202023-09-16%20235403.png)
  
## 硬體  
- MCU使用ESP32-C3-MINI-1為了小空間使用模組版本。
- 陀螺儀使用MPU6500數據線就兩根SDA和SCK。
- 電源管理使用IP5305高集成的行動電源充電IC。
- RGB顯示當前模式和系統資訊。  

## 功能  
- 電子筆: 能在不跟投影機連線的情況下連接電腦在投影幕上繪畫。
- 雷射筆: E-Stick頂端有雷射可以標示重點區域。
- 切換頁數: 利用左右鍵的自訂按鍵功能來實現翻頁功能。
- 滑鼠功能: 有左右鍵滑鼠位置的操縱則是利用搖桿和體感進行操縱。
- 體感操縱: 利用物理晃動來移動鼠標位置。
- 自訂按鍵: 利用藍牙連接手機或電腦來更改E-Stick的按鍵功能。
  
## 按鍵功能  
- 左鍵 與滑鼠左鍵相同功能，可利用mode鍵自訂按鍵
- 右鍵 與滑鼠右鍵相同功能，可利用mode鍵自訂按鍵
- 搖桿 分為4個方向，和中間的按鈕。只有中間的按可以自訂。默認長按為雷射開啟。
- MODE鍵 可以改變模式。長按>=5秒開啟藍牙連接。
- BOOT鍵 下載按鈕。按住Boot，然後按Reset可啟動韌體下載模式，透過序列埠下載韌體。
- RESET鍵 按此按鈕重新啟動系統。
- 開關鍵 按鍵持續時間長於 30ms，但小於 2s為開啟。在 1s 內連續兩次短按鍵為關閉。
    
基本按鍵可以參考ESP32-C3-DevKitM-1的使用方法。





