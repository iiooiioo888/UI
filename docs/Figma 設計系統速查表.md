# Figma 設計系統速查表

> 快速參考指南，包含所有設計系統的顏色、字體、間距等規格。

---

## 🎨 顏色系統（Color Palette）

### 主色（Primary）

| 名稱 | 色值 | 預覽 | 用途 |
|------|------|------|------|
| Blue-500 | `#1890ff` | ▊ | 主按鈕、鏈接、焦點 |
| Blue-400 | `#40a9ff` | ▊ | Hover 狀態 |
| Blue-600 | `#096dd9` | ▊ | Active 狀態 |
| Blue-50 | `#e6f7ff` | ▊ | 淺藍背景 |

---

### 功能色（Functional）

| 名稱 | 色值 | 預覽 | 用途 |
|------|------|------|------|
| Green-500 | `#52c41a` | ▊ | 成功、正確 |
| Green-50 | `#f6ffed` | ▊ | 成功背景 |
| Yellow-500 | `#faad14` | ▊ | 警告、注意 |
| Yellow-50 | `#fffbe6` | ▊ | 警告背景 |
| Red-500 | `#f5222d` | ▊ | 錯誤、刪除 |
| Red-50 | `#fff2f0` | ▊ | 錯誤背景 |

---

### 中性色（Neutral）

| 名稱 | 色值 | 預覽 | 用途 |
|------|------|------|------|
| Gray-850 | `#262626` | ▊ | 標題、主文字 |
| Gray-600 | `#595959` | ▊ | 次要文字 |
| Gray-300 | `#d9d9d9` | ▊ | 邊框、分隔線 |
| Gray-100 | `#f5f5f5` | ▊ | 禁用背景 |
| Gray-50 | `#fafafa` | ▊ | 頁面背景 |
| White | `#ffffff` | ▊ | 卡片、按鈕背景 |

---

## 📏 字體系統（Typography）

### 標題（Headings）

| 名稱 | 字體 | 大小 | 粗細 | 行高 | 預覽 |
|------|------|------|------|------|------|
| H1 | Microsoft YaHei | 24px | 600 | 140% | **保單年結表查詢** |
| H2 | Microsoft YaHei | 20px | 600 | 140% | **【1. 保單資料】** |
| H3 | Microsoft YaHei | 16px | 600 | 140% | **表單分組標題** |

---

### 正文（Body）

| 名稱 | 字體 | 大小 | 粗細 | 行高 | 預覽 |
|------|------|------|------|------|------|
| Large | Microsoft YaHei | 16px | 400 | 150% | 重要正文內容 |
| Regular | Microsoft YaHei | 14px | 400 | 150% | 標準正文內容 |
| Small | Microsoft YaHei | 12px | 400 | 150% | 輔助文字、提示 |

---

### 數字/金額（Numbers）

| 名稱 | 字體 | 大小 | 粗細 | 行高 | 預覽 |
|------|------|------|------|------|------|
| Amount | Segoe UI | 14px | 400 | 150% | HKD 123,456.78 |
| Large Amount | Segoe UI | 20px | 600 | 140% | **HKD 140,802.45** |

---

## 📐 間距系統（Spacing）

| 名稱 | 值 | 預覽 | 用途 |
|------|-----|------|------|
| XS | 4px | ▊▊▊▊ | 緊湊間距 |
| SM | 8px | ▊▊▊▊▊▊▊▊ | 小間距 |
| MD | 16px | ▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊ | 標準間距 |
| LG | 24px | ▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊ | 大間距 |
| XL | 32px | ▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊ | 特大間距 |
| XXL | 48px | ▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊▊ | 頁面間距 |

---

## 🔲 圓角系統（Border Radius）

| 名稱 | 值 | 預覽 | 用途 |
|------|-----|------|------|
| None | 0px | ┌ | 無圓角 |
| Small | 4px | ╭ | 按鈕、輸入框 |
| Medium | 8px | ╭ | 卡片、彈窗 |
| Large | 12px | ╭ | 大型卡片 |
| Full | 999px | ╭ | 頭像、徽章 |

---

## 💫 陰影系統（Shadows）

| 名稱 | 值 | 預覽 | 用途 |
|------|------|------|------|
| Small | `0 2px 4px rgba(0,0,0,0.08)` | ▓ | 卡片、按鈕 Hover |
| Medium | `0 4px 8px rgba(0,0,0,0.12)` | ▓ | 下拉選單、彈窗 |
| Large | `0 8px 16px rgba(0,0,0,0.15)` | ▓ | 大型彈窗、浮層 |

---

## 🧩 組件庫速查

### 按鈕（Buttons）

| 類型 | 背景色 | 文字色 | 邊框 | 高度 |
|------|--------|--------|------|------|
| Primary | Blue-500 | White | None | 32px |
| Secondary | White | Gray-600 | Gray-300 | 32px |
| Danger | Red-500 | White | None | 32px |
| Link | None | Blue-500 | None | 自動 |

**狀態顏色**：
```
Default → Hover → Active → Disabled
Blue-500 → Blue-400 → Blue-600 → Gray-300
```

---

### 輸入框（Inputs）

