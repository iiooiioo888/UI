# Figma 設計實戰工作手冊

> 邊做邊參考的速查手冊，包含所有關鍵信息和常見問題解答。

---

## 🚀 快速啟動清單

### 開始前準備（2 分鐘）
- [ ] 打開瀏覽器（Chrome/Edge/Safari）
- [ ] 訪問 https://figma.com
- [ ] 登入 Figma 賬號（沒有就註冊，免費）
- [ ] 打開本文檔（保持在旁邊）
- [ ] 準備好筆記應用（記錄問題）

### 創建新文件（1 分鐘）
- [ ] 點擊右上角「+」→「Design File」
- [ ] 命名：「年結表計算器 UI 設計」
- [ ] 保存到團隊項目或個人草稿

---

## 📐 關鍵數值速查

### 顏色代碼
```
主色：
  Blue-500: #1890ff  ← 最常用
  Blue-400: #40a9ff
  Blue-600: #096dd9

功能色：
  Green-500: #52c41a  ← 成功
  Yellow-500: #faad14 ← 警告
  Red-500: #f5222d    ← 錯誤

中性色：
  Gray-850: #262626  ← 標題
  Gray-600: #595959  ← 正文
  Gray-300: #d9d9d9  ← 邊框
  Gray-100: #f5f5f5  ← 禁用
  Gray-50: #fafafa   ← 背景
```

### 字體大小
```
標題：
  H1: 24px, 600
  H2: 20px, 600
  H3: 16px, 600

正文：
  Large: 16px, 400
  Regular: 14px, 400  ← 最常用
  Small: 12px, 400

數字：
  Amount: 14px, Segoe UI
  Large Amount: 20px, Segoe UI, 600
```

### 常用間距
```
4px   - 緊湊間距
8px   - 小間距
16px  - 標準間距  ← 最常用
24px  - 大間距    ← 卡片內邊距
32px  - 特大間距
48px  - 頁面間距
```

### 圓角
```
4px   - 按鈕、輸入框
8px   - 卡片、彈窗
999px - 頭像、徽章（Full）
```

### 陰影
```
Small:  0 2px 4px rgba(0,0,0,0.08)
Medium: 0 4px 8px rgba(0,0,0,0.12)
Large:  0 8px 16px rgba(0,0,0,0.15)
```

---

## ⌨️ Figma 快捷鍵速查

### 通用快捷鍵
```
Ctrl+S      - 保存（Figma 自動保存，但養成習慣）
Ctrl+Z      - 撤銷
Ctrl+Y      - 重做
Ctrl+C      - 複製
Ctrl+V      - 粘貼
Ctrl+D      - 重複複製
Delete      - 刪除
```

### 創建工具
```
F           - Frame（畫布）
R           - Rectangle（矩形）
T           - Text（文字）
E           - Ellipse（橢圓）
I           - Image（圖片）
```

### 操作快捷鍵
```
V           - Move（移動工具）
A           - Artboard（畫板）
Ctrl+G      - 分組
Ctrl+Alt+G  - 取消分組
Ctrl+Alt+K  - 創建組件 ⭐ 重要
Shift+A     - Auto Layout ⭐ 重要
```

### 視圖控制
```
空格 + 拖動  - 平移視圖
滾輪        - 縮放
Shift + 2   - 適應選中內容
Shift + 1   - 適應所有內容
```

### 對齊工具
```
Ctrl+Alt+H  - 水平居中
Ctrl+Alt+V  - 垂直居中
```

---

## 🎨 設計系統創建速查

### Color Styles 創建步驟
```
1. 繪製矩形（80x80）
2. 填充顏色（如：#1890ff）
3. 右側面板 → Styles 標籤
4. 點擊「+」號
5. 輸入名稱：Primary / Blue - 500
6. 點擊 Create style
7. 重複以上步驟創建其他顏色
```

### Text Styles 創建步驟
```
1. 按 T 創建文字
2. 設置字體屬性（如：Microsoft YaHei, 24px, 600）
3. 右側面板 → Text Styles 標籤
4. 點擊「+」號
5. 輸入名稱：Heading / H1 - 24px
6. 點擊 Create style
```

### Effects 創建步驟
```
1. 繪製矩形（100x100）
2. 右側面板 → Effects 標籤
3. 點擊「+」→ Drop Shadow
4. 設置參數（如：0 2px 4px rgba(0,0,0,0.08)）
5. Styles → 「+」→ 命名：Shadow / Small
```

---

## 🧩 組件創建速查

