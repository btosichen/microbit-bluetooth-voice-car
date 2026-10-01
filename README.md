# micro:bit Bluetooth Voice Car

公開的 GitHub Pages 網頁遙控器，用 Chrome 或 Edge 透過 Web Bluetooth 連線至 micro:bit。

## 使用方式

1. 開啟已部署的 GitHub Pages 網址。
2. 按「連接 micro:bit」，選擇已執行相容 Bluetooth UART 程式的小車。
3. 按「按一下說話」，以中文說出例如「前進 1 秒」、「右轉半秒」或「停止」。

> 網頁只包含控制介面；micro:bit 必須先燒錄相容的 Bluetooth UART 控制程式。語音辨識通常需要網路與 Chrome 的麥克風權限。

## 安全性

* 每次語音行駛最多 5 秒。
* 行駛期間每 150 ms 傳送一次命令。
* 時間到、按下停止或藍牙中斷時，網頁會送出停止指令。
