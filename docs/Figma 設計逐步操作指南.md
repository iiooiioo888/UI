# Figma 設計逐步操作指南

> 檢查清單格式，完成一項勾選一項，方便邊做邊檢查。

---

## 📋 使用說明

1. 打開 Figma（https://figma.com）
2. 創建新文件：「年結表計算器 UI 設計」
3. 按照以下步驟逐步操作
4. 完成一項勾選一項 ✅

---

## 第一步：創建頁面結構（5 分鐘）

### 創建 Pages
- [ ] 右側面板 → Pages → 「+」
- [ ] 創建以下 9 個頁面：
  - [ ] `📄 Cover`（封面頁）
  - [ ] `📄 Design System`（設計系統）
  - [ ] `📄 Components`（組件庫）
  - [ ] `📄 首頁`
  - [ ] `📄 查詢輸入頁`
  - [ ] `📄 結果展示頁`
  - [ ] `📄 管理後台`
  - [ ] `📄 系統管理`
  - [ ] `📄 Prototype`（交互原型）

### 設置 Cover 頁
- [ ] 切換到 Cover 頁
- [ ] 創建 Frame（1920x1080）
- [ ] 添加背景（填充：Gray-50）
- [ ] 添加項目名稱（H1，居中）
- [ ] 添加版本號和日期
- [ ] 添加設計狀態標籤

---

## 第二步：創建設計系統（30 分鐘）

### 2.1 創建 Color Styles（15 分鐘）

#### 切換到 Design System 頁
- [ ] 創建 Frame（1200x800）
- [ ] 命名為「Colors」

#### 創建主色
- [ ] 繪製矩形（80x80）
- [ ] 填充：`#1890ff`
- [ ] 右側面板 → Styles → 「+」
- [ ] 命名：`Primary / Blue - 500`
- [ ] 重複創建：
  - [ ] `Primary / Blue - 400`（`#40a9ff`）
  - [ ] `Primary / Blue - 600`（`#096dd9`）

#### 創建功能色
- [ ] 綠色：`Success / Green - 500`（`#52c41a`）
- [ ] 黃色：`Warning / Yellow - 500`（`#faad14`）
- [ ] 紅色：`Error / Red - 500`（`#f5222d`）

#### 創建中性色
- [ ] `Neutral / Gray - 850`（`#262626`）
- [ ] `Neutral / Gray - 600`（`#595959`）
- [ ] `Neutral / Gray - 300`（`#d9d9d9`）
- [ ] `Neutral / Gray - 100`（`#f5f5f5`）
- [ ] `Neutral / Gray - 50`（`#fafafa`）

**檢查**：
- [ ] 所有 Color Styles 已創建（共 11 個）
- [ ] 命名規範正確
- [ ] 顏色預覽正確

---

### 2.2 創建 Text Styles（10 分鐘）

#### 創建標題樣式
- [ ] 使用文字工具（T）創建文本
- [ ] 設置：Microsoft YaHei, 24px, 600
- [ ] 右側面板 → Text Styles → 「+」
- [ ] 命名：`Heading / H1 - 24px`
- [ ] 重複創建：
  - [ ] `Heading / H2 - 20px`
  - [ ] `Heading / H3 - 16px`

#### 創建正文樣式
- [ ] `Body / Large - 16px`（Microsoft YaHei, 400）
- [ ] `Body / Regular - 14px`
- [ ] `Body / Small - 12px`

#### 創建數字樣式
- [ ] `Number / Amount - 14px`（Segoe UI, 400）
- [ ] `Number / Large Amount - 20px`（Segoe UI, 600）

**檢查**：
- [ ] 所有 Text Styles 已創建（共 8 個）
- [ ] 字體設置正確
- [ ] 樣式預覽正確

---

### 2.3 創建 Spacing 系統（5 分鐘）

#### 創建間距參考
- [ ] 創建 Frame（800x400）
- [ ] 命名為「Spacing」
- [ ] 繪製矩形，寬度分別為：
  - [ ] 4px（XS）
  - [ ] 8px（SM）
  - [ ] 16px（MD）
  - [ ] 24px（LG）
  - [ ] 32px（XL）
  - [ ] 48px（XXL）
- [ ] 添加文字標籤

