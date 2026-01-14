# 臺科法律與生活考前測驗練習

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-success)](https://law-and-life.yijiun.me)

一個專為臺灣科技大學（NTUST）法律與生活課程設計的互動式考前練習網站。提供期中考與期末考範圍的填空題練習，幫助學生有效複習法律知識。

🔗 **線上體驗：** [law-and-life.yijiun.me](https://law-and-life.yijiun.me)

## ✨ 功能特色

- 📚 **期中考範圍**：涵蓋妨害司法、法律原則、刑法、醫療法等基礎法學概念
- 🎓 **期末考範圍**：涵蓋消保法、勞動基準法、國家賠償、定型化契約等生活應用法律
- 🔄 **題目隨機**：每次練習都會隨機打亂題目順序，增加記憶挑戰
- 🔥 **錯題特訓**：自動記錄答錯的題目，可針對弱點進行複習
- 📊 **即時反饋**：立即顯示答案正確與否，並統計分數
- 📱 **響應式設計**：支援手機、平板、電腦等各種裝置
- ⌨️ **鍵盤快捷鍵**：按 Enter 快速送出答案或進入下一題
- 🎨 **現代化介面**：使用 Neon 風格設計，提供流暢的使用體驗

## 🚀 快速開始

### 線上使用

直接訪問 [law-and-life.yijiun.me](https://law-and-life.yijiun.me) 即可開始使用，無需安裝任何軟體。

### 本地運行

1. **下載專案**
   ```bash
   git clone https://github.com/yijiunchin/ntust-law-and-life.git
   cd ntust-law-and-life
   ```

2. **開啟檔案**
   
   直接用瀏覽器開啟 `index.html` 檔案即可。
   
   或使用本地伺服器（推薦）：
   ```bash
   # 使用 Python
   python -m http.server 8000
   
   # 或使用 Node.js
   npx http-server
   ```
   
   然後在瀏覽器中訪問 `http://localhost:8000`

## 📖 使用說明

1. **選擇考試範圍**
   - 在首頁選擇「期中考範圍」或「期末考範圍」

2. **開始答題**
   - 閱讀題目，在填空處填入正確答案
   - 輸入答案後按「送出答案」或按鍵盤 Enter 鍵
   - 系統會立即顯示答案是否正確

3. **檢視成績**
   - 完成所有題目後，會顯示總分和答錯題數
   - 如果有答錯的題目，可以選擇「錯題特訓」進行複習

4. **錯題複習**
   - 系統會自動記錄答錯的題目
   - 點選「錯題特訓」可以針對錯題進行再次練習
   - 直到完全掌握為止

## 🛠️ 技術架構

### 前端技術

- **React 18**：使用 Hooks (useState, useEffect, useRef, useCallback)
- **Tailwind CSS**：快速建構響應式介面
- **Babel Standalone**：瀏覽器端 JSX 轉換
- **Noto Sans TC**：Google Fonts 繁體中文字型

### 特色實作

- **Fisher-Yates 洗牌演算法**：確保題目順序真正隨機
- **鍵盤事件處理**：支援 Enter 鍵快速操作
- **自動聚焦管理**：優化使用者輸入體驗
- **CSS 動畫**：包含 shake、fade-in 等流暢動畫效果
- **無需建置工具**：單一 HTML 檔案，開箱即用

## 📁 專案結構

```
ntust-law-and-life/
├── index.html          # 主應用程式（包含所有程式碼）
├── README.md           # 專案說明文件
├── LICENSE             # Apache 2.0 授權條款
└── CNAME              # GitHub Pages 自訂網域設定
```

## 📝 題庫說明

### 期中考題庫
- 題目數量：60 題
- 主題涵蓋：
  - 妨害司法公正
  - 法律原則
  - 正當防衛與緊急避難
  - 比例原則
  - 言論自由與妨害名譽
  - 權力分立與司法制度
  - 國民法官與參審陪審
  - 民法與未成年責任
  - 醫療責任
  - 消費者保護法（期中範圍）

### 期末考題庫
- 題目數量：75 題
- 主題涵蓋：
  - 消費者保護法
  - 定型化契約
  - 通訊交易
  - 國家賠償
  - 勞動基準法
  - 契約法律關係

## 🤝 貢獻指南

歡迎提交 Issue 或 Pull Request 來改進這個專案！

### 如何新增題目

1. 編輯 `index.html` 檔案
2. 找到對應的題庫陣列（`MIDTERM_QUESTIONS` 或 `FINAL_QUESTIONS`）
3. 按照以下格式新增題目：
   ```javascript
   { q: "題目內容，用 ______ 標示填空處。", a: "答案" }
   ```
4. 測試確認題目顯示正常
5. 提交 Pull Request

### 建議改進方向

- [ ] 新增更多題目
- [ ] 支援多種題型（選擇題、是非題等）
- [ ] 加入學習統計圖表
- [ ] 支援離線使用（PWA）
- [ ] 新增答題時間限制模式
- [ ] 匯出答題記錄功能

## 📄 授權條款

本專案採用 [Apache License 2.0](LICENSE) 授權。

## 👤 作者

**Yi Jiun Chin**

- Website: [github.yijiun.me](https://github.yijiun.me)
- GitHub: [@yijiunchin](https://github.com/yijiunchin)

## 🙏 致謝

- 感謝臺灣科技大學法律與生活課程提供學習內容
- 感謝所有使用者的回饋與建議

---

<p align="center">
  Made with ❤️ for NTUST Students
</p>