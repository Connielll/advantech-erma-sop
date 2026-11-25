# Advantech eRMA 互動式技能樹操作指南 (Interactive Operational SOP)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-0066cc?style=flat&logo=github)](https://connielll.github.io/advantech-erma-sop/)
[![License](https://img.shields.io/badge/Advantech-Authorized%20Service%20Only-004280?style=flat)](https://erma.advantech.com.tw/Pro/Home/ServiceCenter)
[![Languages](https://img.shields.io/badge/i18n-zh--TW%20%7C%20EN%20%7C%20JA-10b981?style=flat)](#)

本專案將研華科技（Advantech）14 份傳統靜態維修 SOP 文件（包含客戶報修、倉儲點收、工程維修、料件領退與反查工具等），全面解構、重組並開發為一體化的**「遊戲化互動式技能樹（Interactive Skill Tree）」**。

透過明確的技能進度階梯、沉著精確的工業級界面（Unslopped Industrial Design）、實機操作影片與高解析度截圖引導，協助外部授權維修夥伴（如客戶端工程師）無痛自助完成 eRMA 各項系統流程，大幅降低日常溝通成本與誤操作率。

---

## 🌐 線上即時體驗 (Live Demo)

👉 **正式線上版網址**：**[https://connielll.github.io/advantech-erma-sop/](https://connielll.github.io/advantech-erma-sop/)**

* 支援任何電腦、平板與智慧型手機（跨瀏覽器 Chrome / Edge / Safari / Firefox）。
* 全球邊緣節點加速，無需安裝任何環境或依賴套件。

---

## 📖 如何在本機開啟與使用 (Local Usage)

如果您需要在離線環境或內部區域網路使用，亦可直接於本機執行：

### 方法一：直接雙擊開啟（免伺服器）
1. 下載或複製本專案資料夾至本機。
2. 直接使用 Chrome、Edge 等現代瀏覽器**連按兩下開啟 `index.html`** 即可開始操作。

### 方法二：透過本地輕量伺服器開啟（推薦）
若希望達到最流暢的視訊預載與字體渲染體驗，可使用終端機啟動本機伺服器：
```bash
# 在專案目錄下執行
python -m http.server 8080
```
開啟瀏覽器訪問：**`http://localhost:8080/`**

---

## 🎯 核心功能與介面操作說明

### 1. 角色路線篩選 (Track Filters)
頂部快速導覽列提供 4 大權限維度，一鍵聚焦所屬職責任務：
* **全覽技能樹 (All Skills)**：展開全部 18 個技能節點與 5 大推進階梯。
* **客戶報修路線 (Customer)**：帳號註冊開通、線上報修申請、DOA 急件處理。
* **倉庫點收路線 (Warehouse)**：貨故收件點收、外箱條碼列印、發貨出庫。
* **工程維修路線 (Engineering)**：工程初檢分流、BOM 物料領退、檢驗報廢、維修工時收費。
* **工具與管理路線 (Tools & Query)**：CTOS 反查、逾期催收、全球保固期與料號對照。

### 2. 多語系即時切換 (Trilingual Support)
點擊右上角語系按鈕，即可全頁無刷新即時切換：
* **繁中**（繁體中文）
* **EN**（English）
* **日本語**（Japanese）

### 3. 全域即時關鍵字搜尋 (Instant Search)
輸入 RMA 單號、產品序號（S/N）、料號或功能關鍵字，系統會以研華藍邊框即時聚焦符合條件之技能卡片。

### 4. 側滑操作卡片 (Slide-Over Drawer)
點選任一技能卡片即可喚出右側詳情面板：
* **工控鍵帽核心指令**：清晰標示介面中應點擊的按鈕（例如 `<Sign In / Register>`、`<LOGIN>`），避免尋找按鈕的挫折。
* **雙模式操作示範（Media Tabs）**：
  * **5s 動態演示**：自動循環播放真實系統操作視訊（MP4 / GIF）。
  * **靜態步驟截圖**：切換檢視官方高解析度原始紅框步驟註記。
* **全螢幕燈箱檢視（Lightbox）**：點擊示範畫面即可進入全螢幕燈箱模式循環觀看操作細節。
* **注意事項與專家提示**：提示 SAP 保固判定陷阱、條碼列印規格、權限申請等關鍵規則。

### 5. 技能掌握進度追蹤 (Mastery Tracking)
在抽屜底部點擊「**標記已掌握 (Mark as Mastered)**」，卡片將顯示綠色完成印記，頂部進度條會自動計算解鎖百分比（資料自動保存於本機 `localStorage`，重新整理不遺失）。

---

## 📂 目錄結構說明

```text
2026 AI RMA SOP建置/
├── index.html               # 核心單頁應用程式（含全套原生 SVG 圖標、三語系字典與邏輯）
├── README.md                # 專案操作說明文件
├── media/
│   ├── advantech-logo.svg   # 研華官方高解析度向量 SVG 標誌
│   ├── videos/              # 5~10 秒高畫質操作示範視訊 (MP4)
│   ├── gifs/                # 相容性動態示範圖片 (GIF)
│   └── screenshots/         # 14 份 SOP 擷取出的 150 張原始步驟圖片
├── source_docs/             # 原始 14 份 Word / PDF 操作規程文件庫
└── .github/                 # GitHub 自動化設定與部署設定檔
```

---

## 🎨 設計哲學：Unslopped Industrial Craft

本介面嚴格遵循 [`unslop`](https://github.com/heydamir/unslop) 設計標準：
* **沉靜的工控背景（Quiet Chrome）**：消除浮誇的 AI 漸層光暈與紫青發光，採用硬體石墨 Neutral Ramp（`#0c0e14` / `#151924` / `#1b212f`）。
* **極簡工程線條圖標**：全面捨棄一般 Emoji，改採 18px 輕量化統一筆觸之向量線條圖標（Lucide 風格）。
* **研華品牌專屬識別**：僅在焦點動作、狀態指示選用研華官方深藍（`#004280` / `#0066cc`）與官方向量標誌。
* **嚴謹排版與等寬數值**：遵循 4px 階梯與巢狀圓角法則，數值全面啟用 `tabular-nums`。

---

## 🔄 後續新增動態示範指引

若您需要為後續技能節點（#03～#18）補充動態錄影：
1. 錄製 5~10 秒之操作短片（建議解析度約 800~1000px 寬，15~20 fps）。
2. 將 `.mp4` 存入 `media/videos/`（如 `03_child_rma.mp4`）。
3. 執行 Git 提交與推送：
   ```bash
   git add .
   git commit -m "feat: add demo video for skill #03"
   git push
   ```
4. GitHub Pages 將在 1 分鐘內自動建置並全球同步上線。

---

*版權聲明：本指南內容依據 Advantech eRMA Global Service Policy 編製，供授權服務中心與合作夥伴內部教育訓練使用。*