**檢查**：
- [ ] 所有間距已創建（共 6 個）
- [ ] 標籤清晰

---

### 2.4 創建 Effects（5 分鐘）

#### 創建陰影樣式
- [ ] 繪製矩形（100x100）
- [ ] 右側面板 → Effects → 「+」→ Drop Shadow
- [ ] 設置：`0 2px 4px rgba(0,0,0,0.08)`
- [ ] Styles → 「+」→ 命名：`Shadow / Small`
- [ ] 重複創建：
  - [ ] `Shadow / Medium`（`0 4px 8px rgba(0,0,0,0.12)`）
  - [ ] `Shadow / Large`（`0 8px 16px rgba(0,0,0,0.15)`）

**檢查**：
- [ ] 所有 Effects 已創建（共 3 個）

---

## 第三步：創建組件庫（60 分鐘）

### 3.1 按鈕組件（20 分鐘）

#### 創建 Primary Button
- [ ] 切換到 Components 頁
- [ ] 創建 Frame（Auto Layout, Horizontal）
- [ ] 添加 Rectangle（填充：Blue-500，圓角：4px）
- [ ] 添加 Text（「計算」，白色，Body/Regular）
- [ ] 設置 Auto Layout：Padding 8px 16px
- [ ] 右鍵 → Create Component（Ctrl+Alt+K）
- [ ] 命名：`Button / Primary / Default / Medium`

#### 創建 Variants
- [ ] 右側面板 → Variants → 「+」
- [ ] 添加屬性：State（Default, Hover, Active, Disabled, Loading）
- [ ] 添加屬性：Size（Small, Medium, Large）
- [ ] 複製並修改每個變體：
  - [ ] Hover：填充 Blue-400
  - [ ] Active：填充 Blue-600
  - [ ] Disabled：填充 Gray-300，文字透明度 50%
  - [ ] Loading：添加 spinner 圖標

#### 創建 Secondary Button
- [ ] 複製 Primary Button
- [ ] 修改：填充白色，邊框 Gray-300，文字 Gray-600
- [ ] 命名：`Button / Secondary`
- [ ] 創建 Variants（同 Primary）

#### 創建 Danger Button
- [ ] 複製 Primary Button
- [ ] 修改：填充 Red-500
- [ ] 命名：`Button / Danger`

#### 創建 Link Button
- [ ] 創建僅文字的按鈕
- [ ] 文字：Blue-500
- [ ] Hover：添加下劃線
- [ ] 命名：`Button / Link`

**檢查**：
- [ ] 所有按鈕組件已創建（4 類）
- [ ] Variants 設置正確
- [ ] 命名規範正確

---

### 3.2 輸入框組件（20 分鐘）

#### 創建 Text Input
- [ ] 創建 Frame（寬度 200px，高度 32px）
- [ ] 添加 Rectangle（填充白色，邊框 Gray-300，圓角 4px）
- [ ] 添加 Text（Placeholder：「請輸入...」）
- [ ] 設置 Auto Layout
- [ ] Create Component
- [ ] 命名：`Input / Text / Default / Medium`

#### 創建 Variants
- [ ] 添加屬性：State（Default, Hover, Focus, Error, Disabled）
- [ ] 添加屬性：Size（Small, Medium, Large）
- [ ] 修改每個變體：
  - [ ] Hover：邊框 Blue-400
  - [ ] Focus：邊框 Blue-500，添加陰影
  - [ ] Error：邊框 Red-500
  - [ ] Disabled：背景 Gray-100

#### 創建 Date Input
- [ ] 複製 Text Input
- [ ] 左側添加日曆圖標（📅）
- [ ] 命名：`Input / Date`

#### 創建 Number Input
- [ ] 複製 Text Input
- [ ] 文字右對齊
- [ ] 可添加上下箭頭
- [ ] 命名：`Input / Number`

#### 創建 Input with Unit
- [ ] 複製 Text Input
- [ ] 右側添加單位標籤（HKD/USD）
- [ ] 單位背景：Gray-50
- [ ] 命名：`Input / With Unit`

**檢查**：
- [ ] 所有輸入框組件已創建（4 類）
- [ ] Variants 設置正確
- [ ] 狀態顏色正確

---

### 3.3 單選按鈕組件（10 分鐘）

