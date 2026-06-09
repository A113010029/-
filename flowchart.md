# 新聞專題 Pipeline 流程圖
## 主題：基隆漢他病毒疫情（2026年5月）

---

## 圖零：文章內容視覺化

### 0-A　事件發展時序 × 政府回應

```mermaid
flowchart TD
    A["🐭 4月7日\n40歲男性清掃工作場所\n遭老鼠咬傷\n⚠️ 未立即就醫"]
    --> B["😷 5月2日\n出現症狀：發燒・畏寒・食慾喪失\n送醫診治，持續觀察中"]
    --> C["📢 5月19日\n基隆市政府公告通報疾管署\n衛生局長張賢政\n啟動緊急消毒＋病原追蹤"]
    --> D["🏛️ 5月19日 — 謝國樑\n主持緊急防疫會議\n宣示：從根本解決鼠患問題"]
    --> E["⚔️ 5月20日 — 三箭行動"]

    E --> E1["① 免費發放滅鼠藥給市民"]
    E --> E2["② 提供專家到府指導"]
    E --> E3["③ 同步展開環境清消作業"]

    E1 & E2 & E3 --> F["📋 5月22日\n謝國樑主持防疫進度說明會\n公布市場十大稽查重點"]

    F --> G1["🚢 基隆港周邊"]
    F --> G2["🏪 傳統市場"]
    F --> G3["🏘️ 社區巷道"]

    G1 & G2 & G3 --> H["🧹 衛生局＋環保局＋港務單位\n地毯式整治計畫\n預計三週內完成第一波全市消毒覆蓋"]

    style A fill:#e63946,color:#fff
    style B fill:#f4a261,color:#000
    style C fill:#e9c46a,color:#000
    style D fill:#457b9d,color:#fff
    style E fill:#1d3557,color:#fff
    style H fill:#2a9d8f,color:#fff
```

### 0-B　漢他病毒傳播路徑與民眾防護決策樹

```mermaid
flowchart TD
    START(["🐀 環境中有鼠患"])

    START --> T1["接觸途徑"]
    T1 --> T2["鼠類排泄物／鼠屍接觸"]
    T1 --> T3["遭老鼠咬傷或抓傷"]

    T2 & T3 --> Q1{"是否出現症狀？\n發燒・畏寒・肌肉疼痛"}

    Q1 -- 有症狀 --> A1["立即就醫\n主動告知醫師曾有鼠類接觸史"]
    Q1 -- 無症狀（咬傷當下） --> A2["立即清洗傷口\n盡快就醫，不要等症狀出現"]

    START --> P1{"人傳人？"}
    P1 -- 一般情況下不會 --> P2["普通民眾風險相對較低"]
    P1 -- 鼠患嚴重的居住或工作環境 --> P3["⚠️ 提高警覺"]

    P3 --> D1["避免徒手接觸可疑排泄物或鼠屍"]
    P3 --> D2["及早清除垃圾堆積場所"]
    P3 --> D3["配合市府滅鼠行動"]

    style START fill:#e63946,color:#fff
    style A1 fill:#e9c46a,color:#000
    style A2 fill:#f4a261,color:#000
    style P2 fill:#90be6d,color:#000
    style P3 fill:#e63946,color:#fff
```

---

```mermaid
flowchart TD
    A([🦠 主題確立\n基隆漢他病毒疫情]) --> B

    B[步驟 1：選題與素材蒐集\n搜尋基隆漢他病毒相關新聞]
    B --> B1[📰 Taipei Times 2026/05/19\nKeelung reports suspected hantavirus case]
    B --> B2[📰 more-news.tw 2026/05/19\n基隆傳疑似漢他病毒病例]
    B --> B3[📰 more-news.tw 2026/05/20\n謝國樑祭三箭滅鼠]
    B --> B4[📰 more-news.tw 2026/05/22\n基隆全面防鼠防疫]
    B1 & B2 & B3 & B4 --> C

    C[步驟 2：寫新聞草稿\n產出 300–500 字新聞稿]
    C --> C1{AI 起草完成？}
    C1 -- 是 --> C2[✏️ 自己修改潤稿]
    C1 -- 否 --> C

    C2 --> D[步驟 3：事實查核\n驗證至少 1 個 claim]
    D --> D1{查核通過？}
    D1 -- 通過 --> E
    D1 -- 未通過 --> D2[修正內容] --> D

    E[步驟 4：上稿 WordPress\n發布至 cocorico.info]
    E --> E1{發布成功？}
    E1 -- 是 --> F
    E1 -- 否 --> E1b[檢查後台設定] --> E

    F[步驟 5：第二平台發布]
    F --> F1[📘 Facebook 版\n200–300字 口語化 + 連結]
    F --> F2[📸 Instagram 版\n條列式重點 + hashtag x10]
    F1 & F2 --> G([✅ 完成發布])

    style A fill:#f9c74f,stroke:#f3722c,color:#000
    style G fill:#90be6d,stroke:#43aa8b,color:#000
    style B fill:#4d908e,color:#fff
    style C fill:#4d908e,color:#fff
    style D fill:#4d908e,color:#fff
    style E fill:#4d908e,color:#fff
    style F fill:#4d908e,color:#fff
    style F1 fill:#3b5998,color:#fff
    style F2 fill:#c13584,color:#fff
```

## 工具與負責人對照

| 步驟 | 工具 | 負責人 |
|------|------|--------|
| 1. 選題與素材蒐集 | Kiro | AI + 自己確認 |
| 2. 寫新聞草稿 | Kiro | AI 起草，自己修改 |
| 3. 事實查核 | Google + Kiro | 自己做 |
| 4. 上稿 WordPress | WordPress 後台 | 自己操作 |
| 5a. FB 發布 | Facebook | 自己操作 |
| 5b. IG 發布 | Instagram | 自己操作 |

---

## Instagram 發布內容（實際產出）

> 對應步驟 5b，以下為實際發布的 IG caption：

```
⚠️ 基隆出現疑似漢他病毒病例

一名40歲男性4月遭老鼠咬傷
25天後出現發燒、畏寒、食慾不振
確認通報疾管署 🏥

市長謝國樑緊急宣布三大措施 👇
✅ 免費發放滅鼠藥
✅ 專家到府指導
✅ 全市環境清消啟動

基隆港、傳統市場、社區
衛生局 × 環保局 × 港務單位
全面展開地毯式整治 🐀❌

─────────────────
🔬 漢他病毒小知識
主要透過接觸鼠類排泄物或被咬傷傳播
✋ 不會人傳人
被老鼠咬到請立即清洗傷口並就醫！
─────────────────

#基隆 #漢他病毒 #公共衛生 #滅鼠
#Hantavirus #基隆港 #謝國樑
#防疫 #台灣新聞 #健康資訊
```
