# 組件庫詳細規格 - Figma 層級結構

> 每個組件的完整 Figma 層級結構、屬性設置和 Variants 配置。

---

## 🧩 按鈕組件（Buttons）

### 1. Primary Button（主按鈕）

**Component 名稱**：`Button / Primary`

#### Figma 層級結構
```
Button / Primary / Default / Medium (Frame, Auto Layout)
├── Background (Rectangle)
│   ├── Fill: #1890ff
│   ├── Corner Radius: 4px
│   └── Auto Layout: Fill Container
└── Text (Text Layer)
    ├── Content: "計算"
    ├── Style: Body / Regular
    ├── Color: #ffffff
    └── Auto Layout: Hug Contents
```

#### Auto Layout 設置
```
Direction: Horizontal
Padding: 8px 16px
Item Spacing: 8px
Alignment: Center
Resizing: Hug Contents
```

#### Variants 配置
```
Properties:
  - State: Default, Hover, Active, Disabled, Loading
  - Size: Small, Medium, Large

Variant Combinations:
  State × Size = 5 × 3 = 15 variants
```

#### 各狀態規格

| 狀態 | Background Fill | Text Color | 特殊屬性 |
|------|----------------|------------|----------|
| Default | `#1890ff` | `#ffffff` | - |
| Hover | `#40a9ff` | `#ffffff` | - |
| Active | `#096dd9` | `#ffffff` | - |
| Disabled | `#d9d9d9` | `#ffffff80` | - |
| Loading | `#1890ff` | `#ffffff` | 添加 Spinner |

#### 各尺寸規格

| 尺寸 | Height | Text Size | Padding |
|------|--------|-----------|---------|
| Small | 24px | 12px | 4px 12px |
| Medium | 32px | 14px | 8px 16px |
| Large | 40px | 16px | 12px 24px |

---

### 2. Secondary Button（次要按鈕）

**Component 名稱**：`Button / Secondary`

#### Figma 層級結構
```
Button / Secondary / Default / Medium (Frame, Auto Layout)
├── Background (Rectangle)
│   ├── Fill: #ffffff
│   ├── Stroke: 1px solid #d9d9d9
│   ├── Corner Radius: 4px
│   └── Auto Layout: Fill Container
└── Text (Text Layer)
    ├── Content: "重置"
    ├── Style: Body / Regular
    ├── Color: #595959
    └── Auto Layout: Hug Contents
```

#### Variants 配置
```
Properties:
  - State: Default, Hover, Active, Disabled
  - Size: Small, Medium, Large

Variant Combinations:
  State × Size = 4 × 3 = 12 variants
```

#### 各狀態規格

| 狀態 | Fill | Stroke | Text Color |
|------|------|--------|------------|
| Default | `#ffffff` | `#d9d9d9` | `#595959` |
| Hover | `#ffffff` | `#1890ff` | `#1890ff` |
| Active | `#ffffff` | `#096dd9` | `#096dd9` |
| Disabled | `#fafafa` | `#d9d9d9` | `#bfbfbf` |

---

### 3. Danger Button（危險按鈕）

**Component 名稱**：`Button / Danger`

#### Figma 層級結構
同 Primary Button，但顏色不同

#### 各狀態規格

| 狀態 | Background Fill | Text Color |
|------|----------------|------------|
| Default | `#f5222d` | `#ffffff` |
| Hover | `#ff4d4f` | `#ffffff` |
| Active | `#cf1322` | `#ffffff` |
| Disabled | `#d9d9d9` | `#ffffff80` |

---

### 4. Link Button（鏈接按鈕）

**Component 名稱**：`Button / Link`

#### Figma 層級結構
```
Button / Link / Default (Frame, Auto Layout)
└── Text (Text Layer)
    ├── Content: "展開詳情"
    ├── Style: Body / Regular
    ├── Color: #1890ff
    ├── Decorator: Underline (Hover 時)
    └── Auto Layout: Hug Contents
```

#### Variants 配置
```
Properties:
  - State: Default, Hover, Active, Disabled
  - Icon: None, Left, Right

Variant Combinations:
  State × Icon = 4 × 3 = 12 variants
```

#### 各狀態規格

| 狀態 | Text Color | Underline |
|------|------------|-----------|
| Default | `#1890ff` | None |
| Hover | `#40a9ff` | Yes |
| Active | `#096dd9` | Yes |
| Disabled | `#bfbfbf` | None |

---

## 📝 輸入框組件（Inputs）

### 1. Text Input（文本輸入框）

**Component 名稱**：`Input / Text`

