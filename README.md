# StoreSmart 智慧收納

<p align="center">
  <img src="icon-192.png" width="80" alt="StoreSmart">
</p>

AI 驅動的智慧收納系統 — 拍照或使用 Google Lens 截圖，自動辨識物品、估算體積、分配收納位置。

## 功能

- 📷 **拍照建檔** — 拍照後 AI 自動辨識物品名稱、品牌、規格
- 🔍 **Google Lens 截圖** — 支援 AI 模式和全部模式的截圖解析
- 📦 **智慧分袋** — 根據物品特徵標籤自動歸類，同類物品放同一袋
- 📏 **體積估算** — AI 自動估算物品體積，袋子容量即時追蹤
- 🏠 **自訂收納位置** — 定義家中實際收納點 + 袋容量 + 提示詞
- 🔄 **批次建檔** — 一次選多張照片，全自動辨識建檔
- 🔎 **關鍵字搜尋** — 找到物品就知道它在哪個袋子、哪個位置
- ☁️ **Firebase 同步**（選填）— 多裝置共用同一個收納資料庫

## 使用方式

1. 開啟 [StoreSmart](https://你的帳號.github.io/storesmart/)
2. 輸入 Anthropic API Key
3. 設定收納位置（或使用預設的書房書櫃/車庫層架/廚房層架）
4. 開始拍照建檔！

## 技術架構

- **單一 HTML 檔案**，無需後端伺服器
- **Claude Sonnet 4** 做物品辨識、分類、體積估算
- **localStorage** 儲存物品資料（可選 Firebase Firestore 同步）
- **PWA** 支援，可加到手機主畫面使用

## 部署

本專案是純前端 HTML，部署到 GitHub Pages：

```bash
git clone https://github.com/你的帳號/storesmart.git
# 檔案已包含 index.html, manifest.json, icons
# 直接啟用 GitHub Pages (Settings > Pages > main branch)
```

## 授權

MIT License