| 狀態 | 邊框色 | 背景色 | 說明 |
|------|--------|--------|------|
| Default | Gray-300 | White | 正常狀態 |
| Hover | Blue-400 | White | 鼠標懸停 |
| Focus | Blue-500 | White | 輸入中（帶陰影） |
| Error | Red-500 | White | 驗證失敗 |
| Disabled | Gray-300 | Gray-100 | 禁用 |

**尺寸**：
```
Small: 24px
Medium: 32px
Large: 40px
```

---

### 單選按鈕（Radio）

| 狀態 | 邊框色 | 填充色 |
|------|--------|--------|
| Unchecked | Gray-300 | White |
| Checked | Blue-500 | Blue-500 |
| Hover | Blue-400 | White |
| Disabled | Gray-300 | Gray-100 |

**尺寸**：
```
外圈：16px
內圈：8px
```

---

### 卡片（Cards）

| 屬性 | 值 |
|------|-----|
| 背景 | White |
| 邊框 | 1px solid Gray-300 |
| 圓角 | 8px |
| 內邊距 | 24px |
| 陰影 | 可選 Small |

---

### 表格（Tables）

| 元素 | 背景色 | 文字色 | 高度 |
|------|--------|--------|------|
| Header | Gray-50 | Gray-850 | 40px |
| Row | White | Gray-850 | 40px |
| Row Alt | Gray-50 | Gray-850 | 40px |
| Hover | Blue-50 | Gray-850 | 40px |

---

### 彈窗（Modals）

| 屬性 | 值 |
|------|-----|
| 最小寬度 | 400px |
| 背景 | White |
| 圓角 | 8px |
| 陰影 | Medium |
| 遮罩 | rgba(0,0,0,0.45) |

---

### 通知提示（Notifications）

| 類型 | 背景色 | 邊框色 | 圖標色 |
|------|--------|--------|--------|
| Success | Green-50 | Green-300 | Green-500 |
| Error | Red-50 | Red-300 | Red-500 |
| Warning | Yellow-50 | Yellow-300 | Yellow-500 |
| Info | Blue-50 | Blue-300 | Blue-500 |

**尺寸**：
```
寬度：320px
內邊距：16px
```

---

## 📱 頁面模板尺寸

### 桌面端

```
畫布尺寸：1440 x 1024
最大寬度：1440px
側邊距：24px
```

### 響應式斷點

```
Desktop: ≥1440px
Tablet: 1024px - 1439px
Mobile: <1024px（不支持）
```

---

## 🎬 動畫規格

### 持續時間

| 類型 | 時長 |
|------|------|
| 快速（Hover、Click） | 100-200ms |
| 標準（頁面切換） | 300ms |
| 慢速（複雜動畫） | 500ms |

### 緩動函數

| 類型 | 函數 | 用途 |
|------|------|------|
| Ease In | cubic-bezier(0.4, 0, 1, 1) | 進入 |
| Ease Out | cubic-bezier(0, 0, 0.2, 1) | 離開 |
| Ease In Out | cubic-bezier(0.4, 0, 0.2, 1) | 進出 |
| Linear | linear | 匀速 |

---

## ♿ 無障礙設計

### 顏色對比度

| 等級 | 標準文字 | 大文字 |
|------|----------|--------|
| AA | 4.5:1 | 3:1 |
| AAA | 7:1 | 4.5:1 |

**推薦組合**：
- ✅ Gray-850 on White (15.6:1)
- ✅ Gray-600 on White (8.2:1)
- ✅ Blue-500 on White (4.5:1)
- ❌ Blue-400 on White (2.8:1) - 不符合

---

## 🔖 Figma 樣式命名規範

### Color Styles
```
格式：Category / Name - Shade
示例：
  - Primary / Blue - 500
  - Neutral / Gray - 300
  - Success / Green - 500
```

### Text Styles
```
格式：Category / Name - Size
示例：
  - Heading / H1 - 24px
  - Body / Regular - 14px
  - Number / Amount - 14px
```

### Effects
```
格式：Type / Size
示例：
  - Shadow / Small
  - Shadow / Medium
```

### Components
```
格式：Category / Name / State / Size
示例：
  - Button / Primary / Default / Medium
  - Input / Text / Focus / Large
  - Radio / Button / Checked
```

---

## 📊 設計稿檢查清單

### 顏色使用
- [ ] 所有顏色來自 Color Palette
- [ ] 對比度符合 AA 標準
- [ ] 功能色使用正確（成功=綠，錯誤=紅）

### 字體使用
- [ ] 所有文字使用 Text Styles
- [ ] 標題層級正確（H1 > H2 > H3）
- [ ] 金額使用 Segoe UI 字體

### 間距使用
- [ ] 所有間距使用 Spacing System
- [ ] 卡片間距一致（24px）
- [ ] 表單字段間距一致（16px）

### 組件使用
- [ ] 使用組件庫而非手繪
- [ ] 組件狀態正確
- [ ] 組件尺寸正確

### 無障礙
- [ ] 顏色對比度達標
- [ ] 錯誤提示不只靠顏色
- [ ] 所有輸入框有 Label

---

**最後更新**：2026-03-24  
**打印建議**：A4 橫向，方便貼在牆上參考