#### Figma 層級結構
```
Input / Text / Default / Medium (Frame, Auto Layout)
├── Label (Text Layer, 可選)
│   ├── Content: "退保日期"
│   ├── Style: Body / Small
│   ├── Color: #595959
│   └── Auto Layout: Hug Contents
│
├── Input Container (Frame, Auto Layout)
│   ├── Background (Rectangle)
│   │   ├── Fill: #ffffff
│   │   ├── Stroke: 1px solid #d9d9d9
│   │   ├── Corner Radius: 4px
│   │   └── Auto Layout: Fill Container
│   │
│   ├── Input Text (Text Layer)
│   │   ├── Content: "請輸入..."
│   │   ├── Style: Body / Regular
│   │   ├── Color: #595959 (Placeholder: #bfbfbf)
│   │   └── Auto Layout: Hug Contents
│   │
│   └── Right Addon (可選)
│       └── Icon 或 Unit Text
│
└── Error Message (Text Layer, 可選)
    ├── Content: "日期格式無效"
    ├── Style: Body / Small
    ├── Color: #f5222d
    └── Auto Layout: Hug Contents
```

#### Auto Layout 設置
```
Input Container:
Direction: Horizontal
Padding: 8px 12px
Item Spacing: 8px
Alignment: Center
Resizing: Fill Container
```

#### Variants 配置
```
Properties:
  - State: Default, Hover, Focus, Error, Disabled
  - Size: Small, Medium, Large
  - Label: None, Top, Left
  - Required: False, True
  - Error Message: False, True

Variant Combinations:
  State × Size × Label × Required × Error = 5 × 3 × 3 × 2 × 2 = 180 variants
  (建議拆分為多個 Component)
```

#### 各狀態規格

| 狀態 | Stroke | Fill | 特殊屬性 |
|------|--------|------|----------|
| Default | `#d9d9d9` | `#ffffff` | - |
| Hover | `#40a9ff` | `#ffffff` | - |
| Focus | `#1890ff` | `#ffffff` | Shadow: Small |
| Error | `#f5222d` | `#ffffff` | 顯示 Error Message |
| Disabled | `#d9d9d9` | `#f5f5f5` | Text: `#bfbfbf` |

---

### 2. Number Input（數字輸入框）

**Component 名稱**：`Input / Number`

#### Figma 層級結構
同 Text Input，但：
- Text Alignment: Right
- 可添加 Stepper（上下箭頭）

**Stepper 結構**：
```
Stepper (Frame, Vertical)
├── Up Arrow (Icon)
│   ├── Size: 12x12px
│   └── Color: #595959
└── Down Arrow (Icon)
    ├── Size: 12x12px
    └── Color: #595959
```

---

### 3. Date Input（日期輸入框）

**Component 名稱**：`Input / Date`

#### Figma 層級結構
```
Input / Date / Default / Medium (Frame, Auto Layout)
├── Label (可選)
│
├── Input Container (Frame, Auto Layout)
│   ├── Calendar Icon (Icon)
│   │   ├── Icon: 📅
│   │   ├── Size: 16px
│   │   └── Color: #595959
│   │
│   ├── Input Text (Text Layer)
│   │   ├── Content: "2026-03-24"
│   │   ├── Style: Body / Regular
│   │   └── Color: #262626
│   │
│   └── Background (Rectangle)
│       └── 同 Text Input
│
└── Error Message (可選)
```

---

### 4. Input with Unit（帶單位輸入框）

**Component 名稱**：`Input / With Unit`

#### Figma 層級結構
```
Input / With Unit / Default / Medium (Frame, Auto Layout)
├── Label (可選)
│
├── Input Container (Frame, Auto Layout)
│   ├── Input Text (Text Layer)
│   │   ├── Content: "123,456.78"
│   │   ├── Style: Number / Amount
│   │   ├── Alignment: Right
│   │   └── Color: #262626
│   │
│   ├── Unit (Frame)
│   │   ├── Background (Rectangle)
│   │   │   ├── Fill: #fafafa
│   │   │   └── Stroke: 1px solid #d9d9d9 (左側)
│   │   │
│   │   └── Unit Text (Text Layer)
│   │       ├── Content: "HKD"
│   │       ├── Style: Body / Small
│   │       └── Color: #595959
│   │
│   └── Main Background (Rectangle)
│       └── 同 Text Input
│
└── Error Message (可選)
```

---

## 🔘 單選按鈕組件（Radio Buttons）

### 1. Radio Button（單選按鈕）

**Component 名稱**：`Radio / Button`

