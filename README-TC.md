# ShadowDrive 
## 語言選擇：
[English](https://github.com/Knockoi/Shadow-ESC/blob/main/README.md) | [日本語](https://github.com/Knockoi/Shadow-ESC/blob/main/README-JP.md) | [繁體中文](https://github.com/Knockoi/Shadow-ESC/blob/main/README-TC.md)
## 致謝  
我要在此衷心感謝JLCPCB對本專題的大力支持與贊助。沒有JLCPCB的幫助,我無法順利完成這項專題。JLCPCB不僅提供了專案所需的印製電路板,他們家的PCB品質還非常優良,完全符合我專案的要求。在此,我再次表達我的誠摯謝意。JLCPCB對本專題發展的推動,將激勵我繼續努力,創造出更多有價值的作品。JLCPCB所給予的支持,對我而言意義非凡。衷心感謝JLCPCB,使我的創作之路變得更加順遂。   
JLCPCB 是一家領先的 PCB 製造商，以其卓越的品質、快速的周轉時間和經濟實惠而聞名。該公司對精度的承諾和對行業標準的遵守確保了高品質的印刷電路板。 JLCPCB 憑藉用戶友好的平台、透明的定價和包括組裝選項在內的全面服務，迎合了全球客戶的需求。其高效的流程和快速的製造使其成為工期緊迫的專案的理想選擇。總體而言，JLCPCB 是一種可靠且經濟高效的解決方案，可滿足廣泛的工程和創新需求。  
## 概述  
相較於一般的電動滑板控制器ShadowDrive有著更小的體積與超高的集成度，雖然面積只有信用卡大小，但控制能力絕不馬虎，可以控制60V 170A Peak 300A的電機(單路)。
  ![image](https://github.com/Knockoi/Shadow-ESC/blob/main/Image/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202023-12-25%20011755.png)
  
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
### 以上資料從VESC 的商品介紹上COPY

  基本使用可以參考VESC的使用方法。  
  設計藍圖來自於vedderb的完美專題  
      - [VESC 無刷馬達驅動器](https://github.com/vedderb/bldc)



