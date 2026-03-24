# Figma 模板文件結構說明

> 本文檔說明 Figma 設計文件的完整結構、層級組織和命名規範。

---

## 📁 Figma 文件結構

### 頁面結構（Pages）

```
📄 Cover                    # 封面頁
├── 項目信息
├── 設計狀態
└── 快速導航鏈接

📄 Design System            # 設計系統頁
├── Colors（顏色系統）
├── Typography（字體系統）
├── Spacing（間距系統）
├── Shadows（陰影系統）
└── Icons（圖標系統）

📄 Components               # 組件庫頁
├── Buttons（按鈕組件）
├── Inputs（輸入框組件）
├── Radio & Checkbox（單選/複選框）
├── Cards（卡片組件）
├── Tables（表格組件）
├── Modals（彈窗組件）
├── Notifications（通知組件）
├── Loading（加載組件）
└── Navigation（導航組件）

📄 首頁                     # 首頁設計
├── 桌面端（1440x1024）
├── 平板端（1024x768）
└── 交互註釋

📄 查詢輸入頁                # 查詢輸入頁設計
├── 桌面端（1440x1024）
├── 表單狀態（默認/錯誤/成功）
└── 交互註釋

📄 結果展示頁                # 結果展示頁設計
├── 桌面端（1440x1024）
├── 空狀態
└── 交互註釋

📄 管理後台                  # 管理後台設計
├── 產品配置頁
├── 費率表管理頁
└── 變更歷史頁

📄 Prototype                # 交互原型頁
├── 流程圖
├── 原型連接
└── 動畫說明

📄 Archive                  # 存檔頁
├── 舊版本設計
└── 廢棄方案
```

---

## 🎨 頁面詳細結構

### 1. Cover（封面頁）

**Frame 結構**：
```
Cover (1920x1080)
├── Background（填充：Gray-50）
├── Logo（左上角）
├── 項目信息（居中）
│   ├── 項目名稱（H1）
│   ├── 版本號（Body/Regular）
│   ├── 最後更新日期（Body/Small）
│   └── 設計師（Body/Small）
├── 設計狀態（右側）
│   ├── 進度條
│   └── 狀態標籤（進行中/已完成）
└── 快速導航（底部）
    ├── 設計系統 → 鏈接
    ├── 組件庫 → 鏈接
    ├── 首頁 → 鏈接
    └── 查詢輸入頁 → 鏈接
```

---

### 2. Design System（設計系統頁）

**Frame 結構**：
```
Design System
├── Colors (1200x800)
│   ├── Primary（主色）
│   │   ├── Blue-500 (#1890ff)
│   │   ├── Blue-400 (#40a9ff)
│   │   └── Blue-600 (#096dd9)
│   ├── Functional（功能色）
│   │   ├── Green-500 (#52c41a)
│   │   ├── Yellow-500 (#faad14)
│   │   └── Red-500 (#f5222d)
│   └── Neutral（中性色）
│       ├── Gray-850 (#262626)
│       ├── Gray-600 (#595959)
│       ├── Gray-300 (#d9d9d9)
│       ├── Gray-100 (#f5f5f5)
│       └── Gray-50 (#fafafa)
│
├── Typography (1200x600)
│   ├── Headings
│   │   ├── H1 - 24px
│   │   ├── H2 - 20px
│   │   └── H3 - 16px
│   ├── Body
│   │   ├── Large - 16px
│   │   ├── Regular - 14px
│   │   └── Small - 12px
│   └── Numbers
│       ├── Amount - 14px
│       └── Large Amount - 20px
│
├── Spacing (800x400)
│   ├── XS - 4px
│   ├── SM - 8px
│   ├── MD - 16px
│   ├── LG - 24px
│   ├── XL - 32px
│   └── XXL - 48px
│
├── Shadows (800x400)
│   ├── Small
│   ├── Medium
│   └── Large
│
└── Icons (1200x600)
    ├── 系統圖標
    └── 功能圖標
```

**顏色展示格式**：
```
Color Swatch (80x80)
├── Rectangle (80x80, 填充對應顏色)
└── Text Label (下方)
    ├── 名稱（如：Blue-500）
    └── 色值（如：#1890ff）
```