#### Figma 層級結構
```
Radio / Button / Unchecked (Frame, Auto Layout)
├── Circle (Ellipse)
│   ├── Size: 16x16px
│   ├── Stroke: 1px solid #d9d9d9
│   ├── Fill: #ffffff
│   └── Corner Radius: 8px (Full)
│
└── Label (Text Layer)
    ├── Content: "男"
    ├── Style: Body / Regular
    ├── Color: #262626
    └── Margin Left: 8px
```

#### Variants 配置
```
Properties:
  - State: Unchecked, Checked, Hover, Disabled
  - Label: None, Left, Right

Variant Combinations:
  State × Label = 4 × 3 = 12 variants
```

#### 各狀態規格

| 狀態 | Stroke | Fill | Center Circle |
|------|--------|------|---------------|
| Unchecked | `#d9d9d9` | `#ffffff` | None |
| Checked | `#1890ff` | `#1890ff` | 8x8px, White |
| Hover | `#40a9ff` | `#ffffff` | None |
| Disabled | `#d9d9d9` | `#f5f5f5` | 8x8px, `#bfbfbf` |

---

### 2. Radio Group（單選按鈕組）

**Component 名稱**：`Radio / Group`

#### Figma 層級結構
```
Radio / Group / Horizontal (Frame, Auto Layout)
├── Radio Item 1 (Instance of Radio / Button)
├── Radio Item 2 (Instance)
├── Radio Item 3 (Instance)
└── Radio Item 4 (可選，Instance)
```

#### Auto Layout 設置
```
Direction: Horizontal (或 Vertical)
Item Spacing: 24px
Alignment: Center
```

---

## 📦 卡片組件（Cards）

### 1. Standard Card（標準卡片）

**Component 名稱**：`Card / Standard`

#### Figma 層級結構
```
Card / Standard (Frame, Auto Layout)
├── Card Header (Frame, Auto Layout, 可選)
│   ├── Title (Text Layer)
│   │   ├── Content: "【1. 保單資料】"
│   │   ├── Style: Heading / H3
│   │   └── Color: #262626
│   │
│   └── Action (可選)
│       └── Button 或 Link
│
├── Divider (Rectangle, 可選)
│   ├── Height: 1px
│   ├── Fill: #d9d9d9
│   └── Auto Layout: Fill Container
│
├── Card Content (Frame, Auto Layout)
│   ├── Content Goes Here
│   └── Auto Layout: Fill Container
│
└── Card Footer (可選)
    └── Actions 或 Info
```

#### Auto Layout 設置
```
Direction: Vertical
Padding: 24px
Item Spacing: 16px
Alignment: Stretch
Resizing: Fill Container
```

#### 屬性配置
```
Properties:
  - Title (Text): 卡片標題
  - Has Header (Boolean): 是否有標題區
  - Has Divider (Boolean): 是否有分隔線
  - Content (Instance): 內容區域
```

---

### 2. Collapsible Card（可折疊卡片）

**Component 名稱**：`Card / Collapsible`

#### Figma 層級結構
```
Card / Collapsible / Collapsed (Frame, Auto Layout)
├── Card Header (Frame, Auto Layout)
│   ├── Title (Text Layer)
│   │   ├── Content: "【3. 其他】"
│   │   └── Style: Heading / H3
│   │
│   └── Toggle Button (Frame, Auto Layout)
│       ├── Icon (Icon)
│       │   ├── Content: "▶" (Collapsed) / "▼" (Expanded)
│       │   └── Color: #595959
│       │
│       └── Label (Text Layer)
│           ├── Content: "展開" / "收起"
│           └── Style: Body / Small
│
└── Card Content (Frame, Auto Layout)
    ├── Visible: False (Collapsed) / True (Expanded)
    └── Content Goes Here
```

#### Variants 配置
```
Properties:
  - State: Collapsed, Expanded
  - Title (Text): 卡片標題

Variant Combinations:
  State = 2 variants
```

---

## 📊 表格組件（Tables）

### 1. Table Header（表頭）

**Component 名稱**：`Table / Header Row`

#### Figma 層級結構
```
Table / Header Row (Frame, Auto Layout)
├── Header Cell 1 (Frame)
│   ├── Text (Text Layer)
│   │   ├── Content: "產品名稱"
│   │   ├── Style: Body / Regular (Bold)
│   │   └── Color: #262626
│   │
│   └── Auto Layout: Fill Container, Padding: 12px 16px
│
├── Header Cell 2 (Frame)
├── Header Cell 3 (Frame)
└── Header Cell 4 (Frame)
```

#### Auto Layout 設置
```
Direction: Horizontal
Height: 40px
Alignment: Center
Resizing: Fill Container
```