### 按鈕組件創建
```
1. 按 Shift+A 創建 Auto Layout Frame
2. 設置 Direction: Horizontal
3. 添加 Rectangle（填充：#1890ff，圓角：4px）
4. 添加 Text（「計算」，白色）
5. 設置 Padding: 8px 16px
6. 右鍵 → Create Component（Ctrl+Alt+K）
7. 右側面板 → Variants → 「+」
8. 添加屬性：State, Size
9. 複製並修改每個變體
```

### 輸入框組件創建
```
1. 創建 Frame（寬度 200px，高度 32px）
2. 添加 Rectangle（白色背景，灰色邊框）
3. 添加 Text（Placeholder）
4. 設置 Auto Layout
5. Create Component
6. 添加 Variants：State, Size
```

---

## 📱 頁面設計速查

### 查詢輸入頁佈局
```
頂部導航欄：64px
頁面標題區：56px
卡片 1（保單資料）：400px
卡片 2（賬戶價值）：250px
卡片 3（其他）：80px（收起）
底部按鈕區：50px
總高度：約 900px
```

### 結果展示頁佈局
```
頂部導航欄：64px
頁面標題區：56px
操作按鈕區：50px
保單資料表格：150px
戶口價值表格：300px
說明摘要：250px
底部按鈕區：50px
總高度：約 870px
```

---

## 🔍 常見問題解答

### Q1: 如何創建 Auto Layout？
```
方法 1：選中對象 → Shift+A
方法 2：右鍵 → Add auto layout
方法 3：創建 Frame 時選擇 Auto Layout

設置：
- Direction: Horizontal（橫向）或 Vertical（縱向）
- Padding: 內邊距
- Item Spacing: 項目間距
- Alignment: 對齊方式
```

### Q2: 如何創建組件（Component）？
```
1. 設計好元素
2. 選中所有相關圖層
3. 右鍵 → Create Component
4. 或快捷鍵：Ctrl+Alt+K
5. 組件會變成菱形圖標 <>
```

### Q3: 如何創建 Variants？
```
1. 創建第一個組件
2. 右側面板 → Variants 標籤
3. 點擊「+」號
4. 添加屬性（如：State）
5. 添加變體值（如：Default, Hover）
6. 複製組件（Ctrl+D）
7. 修改每個變體的樣式
```

### Q4: 如何使用組件實例？
```
1. 左側 Assets 面板（或按 Shift+I）
2. 找到需要的組件
3. 拖動到畫布上
4. 這就是實例（Instance）
5. 修改實例不會影響原組件
```

### Q5: 如何修改組件？
```
1. 雙擊組件（進入編輯模式）
2. 或右鍵 → Go to main component
3. 修改後所有實例自動更新
```

### Q6: Auto Layout 的 Hug 和 Fill 有什麼區別？
```
Hug Contents: 框架適應內容大小
Fixed: 固定大小
Fill Container: 填滿父容器

建議：
- 按鈕：Hug
- 表單字段：Fill
- 卡片：Fill
```

### Q7: 如何對齊元素？
```
方法 1：選中多個元素 → 使用頂部對齊工具
方法 2：使用快捷鍵
  - Ctrl+Alt+H: 水平居中
  - Ctrl+Alt+V: 垂直居中
方法 3：手動輸入坐標
```

### Q8: 如何創建陰影？
```
1. 選中對象
2. 右側面板 → Effects 標籤
3. 點擊「+」→ Drop Shadow
4. 設置參數：
   - X: 水平偏移
   - Y: 垂直偏移
   - Blur: 模糊度
   - Spread: 擴散
   - Color: 顏色和透明度
```

### Q9: 如何導出圖片？
```
1. 選中 Frame 或元素
2. 右側面板 → Export 標籤
3. 點擊「+」
4. 選擇格式（PNG/JPG/SVG）
5. 選擇倍數（1x/2x）
6. 點擊 Export 按鈕
```

### Q10: 如何分享設計稿？
```
1. 右上角 Share 按鈕
2. 設置權限：
   - Can view: 僅查看
   - Can comment: 可評論
   - Can edit: 可編輯
3. 複製鏈接
4. 發送給團隊成員
```

---

## ⚠️ 常見錯誤與避免方法

### 錯誤 1: 沒有使用 Auto Layout
```
問題：元素對齊困難，調整大小麻煩
解決：所有組件和卡片都使用 Auto Layout
```

### 錯誤 2: 組件命名不規範
```
問題：找不到組件，開發人員困惑
解決：使用規範命名：Category / Name / State / Size
```

### 錯誤 3: 沒有創建 Variants
```
問題：組件太多，難以管理
解決：使用 Variants 管理狀態和尺寸
```

### 錯誤 4: 顏色和字體沒有創建 Styles
```
問題：修改設計時要手動更新所有地方
解決：一開始就創建 Color Styles 和 Text Styles
```

