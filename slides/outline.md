# PBM 口腔傷口癒合｜HTML 教學簡報大綱

對象為牙醫學生、PGY 牙醫師與初學臨床工作者。共 14 張，採繁體中文並保留英文專有名詞。內容取自 PR #2 合併後的 [Wiki 正文](../wiki/README.md)，以 Evidence Card 的 K 節核對定位。視覺欄僅描述構想。本階段停在 Markdown 大綱與人工審核。

## 01｜PBM 的臨床研究問題

**教學目標**：能說明 photobiomodulation（PBM，光生物調節）是什麼，以及為何要先確定測量項目。

- PBM 研究以光照介入，觀察生物反應。
- 讀結果時區分細胞訊號、傷口癒合與疼痛。
- 用「研究的是誰、比較什麼、量什麼、何時量」組織問題。

**Wiki**：[第 1 章〈基礎解說〉](../wiki/01-mechanisms.md#基礎解說)、[第 6 章〈基礎解說〉](../wiki/06-evidence-and-safety.md#基礎解說)

**Evidence Card**：[01 K1、K3](../cards/01-hamblin-2018.md#k-來源定位驗證)

**視覺**：以光照、觀察項目及比較問題串成文字流程。

**證據警示**：01 是機轉敘述性綜述，未直接檢驗人體口腔傷口療效。

## 02｜粒線體與雙相劑量反應

**教學目標**：能辨識綜述討論的機轉指標，說明細胞劑量反應的外推界線。

- 粒線體膜電位（MMP）、三磷酸腺苷（ATP）、活性氧（ROS）是閱讀機轉的三個切入點。
- 正常與受壓細胞可能有不同反應。
- 綜述轉述的小鼠皮質神經元例子中，3 J/cm² 時 MMP 與鈣反應最大。
- 先說明細胞模型與所測指標，再找人體臨床終點。

**Wiki**：[第 1 章〈基礎解說〉](../wiki/01-mechanisms.md#基礎解說)、[〈如何讀一張細胞劑量圖〉](../wiki/01-mechanisms.md#研究案例如何讀一張細胞劑量圖)、[〈證據限制〉](../wiki/01-mechanisms.md#證據限制)

**Evidence Card**：[01 K1–K3](../cards/01-hamblin-2018.md#k-來源定位驗證)

**視覺**：自製概念圖與定性反應示意，避免描摹原圖或新增數據點。

**證據警示**：`PASS_WITH_LIMITS`。被引實驗未獨立核驗。統一臨床療程 `Not applicable`，完整效應量、CI、p 值及部分照射欄位 `Not reported`。3 J/cm² 只屬該細胞例。保留首刊、PMC final-form、正式期次的書目差異，原文再散布授權未確認。

## 03｜看懂照射參數與單位

**教學目標**：能從參數表分辨功率、時間、能量與能量密度，指出分母代表的面積。

- 波長用 nm，功率用 mW 或 W，irradiance 用 mW/cm² 或 W/cm²。
- 固定功率時以 W × 秒檢算能量（J）。
- 在均勻照射的示例中，J ÷ 面積得平均 fluence（J/cm²）。
- Wiki 假設例為 100 mW × 20 秒＝2 J，分布於 2 cm² 或 4 cm² 時分別為 1 或 0.5 J/cm²（先將 100 mW 換為 0.100 W）。

**Wiki**：[第 2 章〈基礎解說〉](../wiki/02-dosimetry.md#基礎解說)、[〈相同能量可以分布在不同面積〉](../wiki/02-dosimetry.md#計算示例相同能量可以分布在不同面積)

**Evidence Card**：[02 K2](../cards/02-morshedzadeh-2022.md#k-來源定位驗證)、[08 K2](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證) 用於比較研究如何定義照射面積，算例直接取自 Wiki。

**視覺**：用同樣的 2 J 並排示意兩塊不同面積。

**證據警示**：算例的均勻光束與固定功率是教學假設。光斑、傷口與掃描面積分開標示，禁止拼成臨床劑量。

## 04｜研究劑量如何檢算

**教學目標**：能並列原報告值、自行檢算及欄位缺漏。

- 02 原報 0.21 W、0.075 W/cm²、30 秒、6.3 J、5 J/cm²，光斑 2.8 cm² 與傷口 1.26 cm² 分列。Wiki 以 0.075 × 30 得 2.25 J/cm²，總劑量與累計範圍仍有歧義。
- 03 原報 50 mW 被稱為 average power density，實測 irradiance `Not reported`。Methods 記 1.23 min／點、11 J／點、66 J／牙，摘要記 11 J/cm²。Wiki 檢算得 3.69 J。
- 08 掃描面積 2.04 cm² 為幾何估計，irradiance `Not reported`、離散點數 `Not applicable`。
- 09 報告 12 J，四次累計能量及離散點數 `Not reported`。05 無可重建的逐篇劑量表，統一療程 `Not applicable`。

**Wiki**：[第 2 章〈先保留原值，再核對單位〉](../wiki/02-dosimetry.md#研究案例先保留原值再核對單位)、[〈證據限制〉](../wiki/02-dosimetry.md#證據限制)

**Evidence Card**：[02 K2](../cards/02-morshedzadeh-2022.md#k-來源定位驗證)、[03 K2](../cards/03-isolan-2021.md#k-來源定位驗證)、[05 K2](../cards/05-giansiracusa-2024.md#k-來源定位驗證)、[08 K2](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證)、[09 K2](../cards/09-yakout-2023.md#k-來源定位驗證)

**視覺**：用「原報告｜Wiki 檢算｜待核欄位」三欄。

**證據警示**：02／03 劑量 `CONFLICT`，02、03、05、08 為 `NEEDS_HUMAN_REVIEW`。保留原值與單位，檢算不回填。

## 05｜二期傷口的量測

**教學目標**：能分辨開放傷面常見的面積、上皮化與臨床評分。

- 二期傷口的 Wiki 例子包括游離牙齦移植（FGG）腭側供區和牙齦切除。
- RWA（remaining wound area）以 mm² 記錄剩餘傷口面積。
- 上皮化是另一項測量，Landry 是臨床癒合評分。
- 比較前先寫清傷口、終點、比較組與時間。

**Wiki**：[第 3 章〈基礎解說〉](../wiki/03-secondary-healing.md#基礎解說)、[〈重點整理〉](../wiki/03-secondary-healing.md#重點整理)

**Evidence Card**：[02 K1、K3](../cards/02-morshedzadeh-2022.md#k-來源定位驗證)、[09 K1、K3](../cards/09-yakout-2023.md#k-來源定位驗證)

**視覺**：用自製線條標出傷面範圍，旁列評分與上皮化的欄位。

**證據警示**：RWA 與 Landry 各自判讀。09 缺可採的連續面積療效資料，主要／次要終點預排序 `Not reported`。

## 06｜腭側供區：早期訊號與出血疑點

**教學目標**：能用時點描述 02 的結果，並判斷哪些數字可轉述。

- 配對 split-mouth 試驗比較 PBM 與 sham，16 人納入、14 人完成。
- 第 7、14 日 RWA 較小，第 21、28 日無顯著差異。
- 第 7 日未上皮化計數有差異，第 14 日無顯著差異。疼痛未見顯著組間差異。
- RWA 正文漏第 21 日且另列日 60。術日出血欄為 10、未出血 14，與 14 名完成者不符。

**Wiki**：[第 3 章〈FGG 腭側供區〉](../wiki/03-secondary-healing.md#研究案例一fgg-腭側供區)、[〈證據限制〉](../wiki/03-secondary-healing.md#證據限制)、[第 6 章〈出血訊號〉](../wiki/06-evidence-and-safety.md#研究案例出血訊號可以說到哪裡)

**Evidence Card**：[02 K1–K5](../cards/02-morshedzadeh-2022.md#k-來源定位驗證)

**視覺**：以 Table 2 時序標示各時點，旁列正文時序差異及出血註記。

**證據警示**：`NEEDS_HUMAN_REVIEW`。劑量與出血計數 `CONFLICT`，只轉述作者的出血方向與 p＝0.046，不估風險率。小樣本、失訪、NSAID 共介入限制外推。

## 07｜翻瓣傷口：一期癒合與皮瓣存活

**教學目標**：能區分一般口腔翻瓣一期癒合及缺血條件下的皮瓣存活率。

- 08 研究美觀牙冠增長術後傷口，手術包含翻瓣與骨切除。
- Modified Landry 評估局部傷口癒合。
- 缺血皮瓣存活率需要相應的存活終點，目前核准 Wiki 的證據範圍缺乏直接資料。

**Wiki**：[第 4 章〈基礎解說〉](../wiki/04-flap-healing.md#基礎解說)、[〈重點整理〉](../wiki/04-flap-healing.md#重點整理)

**Evidence Card**：[08 K1、K3](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證)

**視覺**：左右兩欄分別畫出傷緣相接示意與缺血存活終點的資料缺口。

**證據警示**：08 是 `NEEDS_HUMAN_REVIEW`。一期癒合資料不足以填補缺血皮瓣存活率的缺口。

## 08｜翻瓣試驗：同一人的兩個半弓

**教學目標**：能區分半弓配對與術前術後比較，正確描述無顯著差異。

- 27 人完成、54 半弓，同一人有 PBM 側與 sham 側。
- 所測時點癒合與疼痛無顯著組間差異，等效仍未確立。
- OHIP-14 與滿意度的 Table 3 是術前術後比較，不能將變化歸因 PBM。
- 登錄時序與 Mann–Whitney 是否處理配對仍待核。

**Wiki**：[第 4 章〈同一患者的兩個半弓〉](../wiki/04-flap-healing.md#研究案例同一患者的兩個半弓)、[〈證據限制〉](../wiki/04-flap-healing.md#證據限制)

**Evidence Card**：[08 K1、K3–K5](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證)

**視覺**：用同一人的左右半弓和另一條術前術後時間線呈現兩種比較。

**證據警示**：`NEEDS_HUMAN_REVIEW`。Results 的生活品質歸因與 Table 3／Discussion 比較方式 `CONFLICT`。收案 2022-11-25 至 2024-05-13 與聲稱前瞻登錄日 2024-07-29 的時序 `CONFLICT`，登錄網站尚未另核。小樣本、失訪、半弓間污染及配對方法限制外推。

## 09｜第三大臼齒拔除：短期 VAS

**教學目標**：能把術後疼痛的結論限定在實際比較、時間與分析單位內。

- 03 分派 44 人共 101 顆牙，PBM＋拔牙 51 顆，單做拔牙 50 顆。
- 無 sham，評估者盲化，兩組均用單次 dipyrone。
- 6、24、48 小時的疼痛視覺類比量表（VAS）平均值在 PBM 組較低。
- 研究未測傷口面積，一人可貢獻多顆牙。

**Wiki**：[第 5 章〈基礎解說〉](../wiki/05-extraction-and-adjuncts.md#基礎解說)、[〈第三大臼齒短期疼痛〉](../wiki/05-extraction-and-adjuncts.md#研究案例第三大臼齒短期疼痛)

**Evidence Card**：[03 K1–K4](../cards/03-isolan-2021.md#k-來源定位驗證)

**視覺**：以三個時間點的 VAS 對照表呈現，旁標分派單位為牙。

**證據警示**：`NEEDS_HUMAN_REVIEW`，保留劑量 `CONFLICT`（第 04 張）、群聚調整與等效界值未確認、患者未盲及自報用藥等限制。預定次要終點 `Not reported`。疼痛差異無法推為癒合改善。PMC 的 CC Attribution 版本仍未明，見 [卡片書目](../cards/03-isolan-2021.md)及 Wiki 來源追溯。

## 10｜合併治療：HA 與 guard 同時加入

**教學目標**：能描述 09 真正比較的介入及哪些效果不能分離。

- 牙齦切除試驗有 26 人，各組 13 人。
- 兩組均用 PBM，試驗組加 2% 透明質酸（HA）及 guard。
- 第 7、14、21 日 Landry 較高，第 3 日未見顯著差異。
- 疼痛未見顯著組間差異。比較限於同時加入 HA 與 guard。

**Wiki**：[第 5 章〈牙齦切除後的附加介入〉](../wiki/05-extraction-and-adjuncts.md#研究案例牙齦切除後的附加介入)、[第 6 章〈基礎解說〉的比較設計表](../wiki/06-evidence-and-safety.md#基礎解說)

**Evidence Card**：[09 K1、K3–K4](../cards/09-yakout-2023.md#k-來源定位驗證)

**視覺**：對照組與試驗組並列，共同 PBM 同色，HA／guard 同時框出。

**證據警示**：`PASS_WITH_LIMITS`。回溯登錄、小樣本、患者與操作者未盲、無組織學。無法隔離 HA、guard 或 PBM 各自效應。

## 11｜系統性回顧：VAS 效應量與 AO 分母

**教學目標**：能解釋 05 為何無法從顯示的數字得出可採用的合併療效。

- Giansiracusa 2024 回顧納入 3 研究、124 人，追蹤 7–90 日，終點資料的覆蓋不同。
- VAS 的「CI 98–99%」缺可讀群間效應量，不能讀為改善幅度。
- 齒槽骨炎（AO）原報 35／160，另列 PBM 組 0.52%，分母與對照率不清。
- 需回到可辨識的效應量、不確定性、事件數及各組分母。

**Wiki**：[第 5 章〈如何讀 05 的整合結果〉](../wiki/05-extraction-and-adjuncts.md#證據限制如何讀-05-的整合結果)、[〈為什麼不能直接採用合併療效〉](../wiki/05-extraction-and-adjuncts.md#為什麼不能直接採用合併療效)

**Evidence Card**：[05 K1–K4](../cards/05-giansiracusa-2024.md#k-來源定位驗證)

**視覺**：用「原報數字｜還缺什麼」兩欄，避免把它們放進效果圖。

**證據警示**：`CONFLICT`／`NEEDS_HUMAN_REVIEW`。保持原值與不清楚的分母，勿產生替代效應數字。

## 12｜系統性回顧：異質性與骨修復矛盾

**教學目標**：能說明異質性編碼、表文不一致與方法疑點如何限制判讀。

- Q＝0／I²＝0% 出現在 YES／NO 編碼的敘述，無法確認群間效果一致。
- 骨資料僅一項研究，Table 4 的 YES 與正文無顯著組間差異並列。
- 原文同稱無日期限制與自 2015 年起，三項原始試驗未獨立重審。
- NOS 用於 RCT 與偏差評估報告不清，逐篇劑量未列成可重建的表。

**Wiki**：[第 5 章〈如何讀 05 的整合結果〉](../wiki/05-extraction-and-adjuncts.md#證據限制如何讀-05-的整合結果)、[〈為什麼不能直接採用合併療效〉](../wiki/05-extraction-and-adjuncts.md#為什麼不能直接採用合併療效)

**Evidence Card**：[05 K1–K4](../cards/05-giansiracusa-2024.md#k-來源定位驗證)

**視覺**：以原文出處對照卡呈現 Table 4、正文及偏差評估疑點。

**證據警示**：`CONFLICT`／`NEEDS_HUMAN_REVIEW`。個別病人完整納排 `Not reported`、統一介入 `Not applicable`。不採為合併療效，不推論骨修復有效或抗生素需求降低。

## 13｜判讀練習：終點、比較與分析單位

**教學目標**：能找出容易誤讀的四種比較，回到適當的來源。

- 02 配對供區的早期 RWA，限於該傷口與時點。
- 03 多牙可能群聚，短期 VAS 只回答疼痛。
- 08 半弓有配對結構，無顯著差異不足以確立等效。
- 09 兩組共同 PBM，結果回答加入 HA 與 guard 的組合比較。

**Wiki**：[第 3 章〈重點整理〉](../wiki/03-secondary-healing.md#重點整理)、[第 5 章〈重點整理〉](../wiki/05-extraction-and-adjuncts.md#重點整理)、[第 6 章〈基礎解說〉](../wiki/06-evidence-and-safety.md#基礎解說)

**Evidence Card**：[02 K1、K3–K5](../cards/02-morshedzadeh-2022.md#k-來源定位驗證)、[03 K1、K3–K4](../cards/03-isolan-2021.md#k-來源定位驗證)、[08 K1、K3–K5](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證)、[09 K1、K3–K4](../cards/09-yakout-2023.md#k-來源定位驗證)

**視覺**：以傷口／比較／終點／分析單位四欄做讀表練習。

**證據警示**：02、03、08 保留 `NEEDS_HUMAN_REVIEW`，09 保留 `PASS_WITH_LIMITS`。不混合不同終點，不用未達顯著宣稱等效。

## 14｜臨床界線：安全訊號與查核

**教學目標**：能轉述有疑點的安全訊號、保留限制並完成來源追溯。

- 02 術日出血可轉述作者報告方向與 p 值，計數仍待核。
- 以傷口、族群、比較、分析單位、終點及時間界定每項主張。
- 查 Wiki 段落、Card K 的原文定位，以及 A 節的 DOI、版本與授權。
- 綜合本批研究無法訂出通用處方、禁忌清單或安全劑量上限。

**Wiki**：[第 6 章〈出血訊號〉](../wiki/06-evidence-and-safety.md#研究案例出血訊號可以說到哪裡)、[〈證據限制〉](../wiki/06-evidence-and-safety.md#證據限制)、[Wiki 首頁〈如何追溯主張〉](../wiki/README.md#如何追溯主張)

**Evidence Card**：[02 K1、K4–K5](../cards/02-morshedzadeh-2022.md#k-來源定位驗證)

**視覺**：用出血案例卡示範從一句主張回到 Table 5 的路徑。

**證據警示**：出血計數 `CONFLICT`／`NEEDS_HUMAN_REVIEW`，勿推算絕對或相對風險。保留 `Not reported` 與 `Not applicable`，不得拼出臨床 protocol。

## Graph 工作流程

```text
Wiki retrieval → coverage gate → slide outline → human approval [06A 停止]
  → draft → fidelity check → render check → publish approval [等待另行核准]
```

| 節點 | 通過條件 | 失敗時返回 |
| --- | --- | --- |
| Wiki retrieval | 固定已核准 main 版本，來源僅含核准 Wiki。每個主張有段落並能定位 Card K。 | 返回 Wiki retrieval，僅重取缺失的段落。找不到核准支持就標記缺口。 |
| coverage gate | 12–15 張的主題映射涵蓋指定主題、六章與六卡。缺口及警示都有指定頁。 | 缺來源返回 Wiki retrieval，來源已足但映射漏項則在 coverage gate 補映射。 |
| slide outline | 每頁有標題、目標、3–5 點、Wiki 段落、Card K、視覺構想與警示。 | 欄位或編排有誤返回 slide outline。若主題漏列，返回 coverage gate。 |
| human approval | 審核者明確核准大綱前僅交付 Markdown。進入 draft 須另有生成簡報的授權。 | 要求修訂返回 slide outline，依其變更回查 coverage gate。尚未回覆或拒絕則停在此節點。 |
| draft | 受影響頁依核准大綱製作，保留追溯與警示。 | 返回 draft 修正該頁。若需要更改已核准大綱，返回 slide outline 並重新走 human approval。 |
| fidelity check | 逐頁核對數字、單位、終點、比較、時點、限制及權利。 | 轉寫錯誤返回 draft。來源不足返回 Wiki retrieval 並重新比對覆蓋和核准大綱。 |
| render check | 投影與小畫面上的文字、表格、警示、引用均可讀且連結有效。 | 返回 draft 修正呈現，重過 fidelity check 後再檢查渲染。 |
| publish approval | 人工另外核准發布範圍、權利與版本。可用的簡報仍須等待明確發布核准。 | 版面問題返回 render check，內容／權利問題返回 fidelity check。尚未回覆或拒絕則停在此節點。 |

每個問題最多 **三次局部重試**，初次檢查不計。以頁碼及主張／欄位記錄失敗原因、返回節點、實際重試次數與結果，跨節點仍沿用同一問題計數。第三次仍未解決，停在最早未通過的檢查點並交人工。等待人工核准期間不自行重試或往下執行。06A 完成 slide outline 後停在 human approval。後續 draft、fidelity check、render check 及 publish approval 僅為規劃。