#### 屬性配置
```
Properties:
  - Column Count (Number): 列數
  - Column Widths (Text): 各列寬度
  - Headers (Text): 表頭文字
```

---

### 2. Table Row（表格行）

**Component 名稱**：`Table / Row`

#### Figma 層級結構
```
Table / Row / Default (Frame, Auto Layout)
├── Cell 1 (Frame)
│   ├── Text (Text Layer)
│   │   ├── Content: "『世』心終身壽險計劃"
│   │   ├── Style: Body / Regular
│   │   └── Color: #262626
│   │
│   └── Auto Layout: Fill Container, Padding: 12px 16px
│
├── Cell 2 (Frame)
├── Cell 3 (Frame)
└── Cell 4 (Frame)
```

#### Variants 配置
```
Properties:
  - Type: Default, Alt, Hover, Selected
  - Column Count: 2, 3, 4, 5

Variant Combinations:
  Type × Columns = 4 × 4 = 16 variants
```

#### 各狀態規格

| 狀態 | Fill |
|------|------|
| Default | `#ffffff` |
| Alt | `#fafafa` |
| Hover | `#e6f7ff` |
| Selected | `#bae7ff` |

---

### 3. Complete Table（完整表格）

**Component 名稱**：`Table / Complete`

#### Figma 層級結構
```
Table / Complete (Frame, Auto Layout)
├── Table Header (Instance of Table / Header Row)
├── Table Row 1 (Instance of Table / Row)
├── Table Row 2 (Instance)
├── Table Row 3 (Instance)
├── Table Row 4 (Instance)
└── Table Row 5 (Instance)
```

#### 屬性配置
```
Properties:
  - Row Count (Number): 行數
  - Column Count (Number): 列數
  - Show Header (Boolean): 是否顯示表頭
```

---

## 🪟 彈窗組件（Modals）

### 1. Confirmation Modal（確認彈窗）

**Component 名稱**：`Modal / Confirmation`

#### Figma 層級結構
```
Modal / Confirmation (Frame, Auto Layout)
├── Modal Container (Frame, Auto Layout)
│   ├── Width: 400px (Min)
│   ├── Background: #ffffff
│   ├── Corner Radius: 8px
│   ├── Shadow: Medium
│   │
│   ├── Modal Header (Frame, Auto Layout)
│   │   ├── Title (Text Layer)
│   │   │   ├── Content: "確認刪除"
│   │   │   ├── Style: Heading / H3
│   │   │   └── Color: #262626
│   │   │
│   │   └── Close Button (Icon Button)
│   │       ├── Icon: ✕
│   │       └── Size: 16x16px
│   │
│   ├── Divider (Rectangle)
│   │   ├── Height: 1px
│   │   └── Fill: #d9d9d9
│   │
│   ├── Modal Body (Frame, Auto Layout)
│   │   ├── Content (Text Layer)
│   │   │   ├── Content: "確定要刪除此項嗎？此操作不可恢復。"
│   │   │   ├── Style: Body / Regular
│   │   │   └── Color: #595959
│   │   │
│   │   └── Padding: 24px
│   │
│   └── Modal Footer (Frame, Auto Layout)
│       ├── Cancel Button (Instance of Button / Secondary)
│       │   └── Text: "取消"
│       │
│       ├── Action Button (Instance of Button / Primary)
│       │   └── Text: "確認刪除"
│       │
│       └── Item Spacing: 16px
│
└── Overlay (Rectangle)
    ├── Fill: rgba(0,0,0,0.45)
    └── Blur: 4px (可選)
```

#### Auto Layout 設置
```
Modal Container:
Direction: Vertical
Padding: 24px
Item Spacing: 16px
Alignment: Center
```

---

### 2. Error Modal（錯誤彈窗）

**Component 名稱**：`Modal / Error`

#### Figma 層級結構
同 Confirmation Modal，但 Header 不同：

```
Modal Header (Frame, Auto Layout)
├── Icon (Icon)
│   ├── Icon: ⚠️
│   ├── Size: 24px
│   └── Color: #f5222d
│
├── Title (Text Layer)
│   ├── Content: "錯誤"
│   ├── Style: Heading / H3
│   └── Color: #f5222d
│
└── Close Button (可選)
```

---

### 3. Success Modal（成功彈窗）

**Component 名稱**：`Modal / Success`

#### Figma 層級結構
同 Error Modal，但顏色不同：

```
Icon Color: #52c41a
Title Color: #52c41a
Title Content: "計算完成"
```

---

## 🔔 通知提示組件（Notifications）