---

### 3. Components（組件庫頁）

**Frame 結構**：
```
Components
├── Buttons (1600x1200)
│   ├── Primary Button（主按鈕）
│   │   ├── Default / Medium
│   │   ├── Hover / Medium
│   │   ├── Active / Medium
│   │   ├── Disabled / Medium
│   │   ├── Default / Small
│   │   └── Default / Large
│   ├── Secondary Button（次要按鈕）
│   ├── Danger Button（危險按鈕）
│   └── Link Button（鏈接按鈕）
│
├── Inputs (1600x1200)
│   ├── Text Input（文本輸入框）
│   │   ├── Default
│   │   ├── Hover
│   │   ├── Focus
│   │   ├── Error
│   │   └── Disabled
│   ├── Number Input（數字輸入框）
│   ├── Date Input（日期輸入框）
│   ├── Input with Unit（帶單位輸入框）
│   └── Text Area（多行輸入）
│
├── Radio & Checkbox (1200x800)
│   ├── Radio Button（單選按鈕）
│   │   ├── Unchecked
│   │   ├── Checked
│   │   ├── Hover
│   │   └── Disabled
│   ├── Radio Group（單選按鈕組）
│   │   ├── Horizontal（橫向）
│   │   └── Vertical（縱向）
│   └── Checkbox（複選框）
│
├── Cards (1200x800)
│   ├── Standard Card（標準卡片）
│   └── Collapsible Card（可折疊卡片）
│
├── Tables (1600x1000)
│   ├── Table Header（表頭）
│   ├── Table Row（行）
│   │   ├── Default
│   │   ├── Alt
│   │   └── Hover
│   └── Table with Data（示例表格）
│
├── Modals (1200x800)
│   ├── Confirmation Modal（確認彈窗）
│   ├── Error Modal（錯誤彈窗）
│   └── Success Modal（成功彈窗）
│
├── Notifications (1200x600)
│   ├── Success
│   ├── Error
│   ├── Warning
│   └── Info
│
├── Loading (800x600)
│   ├── Spinner
│   ├── Button Loading
│   └── Page Loading
│
└── Navigation (1200x600)
    ├── Top Nav（頂部導航）
    ├── Side Nav（側邊導航）
    └── Breadcrumb（麵包屑）
```

---

### 4. 首頁（Home Page）

**Frame 結構**：
```
首頁 - Desktop (1440x1024)
├── Top Navigation Bar (1440x64)
│   ├── Logo (左側)
│   ├── System Name
│   └── User Menu (右側)
│       ├── Avatar
│       ├── User Name
│       └── Logout Button
│
├── Page Header (1440x56)
│   └── Title「首頁」
│
├── Content Area (1392x800)
│   ├── Quick Actions (橫向卡片組)
│   │   ├── Quick Query Card (大按鈕)
│   │   ├── Admin Panel Card (精算管理員)
│   │   └── System Admin Card (IT 管理員)
│   │
│   ├── Recent Queries Card (1392x300)
│   │   ├── Card Header
│   │   │   ├── Title「最近查詢記錄」
│   │   │   └── View All Link
│   │   └── Table
│   │       ├── Header Row
│   │       └── Data Rows (5 行)
│   │
│   └── System Announcements Card (可選)
│       └── Announcement Content
│
└── Footer (可選)
```

---

### 5. 查詢輸入頁（Query Input Page）

