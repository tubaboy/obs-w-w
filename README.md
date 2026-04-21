# 🌦️ OBS Weather Widget (obs-w-w)

一個專為 OBS 直播設計的輕量化天氣層疊（Overlay）工具。無需資料庫、無需註冊 API Key，透過網址參數即可即時產生美觀的天氣資訊。

![Language](https://img.shields.io/badge/language-HTML%2FJS-orange)
![License](https://img.shields.io/badge/license-MIT-blue)
![Platform](https://img.shields.io/badge/platform-OBS%20Studio-blueviolet)

## 🚀 快速開始

直接前往產生器頁面設定你的 Widget：
👉 **[即時產生器連結](https://tubaboy.github.io/obs-w-w/)**

## ✨ 特色功能

- 🛠️ **雙架構設計**：分離設定面板 (`index.html`) 與直播 Widget (`widget.html`)，確保 OBS 畫面純淨無偏移。
- 📍 **精確定位**：內建自動完成搜尋功能，直接鎖定經緯度，解決城市名稱模糊匹配的問題。
- 📊 **雙版型支援**：
  - **長形 (Rectangular)**：適合放在畫面頂部或底部的資訊條。
  - **方形 (Square)**：適合側邊欄或資訊板塊。
- 🔄 **自動更新**：
  - 每 **1 分鐘** 自動更新系統時鐘。
  - 每 **15 分鐘** 自動抓取最新天氣資料（包含當前溫度、降雨機率等）。
- 🎨 **現代視覺**：深色模式配上玻璃擬態（Glassmorphism）風格，支援自訂背景透明度。
- ⚡ **極速加載**：純前端渲染，無後端負擔，使用 Open-Meteo 免費 API。

## 📺 OBS 設定說明

1. 在產生器中設定好你的地點與樣式。
2. 複製產生的 `widget.html?...` 連結。
3. 在 OBS 中新增「**瀏覽器**」來源。
4. 根據版型設定對應的寬高：
   - **長形**：寬度 `900` / 高度 `180`
   - **方形**：寬度 `400` / 高度 `480`
5. 勾選「**當來源不顯示時關閉瀏覽器**」（選填，建議保持開啟以維持背景更新）。

## 🛠️ 技術細節

- **資料來源**：[Open-Meteo API](https://open-meteo.com/) (WMO 規範)
- **圖示庫**：[Lucide Icons](https://lucide.dev/)
- **字體**：Fira Code, Fira Sans
- **架構**：Vanilla JavaScript / CSS Grid & Flexbox

## 📝 授權協議

本專案採用 [MIT License](LICENSE) 授權。歡迎隨時 Fork 或是提出 PR！

---
*Created by [tubaboy](https://github.com/tubaboy) with 💡*
