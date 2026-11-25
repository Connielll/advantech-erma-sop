# eRMA 系統操作指南：局部放大 GIF 動圖錄製清單 (MEDIA_TODO.md)

本文件列出知識庫中所有建議錄製 **5~10 秒局部放大 GIF / 螢幕錄影動圖** 的步驟清單、目標存放路徑、檔案命名規範與精確的滑鼠游標操作腳本。

---

## 快速使用說明 (How It Works)

1. **儲存路徑**：錄製完成的 `.gif` 或 `.mp4` 檔案請直接放置於：
   ```
   docs/public/media/gifs/
   ```
2. **自動載入與熱替換**：
   - 網頁組件採用自動優先原則：只要 `docs/public/media/gifs/[檔名].gif` 存在，前端網頁會**立即自動以無聲循環動圖取代預設截圖**（`autoplay loop muted playsinline`）。
   - 若檔案尚未錄製，網頁會自動優雅降級（Fallback）顯示原始 Word/PPTX 中提取的真實截圖與錄製腳本提示框。
3. **建議錄製規格**：
   - **格式**：`.gif` 或 `.mp4` (H.264，體積更小更流暢)
   - **解析度**：800x500 ~ 1280x720（聚焦於關鍵操作區域或按鈕附近，建議局部放大 120%~150%）
   - **時長**：5 ~ 10 秒（單一操作循環）
   - **幀率 (FPS)**：15 ~ 24 FPS
   - **游標提示**：啟用滑鼠點擊黃色光圈或點擊波紋效果，讓使用者一眼看清點擊位置。

---

## 模組一：快速入門與總覽 (01-getting-started)

| 步驟編號 | 對應頁面 | 目標動圖檔名 | 錄製時間 | 畫面焦點與游標動作腳本 (Recording Script) |
|---|---|---|:---:|---|
| **00-REG-01** | `01-getting-started/registration.md` (Step 1) | `00_registration_step_01.gif` | 5s | 滑鼠游標移動至右上角，點擊 **Sign In / Register** 按鈕，彈出登入選單。 |
| **00-REG-02** | `01-getting-started/registration.md` (Step 2) | `00_registration_step_02.gif` | 5s | 在登入彈出視窗底部，點擊 **Register** 超連結跳轉至註冊會員中心。 |
| **00-REG-03** | `01-getting-started/registration.md` (Step 3) | `00_registration_step_03.gif` | 6s | 游標展示右上角語言選單切換至繁中/日文，並提示**避開社群快速登入按鈕**。 |
| **00-REG-04** | `01-getting-started/registration.md` (Step 4) | `00_registration_step_04.gif` | 7s | 快速填寫真實姓名、公司、Email，勾選隱私協議後點擊 **Submit**。 |
| **00-REG-05** | `01-getting-started/registration.md` (Step 5) | `00_registration_step_05.gif` | 5s | 開啟驗證信件並點擊信件內藍色 **Verify Now** 按鈕完成信箱驗證。 |
| **00-LOG-01** | `01-getting-started/login.md` (Step 1) | `00_login_step_01.gif` | 5s | 首頁右上角點擊 **Sign in / Register**，展示標準登入對話框彈出。 |
| **00-LOG-02** | `01-getting-started/login.md` (Step 2) | `00_login_step_02.gif` | 6s | 輸入帳號密碼，於語言選單切換至 English / 繁體中文，點擊 **LOGIN**。 |
| **00-LOG-03** | `01-getting-started/login.md` (Step 3) | `00_login_step_03.gif` | 8s | 展示登入後主畫面，游標環顧頂部搜尋列、個人資訊與左側功能模組樹。 |
| **00-LOG-04** | `01-getting-started/login.md` (Step 4) | `00_login_step_04.gif` | 6s | 點擊登入框內 **Forget Password**，輸入 Email 申請重置密碼信。 |
| **00-SCH-01** | `01-getting-started/search-and-tracking.md` (Step 1) | `00_search_step_01.gif` | 5s | 於頂部搜尋欄鍵入 RMA 單號，按 Enter 彈出即時搜尋結果清單。 |
| **00-SCH-02** | `01-getting-started/search-and-tracking.md` (Step 2) | `00_search_step_02.gif` | 5s | 點擊搜尋結果中的藍色 **RMA No** 超連結，進入案件詳情總覽頁。 |
| **00-SCH-03** | `01-getting-started/search-and-tracking.md` (Step 3) | `00_search_step_03.gif` | 7s | 游標指針依序掃過流程圖：Request ➔ Receive ➔ Repair ➔ Ship 深藍色/灰色外框。 |
| **00-SCH-04** | `01-getting-started/search-and-tracking.md` (Step 4) | `00_search_step_04.gif` | 6s | 點擊流程圖中央的 **Repair** 快捷鍵，展開更換零件料號、工時與照片。 |
| **00-SCH-05** | `01-getting-started/search-and-tracking.md` (Step 5) | `00_search_step_05.gif` | 6s | 切換至 **Report** 頁籤，點擊 **Export PDF** 自動下載正式維修報告 PDF。 |

