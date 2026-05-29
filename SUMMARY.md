# 專案開發工作摘要 (Project Development Summary) 📝

本文件摘要記錄了 **2026-05-29** 針對個人網頁專案所完成的全部開發與配置工作。

---

## 🛠️ 完成的工作內容

### 1. 🌈 精美動態首頁開發 (`index.html`)
建立了一個極具現代視覺美感與即時動態反饋的單頁式 Web 應用程式：
* **視覺美學 (Aesthetics)**：
  - 採用前衛的**玻璃擬態 (Glassmorphism)** 卡片設計，具有背景高斯模糊 (`backdrop-filter`) 與細緻的邊框微光。
  - 設計了可持續平滑流動的暗色系**漸變背景 (Fluid Gradient)**，並搭配兩顆帶有浮動與微縮放動畫的模糊環境光暈粒子（Indigo & Pink）。
  - 為卡片加入動態懸停位移 (3D Lift) 效果與擴散陰影，創造極佳的互動體驗。
* **即時時鐘引擎 (JavaScript)**：
  - 整合動態時間更新，每秒即時計算並同步顯示系統時間。
  - 自動偵測使用者所在時區（例如：台北標準時間）。
  - 格式化輸出符合繁體中文語系的日期格式（例：`2026 年 05 月 29 日 星期五`）。
* **字型與排版**：
  - 整合 Google Fonts，選用高質感的英文字型 **Outfit** 與中文字型 **Noto Sans TC**。
  - 對時鐘數字採用等寬字型設定 (`tabular-nums`)，防止時間跳動時文字產生抖動。

### 2. ⚙️ Git 倉庫初始化與使用者配置
為專案建立了標準的版本控制系統：
* **倉庫初始化**：於專案目錄執行 `git init`，並依據現代 GitHub 標準將預設分支更名為 `main`。
* **使用者資訊配置**：
  - 姓名設定：`MuYi`
  - 電子信箱：`chenmy1989@gmail.com`
* **遠端關聯**：將遠端 origin URL 關聯至：`https://github.com/MuYiLiu1989/L2-DIC1-github.git`

### 3. 📂 專案核心文件建立與過濾
* **`.gitignore`**：建立專案過濾檔，自動忽略 Windows 縮圖快取（`Thumbs.db`）、VS Code 及 IDE 設定檔（`.vscode/`, `.idea/`），保持倉庫乾淨。
* **`README.md`**：撰寫排版美觀、中英對照的專案說明文件，內容包含特色介紹、視覺預覽說明、本地啟動指南、使用的技術棧。
* **動態 Live Demo 整合**：於 README 主標題下方置入即時預覽網址：`https://muyiliu1989.github.io/L2-DIC1-github/`

---

## 📂 專案檔案結構清單

```text
L2 DIC1=github/
├── .git/               # Git 版本控制資料夾
├── .gitignore          # 忽略清單文件
├── index.html          # 首頁核心代碼 (含 CSS 樣式與 JS 時鐘邏輯)
├── README.md           # 專案詳細說明與 Live Demo 連結
└── SUMMARY.md          # 本工作摘要報告文件 (本檔案)
```

---

## 🕒 本地 Git 提交歷史 (Commit History)

目前本地倉庫已有三個乾淨且具描述性的 commits：
1. **`a890e60` Initial commit**
   - 提交了 `.gitignore` 與 `index.html` 的初始代碼。
2. **`6c7aad2` Add README.md with project overview**
   - 提交了專案的說明文件。
3. **`b1aa5bb` Add Live Demo link to README.md**
   - 提交了整合 Live Demo 連結後的更新版 README.md。

---

## 🚀 後續推送到 GitHub 指南

一旦您在 GitHub 上創立了同名的 **`L2-DIC1-github`** 公開/私有倉庫後，只需在終端機輸入以下指令即可將全部程式碼推送到雲端：

```bash
# 推送 main 分支程式碼至 GitHub 並設定上游追蹤
git push -u origin main
```
