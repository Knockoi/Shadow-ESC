# ShadowDrive 
## 語言選擇：
[English](https://github.com/Knockoi/E-Stick/blob/main/README.md) | [简体中文](https://github.com/Knockoi/E-Stick/blob/main/ReadmeCN.md) | [繁體中文](https://github.com/Knockoi/E-Stick/blob/main/ReadmeTC.md)
  
## 概述  
相較於一般的電動滑板控制器ShadowDrive有著更小的體積與超高的集成度，雖然面積只有信用卡大小，但控制能力絕不馬虎，可以控制60V 170A Peak 300A的電機。
  ![image]()
  
## 硬體  
- MCU使用兩個STM32F405RGT6
- 可以選擇配置是否有MPU，陀螺儀使用MPU6500數據線就兩根SDA和SCK。
- 柵極控制器使用DRV8301~8303選用。
- LED顯示當前模式和系統資訊。
- 可以選配藍芽模組，有藍芽模組可以利用藍芽編輯ShadowDrive。

## 功能  
- 驅動卡丁車1~4驅都可以使用(4驅需要兩個ShadowDrive)
- 驅動電動滑板1~4驅都可以使用(4驅需要兩個ShadowDrive)
- 驅動電動滑板車
- 驅動ONE-WHEEL(需要選配有MPU的版本)
- 驅動任何單電機15000W的BLDC馬達
  
## 特徵
- 所有相位的電流和電壓測量（三分流器設計）
- 可調電壓濾波器
- 內建 IMU 晶片（加速計、陀螺儀）
- 再生煞車
- 牽引力控制（單設定和雙設定）
- 有感測器或無感測器操作+ 混合模式
- ASS 就緒（先進的無感測器啟動 = 0 RPM 起的全扭力）-
可設定的 RPM、電流、電壓和功率限制
- 輸入源：PPM、類比
- 通訊連接埠：USB、CAN、UAVCAN 、UART
- 所有輸入源的油門曲線和斜坡
- 用於加速和製動的獨立油門曲線
- 無縫 4 象限操作
- 電機轉數、安時、瓦時計數
- 顯示速度、功率、佔空比、安培流量、估計範圍和電池應用程式上的狀態
- 來自 VESC 陣列的累積資料
- 即時資料分析並透過通訊埠讀出
- 即時資料分析並透過 VESC-Tool APP 或 VESC-Tool 軟體讀取
- 可調節保護：
    以上資料從VESC 的商品介紹上COPY
基本設計可以參考VESC的使用方法。
設計藍圖來自於vedderb的完美專題
 - [VESC 無刷馬達驅動器]([https://awesomeopensource.com/project/elangosundar/awesome-README-templates](https://github.com/vedderb/bldc))