---

## 模組二：客戶端送修流程 (02-customer-rma)

| 步驟編號 | 對應頁面 | 目標動圖檔名 | 錄製時間 | 畫面焦點與游標動作腳本 (Recording Script) |
|---|---|---|:---:|---|
| **01-REQ-01** | `02-customer-rma/rma-request.md` (Step 1) | `01_customer_rma_step_01.gif` | 5s | 點擊左側選單 **Customer** ➔ 展開點擊 **RMA Request** 開啟申請表。 |
| **01-REQ-02** | `02-customer-rma/rma-request.md` (Step 2) | `01_customer_rma_step_02.gif` | 6s | 於 Customer 頁籤確認聯絡人並修改實體回寄地址（Ship-To Address）。 |
| **01-REQ-03** | `02-customer-rma/rma-request.md` (Step 3) | `01_customer_rma_step_03.gif` | 6s | 切換至 Product 頁籤，鍵入序號按 Tab，系統自動彈出料號與保固。 |
| **01-REQ-04** | `02-customer-rma/rma-request.md` (Step 4) | `01_customer_rma_step_04.gif` | 7s | 依序下拉選擇 Category、Sub-Category，勾選 Symptom 故障現象代碼。 |
| **01-REQ-05** | `02-customer-rma/rma-request.md` (Step 5) | `01_customer_rma_step_05.gif` | 6s | 點擊 **+ Add Item**，展示第二筆產品新增至下方列表。 |
| **01-REQ-06** | `02-customer-rma/rma-request.md` (Step 6) | `01_customer_rma_step_06.gif` | 5s | 點擊右下角綠色 **Submit**，彈出確認視窗並生成正式 RMA 單號。 |
| **01-LBL-01** | `02-customer-rma/batch-and-label.md` (Step 1) | `01_customer_rma_step_07.gif` | 5s | 點擊 **Download Excel Template** 下載標準批次申請 Excel 範本。 |
| **01-LBL-02** | `02-customer-rma/batch-and-label.md` (Step 2) | `01_customer_rma_step_08.gif` | 6s | 展示在 Excel 中貼上 10 筆產品序號與問題代碼並存檔。 |
| **01-LBL-03** | `02-customer-rma/batch-and-label.md` (Step 3) | `01_customer_rma_step_09.gif` | 7s | 點擊 Choose File 選取檔案並點擊 Upload，系統逐筆校驗綠色勾選通過。 |
| **01-LBL-04** | `02-customer-rma/batch-and-label.md` (Step 4) | `01_customer_rma_step_10.gif` | 6s | 點擊 **Print Shipping Label**，彈出含 RMA 條碼之外箱標籤預覽並列印。 |
| **01-LBL-05** | `02-customer-rma/batch-and-label.md` (Step 5) | `01_customer_rma_step_11.gif` | 5s | 展示外箱包裝平整黏貼 RMA Shipping Label 之標準實物示意。 |

