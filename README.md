# Raspberry-Pi_Beginner

# 樹梅派 Raspberry Pi 完整入門與 AI 應用實戰講義
> 繁體中文｜從零到一：基礎介紹 → 系統安裝 → 基礎操作 → AI 模型部署 → 實戰專案

本專案提供一份完整、可直接跟著操作的樹梅派教學，適用 Raspberry Pi 4 / Pi 5，包含本地大模型、AI 視覺辨識、語音助手等實戰內容，並附上官方資源連結與圖文指引。

---

## 📌 目錄
1. [樹梅派基本介紹](sslocal://flow/file_open?url=%231-%E6%A8%B9%E6%A2%85%E6%B4%BE%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
2. [必備硬體清單](sslocal://flow/file_open?url=%232-%E5%BF%85%E5%82%99%E7%A1%AC%E9%AB%94%E6%B8%85%E5%96%AE&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
3. [作業系統安裝（圖文步驟）](sslocal://flow/file_open?url=%233-%E4%BD%9C%E6%A5%AD%E7%B3%BB%E7%B5%B1%E5%AE%89%E8%A3%9D%E5%9C%96%E6%96%87%E6%AD%A5%E9%A9%9F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
4. [首次開機與基礎設定](sslocal://flow/file_open?url=%234-%E9%A6%96%E6%AC%A1%E9%96%8B%E6%A9%9F%E8%88%87%E5%9F%BA%E7%A4%8E%E8%A8%AD%E5%AE%9A&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
5. [基礎指令與遠端控制](sslocal://flow/file_open?url=%235-%E5%9F%BA%E7%A4%8E%E6%8C%87%E4%BB%A4%E8%88%87%E9%81%A0%E7%AB%AF%E6%8E%A7%E5%88%B6&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
6. [AI 應用部署實戰](sslocal://flow/file_open?url=%236-ai-%E6%87%89%E7%94%A8%E9%83%A8%E7%BD%B2%E5%AF%A6%E6%88%B0&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
   - 本機大模型 Ollama
   - AI 相機視覺辨識
   - 語音辨識與語音助手
7. [系統優化與效能調校](sslocal://flow/file_open?url=%237-%E7%B3%BB%E7%B5%B1%E5%84%AA%E5%8C%96%E8%88%87%E6%95%88%E8%83%BD%E8%AA%BF%E6%A0%A1&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
8. [常見問題與排除](sslocal://flow/file_open?url=%238-%E5%B8%B8%E8%A6%8B%E5%95%8F%E9%A1%8C%E8%88%87%E6%8E%92%E9%99%A4&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
9. [官方資源連結](sslocal://flow/file_open?url=%239-%E5%AE%98%E6%96%B9%E8%B3%87%E6%BA%90%E9%80%A3%E7%B5%90&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)

---

## 1. 樹梅派基本介紹
樹梅派（Raspberry Pi）是一款信用卡大小的單板電腦，由英國樹梅派基金會開發，最初用於推廣電腦科學教育，現已廣泛應用於物聯網、自動控制、機器學習、伺服器、智能裝置等領域。

### 特色
- 體積小、功耗低、價格親民
- 支援 Wi-Fi / Bluetooth / GPIO
- 內建完整 Linux 系統
- 可執行輕量級 AI 模型與電腦視覺任務

### 主流型號
- **Raspberry Pi 4 Model B**（4GB / 8GB）：入門首選
- **Raspberry Pi 5**：效能更強，適合 AI 與多工負載
- **Raspberry Pi Zero 2 W**：超微型 IoT 裝置

![樹梅派外觀示意圖](https://github.com/Hsi1996/Raspberry-Pi/blob/main/images/saaets/raspberry5.jpg)
*圖片來源：Raspberry Pi 官方*

---

## 2. 必備硬體清單
- 樹梅派主機板（Pi4 / Pi5 建議 4GB 以上）
- Micro SD 卡（16GB+，Class10 / A1 等級）
- 5V 3A USB-C 電源供應器
- 散熱片或風扇（AI 專案必備）
- 網路線 / 無線網路
- （選配）樹梅派官方 AI 相機模組
- （選配）麥克風、喇叭（語音助手使用）

---

## 3. 作業系統安裝（圖文步驟）
### 3.1 下載官方燒錄工具
使用 Raspberry Pi Imager 燒錄系統最穩定。

👉 [官方下載連結](https://www.raspberrypi.com/software/)

### 3.2 燒錄步驟
1. 開啟 Imager
2. 選擇作業系統：`Raspberry Pi OS (64-bit)`
3. 選擇 SD 卡儲存裝置
4. 點擊右上角「齒輪圖示」進階設定
   - 設定主機名稱
   - 開啟 SSH 
   - 設定使用者名稱與密碼
   - 填入 Wi-Fi 名稱與密碼
5. 點擊 `WRITE` 開始燒錄

![Imager 燒錄示意](https://www.raspberrypi.com/app/uploads/2021/10/Imager-Screenshot-1024x576.png)



---

## 4. 首次開機與基礎設定
1. 將 SD 卡插入樹梅派並開機
2. 等待開機完成
3. 使用終端機打以下程式碼確認樹梅派連到同一網域:
ping 樹梅派名稱@帳號名稱

4. 使用 SSH 遠端連線：
```bash
ssh 你的使用者名稱@登入帳號(EX:pi@xxxxxx)
(燒錄時請確認是否開啟ssh)



基礎系統更新:
sudo apt update
sudo apt upgrade -y

開啟進階設定工具:
sudo raspi-config


##開啟VNC Viewer

![步驟一](README.md/images/model.png)

![步驟二](https://github.com/Hsi1996/Raspberry-Pi/blob/main/images/saaets/open_vnc.png)

可開啟相機、擴充 SD 卡容量、調整記憶體分配、啟用 VNC 等。

下載安裝(CNV Viewer)[https://www.realvnc.com/en/connect/download/combined-mobile/]

 (VNC Viewer 無須登入)
![搜尋欄上打帳號](https://github.com/Hsi1996/Raspberry-Pi/blob/main/images/saaets/VNC.png)

![輸入帳號名稱及密碼](https://github.com/Hsi1996/Raspberry-Pi/blob/main/images/saaets/ID_password.png)

