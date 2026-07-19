# 🍀 大師筆記 Master Notes Skill

> 把課程、書籍、研究、報告、演講或多來源素材，轉成「看得懂、記得住、做得到」的高密度知識手冊。

**Master Notes** 不是單純摘要工具，而是一套「知識策展 × 教學設計 × 資訊設計」工作流。它會先讀完整來源、拆成知識原子，再規劃學習路徑、頁面架構、視覺元件與品質檢核，最後產出可直接製作成 PDF、PPTX、Canva 或 Markdown/YAML 的完整筆記系統。

---

## ✨ 它能做什麼

適合處理：

- 課程與研習筆記
- 書籍與長文整理
- 研究論文與報告
- 專案知識手冊
- AI 工具教學
- 品質管理與案例拆解
- 多份 PDF、網址、會議紀錄的整合整理

核心不是「把原文縮短」，而是重新設計讀者的學習路徑：

**定位 → 全局地圖 → 差距診斷 → 原理 → 方法 → 案例 → 可抄模板 → Recap 檢核**

---

## 🧠 核心工作流

```text
來源素材
   ↓
完整讀取與來源索引
   ↓
Knowledge Atoms 知識原子化
   ├─ Claim 核心主張
   ├─ Principle 原理
   ├─ Example 案例
   ├─ Quote 引用
   ├─ Data 數據
   ├─ Method 方法
   ├─ Risk 風險
   └─ Prompt 可抄模板
   ↓
提出 3 版敘事大綱
   ↓
選出最佳學習路徑
   ↓
建立逐頁 Page Map
   ↓
套用頁型與視覺元件
   ↓
100 分 Rubric 品質檢核
   ↓
PDF / PPTX / Canva / Markdown / YAML
```

---

## 🧩 內建 7 種頁型

| Page Archetype | 用途 |
|---|---|
| `cover` | 封面、定位、來源、篇章預告 |
| `overview` | 全局地圖、能力清單、關鍵記憶點 |
| `compare` | 新手 vs 高手、錯誤 vs 正確、方案比較 |
| `principles` | 原理、心法、規則、限制 |
| `matrix` | 決策矩陣、工具選擇、分類表 |
| `method` | 方法論、工作流、步驟與自檢 |
| `build` | 工具實作、App、分析、公式與迭代 |
| `recap` | Checklist、最後觀念、出處與 CTA |

---

## 🎨 內建視覺元件

- 篇章膠囊 `Kicker Pill`
- 新手 vs 高手雙欄比較卡
- 延伸案例 `Example Box`
- 可直接複製的 `Prompt Block`
- 原理／引用 `Quote Callout`
- 決策矩陣與比較表
- 風險提醒 `Warning`
- 收尾 `Checklist`
- 品牌 CTA Bar

預設視覺語言：A4 直式、米白紙感、深咖啡文字、琥珀橘強調，並以藍／綠／紅作為語意色。

---

## 📁 專案結構

```text
master-notes-skill/
├── README.md
├── SKILL.md
├── master-notes.yaml
├── templates/
│   ├── page-blueprints.yaml
│   └── master-prompt.md
└── examples/
    └── input-brief.yaml
```

### 檔案用途

| 檔案 | 說明 |
|---|---|
| `SKILL.md` | Skill 核心規則、啟用條件、完整執行流程 |
| `master-notes.yaml` | 設計 DNA：色彩、字體、元件、頁型、內容架構、Rubric |
| `templates/page-blueprints.yaml` | A4 各頁型的版面區域 Blueprint |
| `templates/master-prompt.md` | 不安裝 Skill 時也能直接使用的母提示詞 |
| `examples/input-brief.yaml` | 新專案的標準輸入範本 |

---

## 🚀 最簡單的使用方式

把這個資料夾交給支援 Skills 的 AI 工作環境，讓它先讀取 `SKILL.md` 與相關 YAML，再提供你的來源資料。

接著只要下指令：

```text
使用「大師筆記 Master Notes」整理這份資料。
先完整讀完來源，做素材拆解與 3 版大綱，
選出最適合的一版，再製作完整筆記手冊。
```

也可以指定：

```text
用大師筆記 Skill，把這 3 份 PDF 整理成 12 頁 A4 手冊。
讀者是第一次接觸這個主題的人。
每個核心概念都要有實際情境、可直接抄的 Prompt 與最後 Checklist。
品牌使用：🍀 Learn AI with Tarshar｜2026
```

---

## 📝 新專案輸入範例

編輯 `examples/input-brief.yaml`：

```yaml
project:
  title: "AI 品質工程師實戰筆記"
  audience: "製造業主管與品質人員"
  goal: "看完能用 AI 重新檢視品質防線"
  target_pages: 12
  output: "PDF"

source:
  files: []
  urls: []
  notes: []

brand:
  owner: "Tarshar"
  logo_text: "🍀 Learn AI with Tarshar｜2026"
```

---

## ✅ 品質閘門

輸出前使用 100 分 Rubric 檢核：

| 評分項目 | 分數 |
|---|---:|
| 結構清晰 | 20 |
| 內容含金量 | 20 |
| 案例轉譯 | 15 |
| 視覺層級 | 15 |
| 可讀性 | 15 |
| 可複用性 | 15 |
| **合格門檻** | **85** |

低於 85 分時，應先找出最低分的兩項修正，再交付成品。

---

## 🔑 大師筆記的 5 個原則

1. **先讀完，再整理**：不能只看目錄或零碎片段就開始寫。
2. **先大綱，再成品**：方向錯誤要在低成本階段先抓出來。
3. **一頁一個核心問題**：避免把頁面塞成文字牆。
4. **概念一定要落地**：原理後面要接案例、方法或可直接使用的模板。
5. **來源與延伸要分開**：原作者觀念、整理者解讀與自創案例必須清楚標示。

---

## 🛡️ 來源與使用說明

本 Skill 的資訊架構，是從一份高密度 AI 學習筆記的編排方式中抽象出可重複使用的設計規則，再重新建構為通用工作流。

- 本專案不包含原始教材全文或原始版面素材。
- 原始課程、引用與案例之著作權仍屬原作者及原權利人。
- 本 Skill 為獨立整理與方法設計，非 Andrew Ng、DeepLearning.AI 或原筆記作者之官方產品。
- 使用外部來源製作筆記時，請保留來源、引用與授權資訊。

---

## 🍀 Brand

**Learn AI with Tarshar｜2026**

把資訊整理成知識，把知識變成可以真正使用的方法。