---

## 模組三：核心維修四大關卡 (03-core-lifecycle)

| 步驟編號 | 對應頁面 | 目標動圖檔名 | 錄製時間 | 畫面焦點與游標動作腳本 (Recording Script) |
|---|---|---|:---:|---|
| **02-AIO-01** | `03-core-lifecycle/all-in-one.md` (Step 1) | `02_stage_allinone_step_01.gif` | 5s | 點擊左選單 **Stage** ➔ **All In One**，載入整合看板。 |
| **02-AIO-02** | `03-core-lifecycle/all-in-one.md` (Step 2) | `02_stage_allinone_step_02.gif` | 6s | 在 RMA/Order No 欄位輸入單號點擊 Search，即時載入四階段狀態。 |
| **02-AIO-03** | `03-core-lifecycle/all-in-one.md` (Step 3) | `02_stage_allinone_step_03.gif` | 8s | 同一頁面中先展開 Receive 確認收件，再展開 Repair 填報維修動作。 |
| **02-AIO-04** | `03-core-lifecycle/all-in-one.md` (Step 4) | `02_stage_allinone_step_04.gif` | 5s | 點擊右下角 **Save All**，系統彈出保存成功通知。 |
| **02-RCV-01** | `03-core-lifecycle/receive.md` (Step 1) | `02_stage_receive_step_01.gif` | 5s | 點選左側選單 **Stage** ➔ **Receive** 進入收件工作台。 |
| **02-RCV-02** | `03-core-lifecycle/receive.md` (Step 2) | `02_stage_receive_step_02.gif` | 5s | 條碼槍刷讀條碼，畫面上自動載入型號、序號與客戶資訊。 |
| **02-RCV-03** | `03-core-lifecycle/receive.md` (Step 3) | `02_stage_receive_step_03.gif` | 6s | 檢視外箱破損，於 Package Status 選擇 Damaged 並上傳外箱照片。 |
| **02-RCV-04** | `03-core-lifecycle/receive.md` (Step 4) | `02_stage_receive_step_04.gif` | 6s | 檢查保固標籤與機殼外觀，勾選 Appearance Status。 |
| **02-RCV-05** | `03-core-lifecycle/receive.md` (Step 5) | `02_stage_receive_step_05.gif` | 6s | 在 Accessories Checklist 勾選隨附的電源線與變壓器。 |
| **02-RCV-06** | `03-core-lifecycle/receive.md` (Step 6) | `02_stage_receive_step_06.gif` | 5s | 點擊藍色 **Receive** 按鈕確認收件，流程圖 Receive 轉為深藍色。 |
| **02-RPR-01** | `03-core-lifecycle/repair.md` (Step 1) | `02_stage_repair_step_01.gif` | 5s | 進入 **Stage** ➔ **Repair**，鍵入單號搜尋打開詳細維修編輯介面。 |
| **02-RPR-02** | `03-core-lifecycle/repair.md` (Step 2) | `02_stage_repair_step_02.gif` | 6s | 查看客戶送修描述，並於 Verified Problem 欄位記錄現場重現狀況。 |
| **02-RPR-03** | `03-core-lifecycle/repair.md` (Step 3) | `02_stage_repair_step_03.gif` | 7s | 選擇 Replace Component，輸入位置 U12 與料號，點擊 Add Action。 |
| **02-RPR-04** | `03-core-lifecycle/repair.md` (Step 4) | `02_stage_repair_step_04.gif` | 5s | 在 **Working Minutes** 欄位鍵入實施工時（如 45 分鐘）並暫存。 |
| **02-RPR-05** | `03-core-lifecycle/repair.md` (Step 5) | `02_stage_repair_step_05.gif` | 7s | 點擊 Upload Attachment 上傳零件燒毀特寫與修復後照片。 |
| **02-RPR-06** | `03-core-lifecycle/repair.md` (Step 6) | `02_stage_repair_step_06.gif` | 6s | 將 **Complete** 切換為 **Y**，點擊 **Submit** 結案進入出貨關卡。 |
| **02-SHP-01** | `03-core-lifecycle/ship.md` (Step 1) | `02_stage_ship_step_01.gif` | 5s | 點擊左側選單 **Stage** ➔ **Ship** 載入待出貨面板。 |
| **02-SHP-02** | `03-core-lifecycle/ship.md` (Step 2) | `02_stage_ship_step_02.gif` | 6s | 篩選 Repair Status = Repaired，點擊 Search 列出所有可出貨案件。 |
| **02-SHP-03** | `03-core-lifecycle/ship.md` (Step 3) | `02_stage_ship_step_03.gif` | 6s | 輸入出貨發票號碼，於 Charge To 下拉選單選擇計費服務中心。 |
| **02-SHP-04** | `03-core-lifecycle/ship.md` (Step 4) | `02_stage_ship_step_04.gif` | 6s | 下拉選擇 DHL，輸入 10 碼快遞單號，確認回寄地址無誤。 |
| **02-SHP-05** | `03-core-lifecycle/ship.md` (Step 5) | `02_stage_ship_step_05.gif` | 6s | 勾選案件並點擊 **Ship / Close Case**，系統提示成功出貨並封存。 |
| **03-CHD-01** | `03-core-lifecycle/child-rma.md` (Step 1) | `03_child_rma_step_01.gif` | 5s | 點選左選單 **Child** ➔ **Child RMA Lookup** 開啟子案件控制台。 |
| **03-CHD-02** | `03-core-lifecycle/child-rma.md` (Step 2) | `03_child_rma_step_02.gif` | 6s | 設定日期區間與發起站點代碼，點擊 Search 查詢後送工廠清單。 |
| **03-CHD-03** | `03-core-lifecycle/child-rma.md` (Step 3) | `03_child_rma_step_03.gif` | 6s | 點擊 Child RMA 單號連結，查閱總部工廠工程師的處置與發料記錄。 |
| **03-CHD-04** | `03-core-lifecycle/child-rma.md` (Step 4) | `03_child_rma_step_04.gif` | 7s | 在母案中核銷收到修復零件，裝回機箱並執行組裝再測試。 |

