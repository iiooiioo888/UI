# Figma 設計稿創建指南

> 本文檔指導如何在 Figma 中創建年結表計算器的設計稿、組件庫和設計系統。

---

## 📋 準備工作

### 1. 創建 Figma 文件

**步驟**：
1. 登入 Figma (https://figma.com)
2. 點擊「+ Design File」
3. 命名為：`年結表計算器 UI 設計`
4. 選擇團隊項目（如有）或個人草稿

---

### 2. 設置文件結構

**創建頁面（Pages）**：
```
📄 Cover                    # 封面頁
📄 Design System            # 設計系統
📄 Components               # 組件庫
📄 首頁                     # 首頁設計
📄 查詢輸入頁                # 核心頁面
📄 結果展示頁                # 結果頁面
📄 管理後台                  # 管理頁面
📄 Prototype                # 交互原型
📄 Archive                  # 存檔（舊版本）
```

---

## 🎨 設計系統（Design System）

### 1. 創建 Color Styles

**路徑**：Design System 頁面 → 創建 Frame → 命名為「Colors」

#### 主色（Primary）
```
名稱：Primary / Blue-500
色值：#1890ff
用途：主按鈕、鏈接、焦點狀態

名稱：Primary / Blue-400
色值：#40a9ff
用途：Hover 狀態

名稱：Primary / Blue-600
色值：#096dd9
用途：Active 狀態
```

#### 功能色（Functional）
```
名稱：Success / Green-500
色值：#52c41a

名稱：Warning / Yellow-500
色值：#faad14

名稱：Error / Red-500
色值：#f5222d
```

#### 中性色（Neutral）
```
名稱：Neutral / Gray-850
色值：#262626
用途：標題、主要文字

名稱：Neutral / Gray-600
色值：#595959
用途：次要文字

名稱：Neutral / Gray-300
色值：#d9d9d9
用途：邊框

名稱：Neutral / Gray-100
色值：#f5f5f5
用途：禁用背景

名稱：Neutral / Gray-50
色值：#fafafa
用途：頁面背景
```

**操作步驟**：
1. 繪製矩形（80x80px）
2. 填充對應顏色
3. 右側面板 → Styles → 「+」→ 命名
4. 重複以上步驟創建所有顏色

---

### 2. 創建 Text Styles

**路徑**：Design System 頁面 → 創建 Frame → 命名為「Typography」

#### 標題（Headings）
```
名稱：Heading / H1
字體：Microsoft YaHei
大小：24px
粗細：600
行高：140%
用途：頁面標題

名稱：Heading / H2
字體：Microsoft YaHei
大小：20px
粗細：600
行高：140%
用途：卡片標題

名稱：Heading / H3
字體：Microsoft YaHei
大小：16px
粗細：600
行高：140%
用途：分組標題
```

#### 正文（Body）
```
名稱：Body / Large
字體：Microsoft YaHei
大小：16px
粗細：400
行高：150%
用途：重要正文

名稱：Body / Regular
字體：Microsoft YaHei
大小：14px
粗細：400
行高：150%
用途：標準正文

名稱：Body / Small
字體：Microsoft YaHei
大小：12px
粗細：400
行高：150%
用途：輔助文字、提示
```

#### 數字/金額（Numbers）
```
名稱：Number / Amount
字體：Segoe UI
大小：14px
粗細：400
行高：150%
用途：金額顯示

名稱：Number / Large Amount
字體：Segoe UI
大小：20px
粗細：600
行高：140%
用途：總金額、突出顯示
```

**操作步驟**：
1. 使用文字工具（T）創建文本
2. 設置字體屬性
3. 右側面板 → Text Styles → 「+」→ 命名
4. 重複以上步驟創建所有字體樣式

---

### 3. 創建間距系統（Spacing）

**路徑**：Design System 頁面 → 創建 Frame → 命名為「Spacing」

```
名稱：Spacing / XS
值：4px

名稱：Spacing / SM
值：8px

名稱：Spacing / MD
值：16px

名稱：Spacing / LG
值：24px

名稱：Spacing / XL
值：32px

名稱：Spacing / XXL
值：48px
```

**操作步驟**：
1. 繪製矩形，寬度為間距值，高度 4px
2. 填充顏色（建議用灰色 #d9d9d9）
3. 添加文字標籤（如「4px」）
4. 右側面板 → 創建 Styles（可選）

---

### 4. 創建陰影（Effects）

**路徑**：Design System 頁面 → 創建 Frame → 命名為「Shadows」

```
名稱：Shadow / Small
值：0 2px 4px rgba(0,0,0,0.08)
用途：卡片、按鈕 Hover

名稱：Shadow / Medium
值：0 4px 8px rgba(0,0,0,0.12)
用途：下拉選單、彈窗

名稱：Shadow / Large
值：0 8px 16px rgba(0,0,0,0.15)
用途：大型彈窗、浮層
```

**操作步驟**：
1. 繪製矩形（100x100px）
2. 右側面板 → Effects → 「+」→ Drop Shadow
3. 設置參數
4. 右側面板 → Styles → 「+」→ 命名

---

## 🧩 組件庫（Components）

### 1. 按鈕（Button）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Buttons」

#### 主按鈕（Primary Button）

**步驟**：
1. 創建 Frame（寬度自動，高度 32px）
2. 添加矩形填充（Auto Layout）
3. 填充色：Primary / Blue-500
4. 圓角：4px
5. 添加文字：「計算」
6. 文字樣式：Body / Regular，白色
7. 添加 Auto Layout（間距 8px）
8. 右側面板 → Create Component（Ctrl+Alt+K）

**創建 Variants**：
```
屬性：State
- Default（背景：Blue-500）
- Hover（背景：Blue-400）
- Active（背景：Blue-600）
- Disabled（背景：Gray-300，文字：Gray-100）
- Loading（背景：Blue-500，添加 spinner）
```

**尺寸 Variants**：
```
屬性：Size
- Small（高度 24px，文字 12px）
- Medium（高度 32px，文字 14px）
- Large（高度 40px，文字 16px）
```

---

#### 次要按鈕（Secondary Button）

**步驟**：同主按鈕，但：
- 填充色：白色
- 邊框：1px solid Gray-300
- 文字色：Gray-600

**Variants**：
```
State: Default / Hover / Active / Disabled
Hover: 邊框 Blue-500，文字 Blue-500
```

---

#### 危險按鈕（Danger Button）

**步驟**：同主按鈕，但：
- 填充色：Red-500
- Hover: Red-400
- Active: Red-600

---

#### 鏈接按鈕（Link Button）

**步驟**：
1. 僅文字，無背景
2. 文字色：Blue-500
3. Hover: 添加下劃線

---

### 2. 輸入框（Input）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Inputs」

#### 文本輸入框

**步驟**：
1. 創建 Frame（寬度 200px，高度 32px）
2. 添加矩形填充
3. 填充色：白色
4. 邊框：1px solid Gray-300
5. 圓角：4px
6. 添加文字（Placeholder）：「請輸入...」
7. 文字樣式：Body / Regular，Gray-600
8. 添加 Auto Layout（內邊距 8px 12px）
9. Create Component

**創建 Variants**：
```
屬性：State
- Default（邊框：Gray-300）
- Hover（邊框：Blue-400）
- Focus（邊框：Blue-500，陰影：Small）
- Error（邊框：Red-500，下方顯示錯誤文字）
- Disabled（背景：Gray-100，邊框：Gray-300）

屬性：Size
- Small（高度 24px）
- Medium（高度 32px）
- Large（高度 40px）
```

---

#### 數字輸入框

**步驟**：
1. 基於文本輸入框
2. 文字右對齊
3. 右側添加上下箭頭圖標（可選）

---

#### 日期輸入框

**步驟**：
1. 基於文本輸入框
2. 左側添加日曆圖標（📅）
3. 格式：YYYY-MM-DD

**添加圖標**：
- 使用 Figma 內置圖標插件（如 Material Design Icons）
- 或導入 SVG 圖標

---

#### 帶單位輸入框

**步驟**：
1. 基於文本輸入框
2. 右側添加單位標籤（HKD/USD/歲）
3. 單位背景：Gray-50
4. 單位文字：Body / Small，Gray-600

---

### 3. 單選按鈕（Radio Button）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Radio Buttons」

**步驟**：
1. 繪製圓圈（16x16px）
2. 邊框：1px solid Gray-300
3. 填充：白色
4. 右側添加文字標籤
5. Create Component

**創建 Variants**：
```
屬性：State
- Unchecked（邊框：Gray-300）
- Checked（邊框：Blue-500，填充：Blue-500，中心白色小圓 8x8px）
- Hover（邊框：Blue-400）
- Disabled（邊框：Gray-300，填充：Gray-100）
```

---

### 4. 卡片（Card）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Cards」

#### 標準卡片

**步驟**：
1. 創建 Frame（寬度自動）
2. 填充：白色
3. 邊框：1px solid Gray-300
4. 圓角：8px
5. 添加 Auto Layout（內邊距 24px）
6. Create Component

---

#### 可折疊卡片

**步驟**：
1. 基於標準卡片
2. 頂部添加標題和展開/收起按鈕
3. 內容區域設置為可隱藏

---

### 5. 表格（Table）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Tables」

#### 表格行（Table Row）

**步驟**：
1. 創建 Frame（高度 40px）
2. 添加 Auto Layout（橫向）
3. 添加單元格（內邊距 12px 16px）
4. Create Component

**Variants**：
```
屬性：Type
- Header（背景：Gray-50，文字粗體）
- Row（背景：白色）
- Row Alt（背景：Gray-50）
- Hover（背景：Blue-50）
```

---

### 6. 彈窗（Modal）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Modals」

#### 確認彈窗

**步驟**：
1. 創建 Frame（寬度 400px）
2. 填充：白色
3. 圓角：8px
4. 陰影：Shadow / Medium
5. 添加 Auto Layout（內邊距 24px）
6. 添加標題、內容、按鈕區
7. Create Component

---

#### 錯誤彈窗

**步驟**：同確認彈窗，但：
- 標題左側添加錯誤圖標（紅色）
- 標題文字：Red-500

---

### 7. 通知提示（Notification）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Notifications」

**步驟**：
1. 創建 Frame（寬度 320px，高度自動）
2. 填充：根據類型（成功：Green-50 背景）
3. 邊框：對應顏色
4. 添加 Auto Layout（內邊距 16px）
5. 左側圖標 + 文字 + 關閉按鈕
6. Create Component

**Variants**：
```
屬性：Type
- Success（綠色）
- Error（紅色）
- Warning（黃色）
- Info（藍色）
```

---

### 8. 加載狀態（Loading）

**路徑**：Components 頁面 → 創建 Frame → 命名為「Loading」

#### Spinner

**步驟**：
1. 使用橢圓工具繪製圓環
2. 或使用 Figma 插件（如 Loading Spinner）
3. 顏色：Blue-500
4. Create Component

---

#### 按鈕加載

**步驟**：
1. 基於主按鈕
2. 文字左側添加 Spinner
3. 文字改為「計算中...」

---

## 📱 頁面設計

### 1. 創建畫布（Frames）

**路徑**：對應頁面（如「查詢輸入頁」）

**步驟**：
1. 按 F 創建 Frame
2. 選擇桌面尺寸：Desktop（1440x1024）
3. 命名：「查詢輸入頁 - 1920x1080」

---

### 2. 查詢輸入頁設計

**步驟**：

#### 頂部導航欄
```
1. 創建 Frame（1440x64px）
2. 填充：白色
3. 邊框底：1px solid Gray-100
4. 左側：Logo + 系統名稱
5. 右側：用戶頭像 + 姓名
```

#### 頁面標題區
```
1. 創建 Frame（1440x56px）
2. 填充：Gray-50
3. 左側：← 返回按鈕（使用組件）
4. 中間：「保單年結表查詢」（H2）
```

#### 表單卡片 1：保單資料
```
1. 從組件庫拖入「Card」組件
2. 設置 Auto Layout
3. 添加標題：「【1. 保單資料】」（H3）
4. 添加表單字段（使用 Input、Radio 組件）
5. 三列佈局（使用 Auto Layout 或 Grid）
```

**字段清單**：
- 退保日期（日期輸入框）
- 繳至日期（日期輸入框）
- 產品名稱（下拉選單）
- 保單生效日（日期輸入框）
- 年齡（數字輸入框）
- 性別（單選按鈕組）
- 吸煙狀態（單選按鈕組）
- 投保金額（數字輸入框）
- 幣種（單選按鈕組）
- 繳費方式（單選按鈕組）

---

#### 表單卡片 2：賬戶價值
```
同卡片 1，字段：
- 紅利結餘（數字輸入框 + 日期）
- 現金儲值結餘（數字輸入框 + 日期）
- 貸款結餘（數字輸入框 + 日期）
- 已繳保費（數字輸入框）
```

---

#### 表單卡片 3：其他（可折疊）
```
1. 使用「可折疊卡片」組件
2. 默認收起狀態
3. 展開後顯示附加字段
```

---

#### 底部按鈕區
```
1. 創建 Frame（右對齊）
2. 拖入「Secondary Button」組件（重置）
3. 拖入「Primary Button」組件（計算）
4. 間距：16px
```

---

### 3. 結果展示頁設計

**步驟**：

#### 操作按鈕區
```
1. 創建 Frame（橫向）
2. 拖入按鈕組件：
   - 📄 導出 PDF
   - 🖨️ 列印
   - ✉️ 發送郵件
   - 🔄 重新計算
3. 間距：16px
```

---

#### 保單資料表格
```
1. 使用 Table 組件
2. 4 列：產品名稱、保單生效日、年齡、性別
3. 表頭 + 1 行數據
```

---

#### 保單戶口價值表格
```
1. 使用 Table 組件
2. 2 列：項目、金額
3. 金額列右對齊
4. 行數：現金價值、紅利結餘、終期紅利、退保價值
```

---

#### 說明摘要
```
1. 創建 Frame
2. 使用 Bullet Points
3. 文字樣式：Body / Regular
```

---

## 🔗 交互原型（Prototype）

### 1. 連接頁面

**步驟**：
1. 切換到 Prototype 標籤
2. 選擇按鈕組件
3. 拖動連接線到目標 Frame
4. 設置交互：
   - Trigger: On Click
   - Animation: Smart Animate
   - Easing: Ease Out
   - Duration: 300ms

---

### 2. 添加交互

#### 表單驗證
```
1. 創建錯誤狀態的 Frame
2. 連接：輸入框 → On Blur → 錯誤狀態 Frame
3. 添加錯誤提示動畫
```

---

#### 計算流程
```
1. 計算按鈕 → On Click → 加載狀態 Frame
2. 加載狀態 → After Delay (2000ms) → 結果頁
3. 或 → 錯誤彈窗
```

---

### 3. 設置過渡動畫

```
頁面切換：Smart Animate，Ease Out，300ms
彈窗出現：Ease Out，200ms
卡片展開：Ease In Out，300ms
```

---

## 📤 導出與分享

### 1. 導出設計稿

**步驟**：
1. 選擇要導出的 Frame
2. 右側面板 → Export
3. 格式：PNG / PDF / SVG
4. 倍數：1x, 2x（可選）
5. 點擊 Export

---

### 2. 分享給團隊

**步驟**：
1. 右上角 Share 按鈕
2. 設置權限：
   - Can view：僅查看
   - Can comment：可評論
   - Can edit：可編輯
3. 複製鏈接
4. 發送給團隊成員

---

### 3. 開發人員移交（Handoff）

**步驟**：
1. 開發人員打開 Figma 鏈接
2. 右側面板 → Inspect
3. 查看 CSS 代碼、尺寸、顏色
4. 導出所需資源（圖標、圖片）

---

## 🎯 Figma 插件推薦

### 1. 圖標插件
- **Material Design Icons** - Google Material 圖標庫
- **Iconify** - 超過 100,000 個圖標
- **Feather Icons** - 簡約風格圖標

### 2. 內容填充插件
- **Content Reel** - 自動填充虛擬數據
- **Mockaroo** - 生成真實感數據

### 3. 效率插件
- **Autoflow** - 自動繪製流程線
- **Sticky Notes** - 添加註釋
- **A11y - Color Contrast Checker** - 無障礙對比度檢查

### 4. 設計系統插件
- **Style Organizer** - 整理樣式
- **Design Lint** - 檢查設計規範

---

## 📋 設計稿檢查清單

### 設計系統
- [ ] 所有 Color Styles 已創建
- [ ] 所有 Text Styles 已創建
- [ ] Spacing 系統已定義
- [ ] Shadow 系統已定義

### 組件庫
- [ ] 按鈕（所有狀態和尺寸）
- [ ] 輸入框（所有類型和狀態）
- [ ] 單選按鈕
- [ ] 卡片
- [ ] 表格
- [ ] 彈窗
- [ ] 通知提示
- [ ] 加載狀態

### 頁面設計
- [ ] 首頁
- [ ] 查詢輸入頁
- [ ] 結果展示頁
- [ ] 管理後台頁
- [ ] 系統管理頁

### 交互原型
- [ ] 頁面跳轉連接
- [ ] 表單驗證流程
- [ ] 計算加載流程
- [ ] 彈窗交互

### 交付準備
- [ ] 所有 Frame 命名規範
- [ ] 圖層分組清晰
- [ ] 無用圖層已清理
- [ ] 已添加註釋說明
- [ ] 已分享給團隊

---

**最後更新**：2026-03-24  
**狀態**：草稿
