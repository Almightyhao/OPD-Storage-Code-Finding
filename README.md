# 🧾 Storage Code Finder

門診藥品儲位查詢工具（**0912 TSGH 儲位更新版**）  

> 由 Excel 自動載入的輕量查詢系統，可即時搜尋藥品儲位、庫存區位置。  

---

## 🚀 功能特色

- 🔄 **自動讀取 GitHub main 分支**的最新 Excel (`Storage Code.xlsx`)
- 🔍 **支援模糊搜尋與部分關鍵字**（例如輸入「阿奇」即可找到「阿奇黴素」）
- 📋 顯示對應欄位：**藥品名稱、儲位區、庫存區**
- 🧩 **勾選暫存清單功能**：可將查詢結果勾選加入下方清單，暫存後再查看或匯出 CSV
- 💾 **LocalStorage 保存勾選狀態**，重新整理頁面不會消失
- 💡 完全前端執行，無須伺服器、無資料外傳

---

## 💡 使用方式

1. 開啟網頁  
   👉 [**Storage Code Finder**](https://almightyhao.github.io/Storage-Code-Finding/)

2. 在輸入框輸入藥名（完整或部分關鍵字）

3. 點選 **「重新整理」** 可重新抓取最新 Excel

4. 可在搜尋結果左側勾選藥品以建立暫存清單：
   - 勾選 → 加入清單  
   - 取消勾選 → 移除清單  
   - 清單可匯出為 CSV 或全部清空  

---

## 📂 Excel 更新說明

- Excel 檔案名稱：`Storage Code.xlsx`  
- 檔案位置：**repo 根目錄**
- 更新方式：上傳新版本至 `main` 分支 → 網頁自動抓取最新版本  

---

## 🧭 技術架構

| 模組 | 功能 | 來源 |
|------|------|------|
| [SheetJS (xlsx)](https://github.com/SheetJS/sheetjs) | 解析 Excel | CDN |
| [Fuse.js](https://fusejs.io/) | 模糊搜尋引擎 | CDN |
| HTML + CSS + JS | 前端顯示介面 | 自製輕量版 |

---

## 🧩 版本紀錄

| 版本 | 日期 | 說明 |
|------|------|------|
| **0912** | 2025/09/12 | TSGH 儲位更新版，支援自動載入 main 分支 Excel 與模糊搜尋 |
| **1017** | 2025/10/17 | 新增「勾選暫存清單」功能，可在下方清單中查看或匯出勾選藥品 |

---

📦 **Repository:** [github.com/Almightyhao/Storage-Code-Finding](https://github.com/Almightyhao/Storage-Code-Finding)