---

## 模組四：物料管理與調度 (04-material)

| 步驟編號 | 對應頁面 | 目標動圖檔名 | 錄製時間 | 畫面焦點與游標動作腳本 (Recording Script) |
|---|---|---|:---:|---|
| **04-MAT-01** | `04-material/material-request.md` (Step 1) | `04_material_step_01.gif` | 6s | 在 Repair 案件中點擊 Product Name 藍色連結，彈出層級式 BOM 清單。 |
| **04-MAT-02** | `04-material/material-request.md` (Step 2) | `04_material_step_02.gif` | 6s | 在 BOM 中搜尋料號，點選 Apply 圖示，輸入數量 1 並填寫備註。 |
| **04-MAT-03** | `04-material/material-request.md` (Step 3) | `04_material_step_03.gif` | 6s | 在 Part Location 欄位鍵入 C105，點擊搜尋反查原廠料號。 |
| **04-MAT-04** | `04-material/material-request.md` (Step 4) | `04_material_step_04.gif` | 6s | 進入 Material Application，鍵入料號、選擇架位並點擊 Add。 |
| **04-MAT-05** | `04-material/material-request.md` (Step 5) | `04_material_step_05.gif` | 5s | 在 My Application 查看領料單狀態（Open 或 Waiting ATP）。 |
| **04-DSP-01** | `04-material/dispatch-and-stock.md` (Step 1) | `04_material_step_10.gif` | 6s | 倉庫標籤機收到領料指令，自動印出含有 QR Code 的領料貼紙。 |
| **04-DSP-02** | `04-material/dispatch-and-stock.md` (Step 2) | `04_material_step_11.gif` | 6s | 倉管依貼紙上之 Bin Location 架位揀料並核對包裝標籤。 |
| **04-DSP-03** | `04-material/dispatch-and-stock.md` (Step 3) | `04_material_step_12.gif` | 5s | 掃描槍刷讀貼紙上的 QR Code，狀態瞬間切換為 D-Waiting DOC。 |
| **04-DSP-04** | `04-material/dispatch-and-stock.md` (Step 4) | `04_material_step_13.gif` | 6s | 於 To Do List 查閱缺料 Ordering 項目及原廠預計到貨日 (ATP)。 |

