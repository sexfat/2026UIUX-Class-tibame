# 修改紀錄

## 2026-11-24

### Repo 設定
- 新增 `.gitignore`，忽略 `.agents/`、`.vscode/`、`AGENTS.md`。（`1a9d969`）
- 遠端網址改為新的 repo 名稱：`https://github.com/sexfat/2026UIUX-Class-tibame.git`（只改本機 git 設定，沒有 commit）。

### Unit 09：元件、樣式與設計系統概念
- **簡報 `Unit_09/slides.html`**：取代原本的空白版本，共 23 張，沿用 Unit 08 版型。（`fa48fdf`、`00e9a58`）
  - Part 1 樣式與設計權杖：Design Tokens、Primitive 與 Semantic 兩層命名（含可切換 Light / Dark 的示範卡片）、Figma Styles 與 Variables 比較、常見地雷
  - Part 2 元件與原子設計：五層架構、母元件與實例的繼承與覆寫、常見地雷
  - Part 3 變體與屬性控制：按鈕狀態矩陣、四種元件屬性、變體爆炸（48 → 24 ＋ Boolean）
  - Part 4 設計系統與交付：三大支柱、Auto Layout 與 CSS Flexbox / Tailwind 對照、Do / Don't 說明文件、常見地雷
  - 第 22 張本堂小結、第 23 張「範本與資源」（Figma 範本檔案與說明頁兩張連結卡片）
  - 課堂實作（「按鈕與表單元件系統化改造」60 分鐘）依需求暫不放入
- **Figma 範本插件 `Unit_09/figma-template/`**：（`fa48fdf`、`19599ae`）
  - `plugin/`（`manifest.json`、`code.js`）與 `unit09-design-system-plugin.zip`：在新的 Figma 檔案執行一次，建立 106 個 Variables（Primitive ＋ Semantic Light / Dark）、13 個文字樣式、陰影與 Focus 效果、漸層，以及 Foundations、Components（Icon、Button 45 個變體、Input Field、Badge、Booking Card）、Preview 頁面
  - `tokens/*.tokens.json`（W3C Design Tokens 格式）與 `tokens.css`：和插件同一份資料產生
  - 修正：component set 高度被固定為 100px；Booking Card 的 Badge 標籤改為「待補資料」；Button 改為每列 5 個 State 的表格排列
- **範本說明頁 `Unit_09/figma-template.html`**：範本內容與元件屬性表、直接複製 Figma 檔案的步驟、插件匯入步驟、匯入後確認清單、Token 檔案下載（附下載按鈕）。（`fa48fdf`、`ce63a72`）
- **Figma 範本檔案**：https://www.figma.com/design/J6gMn8zPlpR6gX62ZQMnRK（建在 Ateam 團隊；需將分享權限設為 Anyone with the link → can view，學生才能開啟並 Duplicate）

### Claude Skill：uiux-check
- 新增 `skills/uiux-check/`：依 Unit 06 十大易用性原則、Unit 07 完形心理學與 Laws of UX、Unit 08 介面視覺基礎審查 UI/UX，輸出依嚴重度排序的問題清單與修正建議。（`19599ae`）
  - `references/`：三個單元的規則與檢查問題
  - `scripts/contrast.py`：WCAG 對比度計算
  - `scripts/css_audit.py`：掃描 CSS 的間距、字級、行高、圓角與寫死色碼
- 新增 `skills/README.md`（Skill 結構說明、Claude Code 與網頁版安裝方式、使用範例）與 `skills/uiux-check.zip`。
- 同一份 Skill 也安裝在本機 `~/.claude/skills/uiux-check`。

### 主頁與 README
- `Unit_09/README.md`：單元目標與課程介紹依新簡報改寫（Tokens、原子設計、變體與屬性、設計系統交付、Figma 範本）。
- `index.html`：Unit 09 卡片加上「Figma 範本」按鈕；新增「Claude Skills」區塊與 uiux-check 卡片（安裝說明、下載 zip）。（`fa48fdf`、`00e9a58`）
- `README.md`：Unit 09 加上 Figma 範本連結；新增「Claude Skills」表格。（`fa48fdf`、`19599ae`）

### 待確認
- Figma 範本檔案的分享權限。
- 修正後的插件尚未在 Figma 桌面版實際執行過（已用模擬環境測試）。
- `skills/README.md` 中的 `npx degit` 指令與 Claude 網頁版上傳 Skill 的選單名稱尚未實測。