**Frame 結構**：
```
查詢輸入頁 - Desktop (1440x1024)
├── Top Navigation Bar (1440x64)
│
├── Page Header (1440x56)
│   ├── Back Button (←)
│   └── Title「保單年結表查詢」
│
├── Content Area (1392x850)
│   ├── Form Card 1: 保單資料 (1392x400)
│   │   ├── Card Header
│   │   │   └── Title「【1. 保單資料】」
│   │   └── Form Fields (3 列佈局)
│   │       ├── 退保日期 *
│   │       ├── 繳至日期 *
│   │       ├── 產品名稱 *
│   │       ├── 保單生效日 *
│   │       ├── 年齡 *
│   │       ├── 性別 *
│   │       ├── 吸煙狀態 *
│   │       ├── 投保金額 *
│   │       ├── 幣種
│   │       └── 繳費方式
│   │
│   ├── Form Card 2: 賬戶價值 (1392x250)
│   │   ├── Card Header
│   │   │   └── Title「【2. 賬戶價值】」
│   │   └── Form Fields (3 列佈局)
│   │       ├── 紅利結餘
│   │       ├── 現金儲值結餘
│   │       ├── 貸款結餘
│   │       └── 已繳保費 *
│   │
│   ├── Form Card 3: 其他 (1392x80)
│   │   ├── Card Header
│   │   │   ├── Title「【3. 其他】」
│   │   │   └── Expand Button (▶ 展開)
│   │   └── Collapsed Content (隱藏)
│   │
│   └── Action Bar (1392x50)
│       ├── Reset Button (次要按鈕)
│       └── Calculate Button (主按鈕)
│
└── Error States (單獨 Frame)
    ├── Field Error (輸入框錯誤)
    ├── Form Error (表單錯誤)
    └── Modal Error (彈窗錯誤)
```

---

### 6. 結果展示頁（Result Page）

**Frame 結構**：
```
結果展示頁 - Desktop (1440x1024)
├── Top Navigation Bar (1440x64)
│
├── Page Header (1440x56)
│   ├── Back Button (←)
│   └── Title「年結表結果」
│
├── Action Bar (1392x50)
│   ├── Export PDF Button
│   ├── Print Button
│   ├── Email Button
│   └── Recalculate Button
│
├── Content Area (1392x800)
│   ├── Policy Info Card (1392x150)
│   │   ├── Card Header
│   │   │   └── Title「保單資料」
│   │   └── Info Table (4 列)
│   │       ├── Header Row
│   │       └── Data Row
│   │
│   ├── Account Value Card (1392x250)
│   │   ├── Card Header
│   │   │   └── Title「保單戶口價值」
│   │   └── Value Table (2 列)
│   │       ├── Header Row
│   │       └── Data Rows (4 行)
│   │           ├── 現金價值
│   │           ├── 紅利結餘
│   │           ├── 終期紅利
│   │           └── 退保價值
│   │
│   └── Summary Card (1392x200)
│       ├── Card Header
│       │   └── Title「說明摘要」
│       └── Bullet Points
│           ├── 本年度紅利增長率
│           ├── 累計紅利
│           └── 保證現金價值
│
└── Empty State (單獨 Frame)
    └── 無數據提示
```

---

### 7. 管理後台頁（Admin Panel）

**Frame 結構**：
```
管理後台 - 產品配置 (1440x1024)
├── Top Navigation Bar (1440x64)
│
├── Page Header (1440x56)
│   ├── Back Button (←)
│   └── Title「數據管理」
│
├── Tabs (1392x48)
│   ├── 產品配置 (Active)
│   ├── 費率表管理
│   └── 變更歷史
│
├── Content Area (1392x800)
│   ├── Product Table Card
│   │   ├── Card Header
│   │   │   ├── Title「產品配置列表」
│   │   │   └── Add Product Button
│   │   └── Table
│   │       ├── Header Row
│   │       │   ├── 代碼
│   │       │   ├── 產品名稱
│   │       │   ├── 狀態
│   │       │   └── 操作
│   │       └── Data Rows
│   │           ├── 產品 1
│   │           ├── 產品 2
│   │           └── ...
│   │
│   └── Pagination (可選)
│       └── 分頁控件
│
└── Edit Product Modal (單獨 Frame)
    └── 編輯產品表單
```

---

## 🏷️ 層級命名規範

### Frame 命名
```
格式：[類型] 名稱 / 狀態 / 尺寸
示例：
  - [Page] 首頁 / Desktop
  - [Component] Button / Primary / Default
  - [Modal] Confirmation / Default
```

### Group 命名
```
格式：組名 - 用途
示例：
  - Form Fields - 保單資料
  - Table Rows - 產品列表
  - Actions - 底部按鈕
```