#### 創建 Radio Button
- [ ] 繪製 Ellipse（16x16px）
- [ ] 邊框：Gray-300，填充：白色
- [ ] 右側添加文字標籤
- [ ] Create Component
- [ ] 命名：`Radio / Button / Unchecked`

#### 創建 Variants
- [ ] 添加屬性：State（Unchecked, Checked, Hover, Disabled）
- [ ] Checked：邊框 Blue-500，填充 Blue-500，中心白色小圓
- [ ] Hover：邊框 Blue-400
- [ ] Disabled：邊框 Gray-300，填充 Gray-100

#### 創建 Radio Group
- [ ] 創建 Frame（Auto Layout, Horizontal）
- [ ] 添加 3-4 個 Radio Button 實例
- [ ] 間距：24px
- [ ] 命名：`Radio / Group / Horizontal`

**檢查**：
- [ ] Radio Button 已創建
- [ ] Variants 正確
- [ ] Radio Group 已創建

---

### 3.4 卡片組件（10 分鐘）

#### 創建 Standard Card
- [ ] 創建 Frame（Auto Layout, Vertical）
- [ ] 填充：白色，邊框：Gray-300，圓角：8px
- [ ] 添加 Auto Layout：Padding 24px
- [ ] Create Component
- [ ] 命名：`Card / Standard`

#### 添加屬性
- [ ] Title（Text）：卡片標題
- [ ] Has Header（Boolean）
- [ ] Content（Instance）

#### 創建 Collapsible Card
- [ ] 複製 Standard Card
- [ ] 添加展開/收起按鈕
- [ ] 創建 Variants：Collapsed, Expanded
- [ ] 命名：`Card / Collapsible`

**檢查**：
- [ ] 卡片組件已創建（2 類）
- [ ] 屬性設置正確

---

### 3.5 表格組件（15 分鐘）

#### 創建 Table Header Row
- [ ] 創建 Frame（高度 40px，Auto Layout）
- [ ] 添加多個 Cell（填充：Gray-50）
- [ ] 文字：粗體
- [ ] Create Component
- [ ] 命名：`Table / Header Row`

#### 創建 Table Row
- [ ] 創建 Frame（高度 40px）
- [ ] 添加 Cells
- [ ] Create Component
- [ ] 命名：`Table / Row / Default`

#### 創建 Variants
- [ ] 添加屬性：Type（Default, Alt, Hover, Selected）
- [ ] 修改填充色：
  - [ ] Alt：Gray-50
  - [ ] Hover：Blue-50
  - [ ] Selected：Blue-100

**檢查**：
- [ ] 表格組件已創建
- [ ] Variants 正確

---

### 3.6 彈窗組件（15 分鐘）

#### 創建 Confirmation Modal
- [ ] 創建 Frame（寬度 400px，Auto Layout）
- [ ] 填充：白色，圓角：8px，陰影：Medium
- [ ] 添加 Header（標題 + 關閉按鈕）
- [ ] 添加 Divider
- [ ] 添加 Body
- [ ] 添加 Footer（兩個按鈕）
- [ ] Create Component
- [ ] 命名：`Modal / Confirmation`

#### 創建 Error Modal
- [ ] 複製 Confirmation Modal
- [ ] 修改標題顏色：Red-500
- [ ] 添加警告圖標
- [ ] 命名：`Modal / Error`

#### 創建 Success Modal
- [ ] 複製 Confirmation Modal
- [ ] 修改標題顏色：Green-500
- [ ] 添加成功圖標
- [ ] 命名：`Modal / Success`

**檢查**：
- [ ] 彈窗組件已創建（3 類）
- [ ] 顏色正確

---

### 3.7 通知提示組件（10 分鐘）

#### 創建 Notification Toast
- [ ] 創建 Frame（寬度 320px，Auto Layout）
- [ ] 填充：根據類型（Success：Green-50）
- [ ] 邊框：對應顏色
- [ ] 添加圖標、文字、關閉按鈕
- [ ] Create Component
- [ ] 命名：`Notification / Toast / Success`

#### 創建 Variants
- [ ] 添加屬性：Type（Success, Error, Warning, Info）
- [ ] 修改填充色和邊框色