### Notification Toast

**Component 名稱**：`Notification / Toast`

#### Figma 層級結構
```
Notification / Toast / Success (Frame, Auto Layout)
├── Background (Rectangle)
│   ├── Fill: #f6ffed (Success)
│   ├── Stroke: 1px solid #b7eb8f
│   └── Corner Radius: 4px
│
├── Content Container (Frame, Auto Layout)
│   ├── Icon (Icon)
│   │   ├── Icon: ✅
│   │   ├── Size: 16px
│   │   └── Color: #52c41a
│   │
│   ├── Message (Text Layer)
│   │   ├── Content: "保存成功"
│   │   ├── Style: Body / Regular
│   │   └── Color: #262626
│   │
│   └── Close Button (Icon, 可選)
│       ├── Icon: ✕
│       └── Size: 12x12px
│
└── Auto Layout Settings
    Direction: Horizontal
    Padding: 16px
    Item Spacing: 12px
    Alignment: Center
```

#### Variants 配置
```
Properties:
  - Type: Success, Error, Warning, Info
  - Has Close Button: False, True

Variant Combinations:
  Type × Close = 4 × 2 = 8 variants
```

#### 各類型規格

| 類型 | Fill | Stroke | Icon Color |
|------|------|--------|------------|
| Success | `#f6ffed` | `#b7eb8f` | `#52c41a` |
| Error | `#fff2f0` | `#ffccc7` | `#f5222d` |
| Warning | `#fffbe6` | `#ffe58f` | `#faad14` |
| Info | `#e6f7ff` | `#91d5ff` | `#1890ff` |

---

## ⏳ 加載組件（Loading）

### 1. Spinner

**Component 名稱**：`Loading / Spinner`

#### Figma 層級結構
```
Loading / Spinner / Medium (Frame)
└── Spinner (SVG 或 Plugin)
    ├── Size: 32x32px (Medium)
    ├── Stroke: 3px
    ├── Color: #1890ff
    └── Animation: Rotate (Prototype)
```

#### Variants 配置
```
Properties:
  - Size: Small, Medium, Large

Variant Combinations:
  Size = 3 variants
```

#### 各尺寸規格

| 尺寸 | Size | Stroke |
|------|------|--------|
| Small | 24x24px | 2px |
| Medium | 32x32px | 3px |
| Large | 48x48px | 4px |

---

### 2. Button Loading

**Component 名稱**：`Loading / Button`

#### Figma 層級結構
```
Loading / Button (Instance of Button / Primary)
├── Spinner (Instance of Loading / Spinner / Small)
└── Text
    ├── Content: "計算中..."
    └── Color: #ffffff
```

---

### 3. Page Loading

**Component 名稱**：`Loading / Page`

#### Figma 層級結構
```
Loading / Page (Frame, Auto Layout)
├── Overlay (Rectangle)
│   ├── Fill: rgba(255,255,255,0.8)
│   └── Fill Container
│
├── Loading Container (Frame, Auto Layout)
│   ├── Spinner (Instance of Loading / Spinner / Large)
│   │
│   └── Message (Text Layer)
│       ├── Content: "計算中，請稍候..."
│       ├── Style: Body / Regular
│       └── Color: #595959
│
└── Auto Layout Settings
    Direction: Vertical
    Item Spacing: 16px
    Alignment: Center
```

---

## 📋 組件使用檢查清單

### 按鈕
- [ ] 使用正確的按鈕類型（Primary/Secondary/Danger/Link）
- [ ] 使用正確的狀態（Default/Hover/Active/Disabled）
- [ ] 使用正確的尺寸（Small/Medium/Large）
- [ ] 文字簡潔明確

### 輸入框
- [ ] 使用正確的輸入類型（Text/Number/Date/With Unit）
- [ ] 標記必填字段（*）
- [ ] 顯示錯誤提示（如適用）
- [ ] 使用正確的狀態

### 單選按鈕
- [ ] 橫向排列（減少點擊）
- [ ] 清晰標記選中狀態
- [ ] 組間距一致（24px）

### 卡片
- [ ] 標題清晰
- [ ] 內容分組合理
- [ ] 間距一致

### 表格
- [ ] 表頭清晰
- [ ] 交替行顏色
- [ ] 金額右對齊
- [ ] Hover 狀態

### 彈窗
- [ ] 標題明確
- [ ] 操作按鈕清晰
- [ ] 可關閉

### 通知
- [ ] 使用正確的類型
- [ ] 文字簡潔
- [ ] 自動消失（3 秒）

---

**最後更新**：2026-03-24  
**狀態**：草稿