### 錯誤 5: 圖層命名混亂
```
問題：找不到需要的圖層
解決：及時命名圖層和分組
```

### 錯誤 6: 沒有使用組件
```
問題：重複元素多，修改困難
解決：重複使用的元素都創建為組件
```

---

## 💡 設計小技巧

### 技巧 1: 使用網格系統
```
設置：
- Layout Grid: Columns
- Count: 12
- Gutter: 24px
- Margin: 24px
```

### 技巧 2: 使用約束（Constraints）
```
設置：
- 選擇元素
- 右側面板 → Constraints
- 設置水平和垂直約束
- 響應式設計必備
```

### 技巧 3: 使用插件提高效率
```
推薦插件：
- Unsplash: 免費圖片
- Material Design Icons: 圖標庫
- Content Reel: 填充內容
- Autoflow: 繪製流程線
- Stark: 無障礙檢查
```

### 技巧 4: 使用版本歷史
```
操作：
- 右上角菜單 → Show version history
- 重要節點創建版本
- 可以回滾到任何版本
```

### 技巧 5: 使用組件屬性
```
設置：
- 選擇組件
- 右側面板 → Component properties
- 添加屬性（Text, Boolean, Instance）
- 實例可以直接修改屬性
```

---

## 📊 進度追蹤表

### 設計系統（30 分鐘）
- [ ] Color Styles（11 個）
- [ ] Text Styles（8 個）
- [ ] Spacing（6 個）
- [ ] Effects（3 個）
- 完成時間：____

### 組件庫（60 分鐘）
- [ ] Buttons（4 類）
- [ ] Inputs（4 類）
- [ ] Radio Buttons（2 類）
- [ ] Cards（2 類）
- [ ] Tables（2 類）
- [ ] Modals（3 類）
- [ ] Notifications（4 類）
- [ ] Loading（3 類）
- 完成時間：____

### 頁面設計（90 分鐘）
- [ ] 首頁
- [ ] 查詢輸入頁
- [ ] 結果展示頁
- [ ] 管理後台頁
- [ ] 系統管理頁
- 完成時間：____

### 交互原型（30 分鐘）
- [ ] 頁面連接
- [ ] 組件交互
- [ ] 動畫設置
- 完成時間：____

### 檢查與導出（15 分鐘）
- [ ] 設計檢查
- [ ] 資源導出
- [ ] 團隊分享
- 完成時間：____

**總完成時間**：____

---

## 🆘 遇到問題怎麼辦？

### 問題類型 1: 操作問題
```
解決方法：
1. 查看本文檔的「常見問題解答」
2. Google: "Figma how to [你的問題]"
3. Figma 官方教程：https://help.figma.com
4. YouTube 搜索：Figma tutorial
```

### 問題類型 2: 設計問題
```
解決方法：
1. 參考「UI 設計規範.md」
2. 參考「Figma 設計系統速查表.md」
3. 查看競品設計
4. 詢問團隊成員
```

### 問題類型 3: 技術問題
```
解決方法：
1. 刷新瀏覽器
2. 清除緩存
3. 重啟 Figma
4. 聯繫 Figma 支持
```

---

## 🎯 設計完成檢查清單

### 設計系統
- [ ] 所有 Color Styles 已創建
- [ ] 所有 Text Styles 已創建
- [ ] 所有 Effects 已創建
- [ ] 樣式命名規範

### 組件庫
- [ ] 所有組件已創建
- [ ] Variants 設置正確
- [ ] 組件命名規範
- [ ] Auto Layout 設置正確

### 頁面設計
- [ ] 所有頁面已設計
- [ ] 佈局正確
- [ ] 使用設計系統
- [ ] 使用組件庫
- [ ] 無用圖層已清理

### 交互原型
- [ ] 頁面連接完成
- [ ] 組件交互完成
- [ ] 動畫設置完成
- [ ] 原型測試通過

### 交付準備
- [ ] 設計稿導出
- [ ] 資源導出
- [ ] 分享給團隊
- [ ] 文檔更新

---

## 📞 需要幫助？

如果遇到無法解決的問題：

1. **記錄問題**：截圖 + 描述
2. **查看文檔**：14 個設計文檔可能已有答案
3. **搜索網絡**：Google / YouTube
4. **詢問團隊**：分享你的 Figma 鏈接

---

**開始時間**：____  
**預計完成**：____  
**實際完成**：____

**設計師**：____  
**日期**：____

**備註**：
_________________________________
_________________________________
_________________________________

---

**最後更新**：2026-03-24  
**狀態**：可用  
**版本**：1.0