**檢查**：
- [ ] 通知組件已創建
- [ ] Variants 正確

---

### 3.8 加載組件（10 分鐘）

#### 創建 Spinner
- [ ] 使用橢圓工具繪製圓環
- [ ] 或使用插件（Loading Spinner）
- [ ] 顏色：Blue-500
- [ ] Create Component
- [ ] 命名：`Loading / Spinner / Medium`

#### 創建 Variants
- [ ] 添加屬性：Size（Small, Medium, Large）

#### 創建 Button Loading
- [ ] 基於 Primary Button
- [ ] 添加 Spinner
- [ ] 文字：「計算中...」

**檢查**：
- [ ] 加載組件已創建
- [ ] 尺寸正確

---

## 第四步：設計頁面（90 分鐘）

### 4.1 查詢輸入頁（30 分鐘）

#### 創建 Frame
- [ ] 切換到「查詢輸入頁」
- [ ] 創建 Frame（1440x1024）
- [ ] 命名：「查詢輸入頁 - Desktop」

#### 添加頂部導航欄
- [ ] 從組件庫拖入或創建
- [ ] 高度：64px
- [ ] 添加 Logo、系統名稱、用戶信息

#### 添加頁面標題區
- [ ] 高度：56px
- [ ] 填充：Gray-50
- [ ] 添加返回按鈕和標題

#### 添加表單卡片 1：保單資料
- [ ] 拖入 Card / Standard 組件
- [ ] 添加標題：「【1. 保單資料】」
- [ ] 添加表單字段（使用 Input 和 Radio 組件）
- [ ] 三列佈局

#### 添加表單卡片 2：賬戶價值
- [ ] 同上
- [ ] 字段：紅利結餘、現金儲值等

#### 添加表單卡片 3：其他
- [ ] 拖入 Card / Collapsible
- [ ] 默認收起狀態

#### 添加底部按鈕
- [ ] 拖入 Button / Secondary（重置）
- [ ] 拖入 Button / Primary（計算）

**檢查**：
- [ ] 所有卡片已添加
- [ ] 表單字段正確
- [ ] 佈局正確

---

### 4.2 結果展示頁（20 分鐘）

#### 創建 Frame
- [ ] 切換到「結果展示頁」
- [ ] 創建 Frame（1440x1024）

#### 添加操作按鈕區
- [ ] 4 個按鈕：導出 PDF、列印、發送郵件、重新計算

#### 添加保單資料表格
- [ ] 拖入 Table 組件
- [ ] 5 列：產品名稱、保單生效日、年齡、性別、投保金額

#### 添加保單戶口價值表格
- [ ] 2 列：項目、金額
- [ ] 金額右對齊

#### 添加說明摘要
- [ ] 使用 Bullet Points

**檢查**：
- [ ] 所有表格已添加
- [ ] 金額格式正確

---

### 4.3 首頁（20 分鐘）

#### 創建 Frame
- [ ] 切換到「首頁」
- [ ] 創建 Frame（1440x1024）

#### 添加快速入口卡片
- [ ] 2 個大卡片：快速查詢、管理後台

#### 添加最近查詢記錄
- [ ] 表格形式
- [ ] 5 行數據

#### 添加系統公告（可選）
- [ ] 卡片形式

**檢查**：
- [ ] 卡片佈局正確
- [ ] 表格正確

---

### 4.4 管理後台頁（20 分鐘）

#### 創建 Frame
- [ ] 切換到「管理後台」
- [ ] 創建 Frame（1440x1024）

#### 添加選項卡
- [ ] 3 個：產品配置、費率表管理、變更歷史

#### 添加產品列表表格
- [ ] 5 列：代碼、產品名稱、類別、狀態、操作

#### 添加分頁控件
- [ ] 底部

**檢查**：
- [ ] 選項卡正確
- [ ] 表格正確

---

## 第五步：創建交互原型（30 分鐘）

### 5.1 連接頁面（15 分鐘）

#### 切換到 Prototype 標籤
- [ ] 選擇「首頁」的「快速查詢」按鈕
- [ ] 拖動連接線到「查詢輸入頁」
- [ ] 設置：On Click → Navigate To → Smart Animate → 300ms

