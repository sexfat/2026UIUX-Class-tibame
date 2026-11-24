# 單元 9：元件、樣式與設計系統概念

## 單元目標

- 理解 Design Tokens 與單一真相來源的概念，能區分 Primitive（基礎層）與 Semantic（語意層）兩層命名，並說明深色模式如何透過語意層切換。
- 能分辨 Figma Styles 與 Variables 的適用情境，用 Variables 建立 Light / Dark 兩種 Mode。
- 運用原子設計（Atoms → Molecules → Organisms → Templates → Pages）拆解介面，理解母元件與實例的繼承與覆寫規則，避免隨意 Detach。
- 為可互動元件定義完整的狀態矩陣，並善用 Variant、Boolean、Text、Instance Swap 四種元件屬性，避免變體爆炸。
- 了解設計系統的三大支柱（基礎規範、元件庫、使用說明文件），以及 Auto Layout 如何對應前端 Flexbox 與 Tailwind，做出工程師能直接實作的交付。

## 課程介紹

本單元介紹設計規模化的關鍵概念——元件與設計系統。當設計稿頁面越來越多，如何讓按鈕、卡片、導覽列等重複出現的元素保持一致，並在需要修改時一次更新所有位置，是每位設計師必須面對的課題。課程貫穿兩個核心觀念：單一真相來源（Single Source of Truth）與前端元件化思維。

課程分為四個部分：第一部分以 Design Tokens 將設計決策參數化，說明 Primitive 與 Semantic 兩層命名，以及 Figma Styles 與 Variables 的分工；第二部分以原子設計拆解介面，並說明母元件與實例的繼承與覆寫規則；第三部分建立狀態矩陣，運用 Variant、Boolean、Text、Instance Swap 四種元件屬性控制元件，減少元件庫膨脹；第四部分說明設計系統的三大支柱，以及 Auto Layout 與前端 Flexbox、Tailwind 的對應關係，讓設計稿成為團隊與工程師共用的規格書。

課程結束後，學員將能使用課程提供的 Figma Design System 範本進行練習，範本包含 Light / Dark 雙模式的 Variables、文字與效果 Styles，以及 Button、Input Field、Badge 等元件，並能說明設計系統對產品一致性與團隊協作的貢獻。