### Layer 命名
```
格式：元素類型 - 名稱
示例：
  - Text - 標題
  - Rectangle - 背景
  - Icon - 日曆
  - Input - 退保日期
```

---

## 📐 Auto Layout 設置

### 按鈕 Auto Layout
```
Frame: Button / Primary
├── Direction: Horizontal
├── Padding: 8px 16px
├── Item Spacing: 8px
├── Alignment: Center
└── Resizing: Hug Contents
```

### 表單字段 Auto Layout
```
Frame: Form Field
├── Direction: Vertical
├── Padding: 0
├── Item Spacing: 4px
├── Alignment: Stretch
└── Resizing: Fill Container
```

### 卡片 Auto Layout
```
Frame: Card
├── Direction: Vertical
├── Padding: 24px
├── Item Spacing: 16px
├── Alignment: Stretch
└── Resizing: Fill Container
```

---

## 🎯 組件屬性（Component Properties）

### 按鈕組件屬性
```
Properties:
  - State (Variant): Default, Hover, Active, Disabled, Loading
  - Size (Variant): Small, Medium, Large
  - Text (Text Property): 按鈕文字
  - Icon (Boolean): 是否顯示圖標
  - Icon Left (Instance): 左側圖標
  - Icon Right (Instance): 右側圖標
```

### 輸入框組件屬性
```
Properties:
  - State (Variant): Default, Hover, Focus, Error, Disabled
  - Size (Variant): Small, Medium, Large
  - Label (Text Property): 字段標籤
  - Placeholder (Text Property): 佔位文字
  - Value (Text Property): 輸入值
  - Unit (Text Property): 單位
  - Error Message (Text Property): 錯誤提示
  - Required (Boolean): 是否必填
```

### 卡片組件屬性
```
Properties:
  - Title (Text Property): 卡片標題
  - Collapsible (Boolean): 是否可折疊
  - Expanded (Boolean): 是否展開
  - Content (Instance): 內容區域
```

---

## 📤 導出設置

### 導出格式
```
設計稿審查：PNG @1x, @2x
開發移交：PDF, SVG (圖標)
文檔插入：PNG @1x
打印：PDF A4
```

### 導出 Frame
```
- Cover
- Design System (所有子 Frame)
- Components (所有子 Frame)
- 首頁 - Desktop
- 查詢輸入頁 - Desktop
- 結果展示頁 - Desktop
- 管理後台 - Desktop
```

---

## 🔗 原型連接

### 頁面跳轉
```
首頁
├── 點擊「快速查詢」→ 查詢輸入頁
├── 點擊「管理後台」→ 管理後台頁
└── 點擊最近記錄 → 結果展示頁

查詢輸入頁
├── 點擊「計算」→ 結果展示頁
├── 點擊「返回」→ 首頁
└── 點擊「重置」→ 確認彈窗

結果展示頁
├── 點擊「導出 PDF」→ 下載
├── 點擊「列印」→ 列印對話框
├── 點擊「發送郵件」→ 郵件彈窗
├── 點擊「重新計算」→ 查詢輸入頁
└── 點擊「返回」→ 首頁
```

---

## 📋 檢查清單

### 文件組織
- [ ] 所有頁面已創建並命名
- [ ] 所有 Frame 已命名規範
- [ ] 圖層分組清晰
- [ ] 無用圖層已清理

### 設計系統
- [ ] Color Styles 已創建
- [ ] Text Styles 已創建
- [ ] Effects 已創建
- [ ] 所有樣式已命名規範

### 組件庫
- [ ] 所有組件已創建
- [ ] Variants 已設置
- [ ] Properties 已配置
- [ ] 組件已命名規範

### 頁面設計
- [ ] 所有頁面已設計
- [ ] Auto Layout 已應用
- [ ] 響應式已考慮
- [ ] 無障礙已檢查

### 原型
- [ ] 頁面連接已完成
- [ ] 動畫已設置
- [ ] 交互已測試

### 交付
- [ ] 設計稿已導出
- [ ] 資源已導出
- [ ] 已分享給團隊
- [ ] 文檔已更新

---

**最後更新**：2026-03-24  
**狀態**：草稿