#### 連接其他頁面
- [ ] 查詢輸入頁 → 計算 → 結果展示頁
- [ ] 結果展示頁 → 返回 → 查詢輸入頁
- [ ] 首頁 → 管理後台 → 管理後台頁

**檢查**：
- [ ] 所有頁面已連接
- [ ] 動畫設置正確

---

### 5.2 添加組件交互（15 分鐘）

#### 添加按鈕 Hover
- [ ] 選擇按鈕組件
- [ ] Prototype → Add Interaction
- [ ] While Hovering → Change To → Hover 狀態

#### 添加輸入框 Focus
- [ ] 選擇輸入框
- [ ] While Pressing → Change To → Focus 狀態

#### 添加卡片展開
- [ ] 選擇 Collapsible Card
- [ ] On Click → Toggle → Expanded 狀態

**檢查**：
- [ ] 所有交互已添加
- [ ] 測試原型

---

## 第六步：檢查與導出（15 分鐘）

### 6.1 檢查（10 分鐘）

#### 檢查設計系統
- [ ] 所有 Color Styles 正確
- [ ] 所有 Text Styles 正確
- [ ] 所有 Effects 正確

#### 檢查組件庫
- [ ] 所有組件已創建
- [ ] Variants 正確
- [ ] 命名規範

#### 檢查頁面
- [ ] 所有頁面已設計
- [ ] 佈局正確
- [ ] 無用圖層已清理

---

### 6.2 導出（5 分鐘）

#### 導出設計稿
- [ ] 選擇所有頁面 Frame
- [ ] 右側面板 → Export
- [ ] 格式：PNG
- [ ] 倍數：1x, 2x
- [ ] 點擊 Export

#### 導出資源
- [ ] 圖標
- [ ] Logo
- [ ] 其他圖片資源

---

## 第七步：分享與文檔（10 分鐘）

### 7.1 分享給團隊（5 分鐘）

#### 設置權限
- [ ] 右上角 Share 按鈕
- [ ] 設置權限：Can view / Can comment / Can edit
- [ ] 複製鏈接
- [ ] 發送給團隊

---

### 7.2 更新文檔（5 分鐘）

#### 更新項目任務清單
- [ ] 勾選已完成的任務
- [ ] 更新進度

#### 更新 CHANGELOG
- [ ] 添加新增內容
- [ ] 更新版本號

---

## 📊 總體進度檢查

### 設計系統
- [ ] Color Styles（11 個）
- [ ] Text Styles（8 個）
- [ ] Spacing（6 個）
- [ ] Effects（3 個）

### 組件庫
- [ ] Buttons（4 類）
- [ ] Inputs（4 類）
- [ ] Radio Buttons（2 類）
- [ ] Cards（2 類）
- [ ] Tables（2 類）
- [ ] Modals（3 類）
- [ ] Notifications（4 類）
- [ ] Loading（3 類）

### 頁面設計
- [ ] 首頁
- [ ] 查詢輸入頁
- [ ] 結果展示頁
- [ ] 管理後台頁
- [ ] 系統管理頁

### 交互原型
- [ ] 頁面連接
- [ ] 組件交互
- [ ] 動畫設置

### 交付
- [ ] 設計稿導出
- [ ] 資源導出
- [ ] 分享給團隊
- [ ] 文檔更新

---

## ⏱️ 預計時間

| 步驟 | 預計時間 |
|------|----------|
| 第一步：創建頁面結構 | 5 分鐘 |
| 第二步：創建設計系統 | 30 分鐘 |
| 第三步：創建組件庫 | 60 分鐘 |
| 第四步：設計頁面 | 90 分鐘 |
| 第五步：創建交互原型 | 30 分鐘 |
| 第六步：檢查與導出 | 15 分鐘 |
| 第七步：分享與文檔 | 10 分鐘 |
| **總計** | **約 4 小時** |

---

## 💡 小貼士

1. **使用 Auto Layout**：讓設計更靈活
2. **善用組件**：修改一處，全局更新
3. **命名規範**：方便開發人員理解
4. **定期保存**：Ctrl+S
5. **使用版本歷史**：重要節點創建版本

---

**開始時間**：____  
**預計完成**：____  
**實際完成**：____

**設計師**：____  
**日期**：____

---

**最後更新**：2026-03-24  
**狀態**：可用
