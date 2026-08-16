# ISO 26262 × ASPICE 繁中教學站

把汽車電子領域最常被同時要求的兩套規範做成**系統化深度教學**：**ISO 26262**（功能安全）管「安不安全」，**ASPICE**（軟體開發流程）管「做得好不好」，兩者在同一條 V-model 上匯流。每個單元都附可照做的 **Worked Example**。

- 目標讀者：車用電子軟體工程師 / 功能安全工程師 / 流程品質工程師 / 學生
- 單元數：20 深度單元（L0 → L5）
- 授權：本站內容 CC-BY-4.0
- 網站：[https://shumingyang-opencode.github.io/iso26262-aspice-tech-zh-tw/](https://shumingyang-opencode.github.io/iso26262-aspice-tech-zh-tw/)

## 網站結構

```
iso26262-aspice-tech-zh-tw/
├── index.html            # 課程總覽 + 入口卡片
├── map.html              # 概念地圖：雙規範全景
├── learning-path.html    # 學習路線：L0 → L5 六層
├── glossary.html         # 📖 術語表
├── processes.html        # 🗂️ 過程速查（ASPICE ↔ ISO ↔ 交付物）
├── standards.html        # 🏛️ 標準對照（12 parts ↔ 過程群 ↔ ASIL）
├── about.html            # 關於本站
├── docs/                 # 單元教學頁
│   ├── index.html        # 單元一覽
│   └── unit-01.html … unit-20.html
├── assets/site.css       # 單一共享樣式
└── .nojekyll
```

## 單元列表（20 單元）

| Lv | 單元 | 內容 |
|----|------|------|
| L0 | 1 | 概論：為什麼需要 ISO 26262 與 ASPICE（V-model、雙規範分工） |
| L0 | 2 | ISO 26262 全景：12 parts、安全生命週期、ASIL |
| L0 | 3 | ASPICE 全景：過程群、CL0–5、N/P/L/F 評分 |
| L1 | 4 | 概念階段：Item 定義與 HARA（AEB Worked Example） |
| L1 | 5 | 安全目標與安全需求（SG→FSR→TSR、ASIL 分解） |
| L1 | 6 | SYS.1–SYS.3：需求擷取、系統需求、系統架構 |
| L1 | 7 | SYS.4/SYS.5：系統整合與資格測試 |
| L2 | 8 | SWE.1 軟體需求分析（軟體需求規格、雙向追溯） |
| L2 | 9 | SWE.2 軟體架構設計（freedom from interference、分區） |
| L2 | 10 | SWE.3 詳細設計與建置（MISRA C、防禦式設計） |
| L2 | 11 | SWE.4 軟體單元驗證（靜態分析、單元測試、覆蓋率） |
| L2 | 12 | SWE.5 軟體整合與整合測試 |
| L3 | 13 | SWE.6 軟體資格測試（需求式測試、Robustness） |
| L3 | 14 | 硬體層 Part 5（FMEDA、PMHF/SPFM/LFM、BIST） |
| L3 | 15 | 安全分析：FMEA、FTA、DFA |
| L4 | 16 | 支持流程：SUP.8/SUP.9/SUP.10 |
| L4 | 17 | 品質保證與管理：SUP.1、SUP.4、MAN.3、MAN.6 |
| L4 | 18 | 功能安全流程管理：Part 2/8（安全計畫、確認措施、安全案例） |
| L5 | 19 | ASPICE × ISO 26262 整合實務（對照矩陣、雙軌流程） |
| L5 | 20 | 完整 Worked Example：從 HARA 到 SWE.6 全流程走查 |

## 開發

本站為純靜態 HTML，內容由 `/tmp/opencode/iso_site/` 的內容模組生成，無建置步驟。

```sh
# 本機預覽（擇一）
python3 -m http.server 8000
npx serve .
```

## 授權

本站教學內容（繁體中文解說）為本站原創，採 CC-BY-4.0；術語與規範引用自 ISO 26262 與 Automotive SPICE（VDA）之公開資訊。

## 相關連結

- 學習路徑建議服務：[learning-path-advisor](https://shuming-yang.github.io/learning-path-advisor/) — 依角色推薦教學網站學習路徑