---

## 模組五：實用工具與設定 (05-tools)

| 步驟編號 | 對應頁面 | 目標動圖檔名 | 錄製時間 | 畫面焦點與游標動作腳本 (Recording Script) |
|---|---|---|:---:|---|
| **05-WAR-01** | `05-tools/warranty-lookup.md` (Step 1) | `05_warranty_lookup_step_01.gif` | 5s | 點擊左選單 **ToolsLookup** ➔ **Warranty Lookup** 開啟查詢頁面。 |
| **05-WAR-02** | `05-tools/warranty-lookup.md` (Step 2) | `05_warranty_lookup_step_02.gif` | 5s | 勾選 By Barcode，輸入主機板序號並點擊 Search 放大鏡圖示。 |
| **05-WAR-03** | `05-tools/warranty-lookup.md` (Step 3) | `05_warranty_lookup_step_03.gif` | 7s | 游標指向 Shipping Date、Warranty 到期日與工單 M/O 連結。 |
| **05-CTO-01** | `05-tools/ctos-lookup.md` (Step 1) | `05_ctos_lookup_step_01.gif` | 5s | 點擊左側 **ToolsLookup** ➔ **CTOS Lookup** 進入組裝反查介面。 |
| **05-CTO-02** | `05-tools/ctos-lookup.md` (Step 2) | `05_ctos_lookup_step_02.gif` | 6s | 輸入整機序號點擊搜尋，調閱 SFIS 車間條碼記錄。 |
| **05-CTO-03** | `05-tools/ctos-lookup.md` (Step 3) | `05_ctos_lookup_step_03.gif` | 7s | 滾動 Key Parts Info 列表，核對 CPU、主機板、RAM 之實體序號。 |
| **05-CTO-04** | `05-tools/ctos-lookup.md` (Step 4) | `05_ctos_lookup_step_04.gif` | 7s | 比對出貨廠區 Plant Location 為 TWH1 且 Bill To 為海外分公司（判定為 Internal DOA）。 |
| **05-REM-01** | `05-tools/stage-reminder.md` (Step 1) | `05_stage_reminder_step_01.gif` | 5s | 點選 **Tools (Setting)** ➔ **Stage Reminder**，點擊 Create 按鈕。 |
| **05-REM-02** | `05-tools/stage-reminder.md` (Step 2) | `05_stage_reminder_step_02.gif` | 6s | 選取 RMA NO，輸入單號，並指定在 Receive 關卡觸發提醒。 |
| **05-REM-03** | `05-tools/stage-reminder.md` (Step 3) | `05_stage_reminder_step_03.gif` | 6s | 填寫提醒警示文字「品質異常特檢件，收件後送 3F 品保」，點擊 Create。 |
| **05-REM-04** | `05-tools/stage-reminder.md` (Step 4) | `05_stage_reminder_step_02.gif` | 5s | 於提醒清單中點擊垃圾桶圖示刪除解除該案件之攔截提醒。 |

---

> 💡 **維護建議**：只要錄好上述對應檔名的 GIF，放置到 `docs/public/media/gifs/` 資料夾中，重新整理網頁就會自動載入，完全不需要修改任何程式碼或 Markdown 文件！
