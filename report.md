# 任務 06B：HTML 教學簡報

**狀態**：14 張 HTML 簡報已製作，等待人工核准。以 PR #3 合併的核准大綱（main 5b2f61e）為基準。

- [HTML 簡報](slides/deck.html)採單檔 HTML、CSS、JavaScript，含左右鍵、上一張／下一張、頁碼與逐頁來源。第 4、11、12 張使用對照表，第 14 張有學習總結。
- 逐頁核對核准大綱、數字、警示與 56 個來源連結及錨點。文獻原有 `CONFLICT`、`NEEDS_HUMAN_REVIEW` 與 `PASS_WITH_LIMITS` 保留。
- 使用本機 HTTP 在 Chromium 測試四種尺寸、逐頁導覽與截圖。雲端瀏覽器的 `file://` 政策限制及實際修訂見 [執行紀錄](wiki/log.md)。待人工核對項目見 [HTML 審核清單](reviews/task06b-html-review.md)。

---

# 任務 06A：HTML 教學簡報大綱規劃

**狀態**：Markdown 大綱已完成，等待人工核准。以合併任務 05 PR #2 的 main（dd3f395）為基準，既有文獻疑點及 QA 標記照錄。以下保留各階段當時的狀態紀錄。

- [14 張簡報大綱](slides/outline.md)涵蓋六章 Wiki 與六張 Evidence Cards。每張列教學目標、重點、Wiki 段落、Card K、視覺構想及警示。
- Graph 定義八個節點、失敗回返、每項問題最多三次局部重試，以及兩個人工核准節點。本階段停在大綱核准，後續草稿、呈現檢查與發布均為規劃。
- [人工審核清單](reviews/task06a-outline-review.md)列出待核項目，包括劑量原值與檢算、合併統計疑點、出血計數、配對與登錄時序、疼痛與癒合的區隔，以及缺血皮瓣存活的證據缺口。
- [執行紀錄](wiki/log.md)保存核對範圍及結果。正文來源限於核准 Wiki，沿用其卡片與原文定位，未新增研究或數據。

---

# 任務 05：六章 Wiki 正文初稿

**狀態**：初稿待人工審核。以確認含 PR #1 合併提交的 main 為起點，依核准大綱撰寫繁體中文六章正文。任務 04 當時的審核等待記錄保留於下方歷史。

- [Wiki 首頁與六章導覽](wiki/README.md) 包含逐章學習目標、基礎解說、研究案例、證據限制、重點整理與來源追溯。
- [人工審核清單](reviews/task05-wiki-review.md) 涵蓋逐章設計、樣本、比較組、時間、統計、劑量與待決問題。
- 只用 01、02、03、05、08、09。核對依據是現有 Evidence Cards、卡片 K 原文定位及任務 03 查核紀錄。本輪未重新解析原始文獻或重算統計。
- 保留已知劑量、計數、群聚、合併統計、登錄與歸因疑點。缺血皮瓣存活率維持證據缺口。初稿完成後停止，等待人工審核。

[實際執行與品質核對](wiki/log.md#任務-05-實際執行紀錄)

---

# 任務 04：PBM LLM Wiki 六章大綱

**結果**：大綱與人工審核清單完成，待人工核准。任務 03 的有條件核准僅延伸至大綱規劃，既有四張 `NEEDS_HUMAN_REVIEW` 與兩張 `PASS_WITH_LIMITS` 維持。

- [六章大綱](wiki/outline.md) 涵蓋 6／6 張卡。將一期癒合章縮至口腔牙冠增長術後翻瓣，缺血皮瓣存活率列為待補證的獨立終點。合併治療案例標示為牙齦切除。
- [人工審核清單](reviews/task04-outline-review.md) 涵蓋章序、來源、數據、證據層級、疑點及初學者可讀性。
- 流程與核對結果見 [執行紀錄](wiki/log.md)。本輪依遠端 main 的 Evidence Cards 與任務 03 查核紀錄做文件忠實度檢查，未重新審查原始研究。
- 待人工決定：02／03 劑量與計數／群聚問題、05 的教學用途、08 的登錄／配對／歸因、09 共介入案例的取捨、皮瓣存活率補證及 01／03 再利用授權。

以下保留任務 01–03 的歷史紀錄。正式 Wiki 正文、HTML 簡報及發布均在本次授權範圍外。

---

# 任務 03：全文匯入、Evidence Cards與嚴格證據查核

日期：2026-11-23（Asia/Taipei）。狀態：AWAITING_HUMAN_REVIEW。
起始實際記錄：23:45:09.252915；全文／表格解析完成節點：23:48:53.848；卡片初稿節點：23:51:34.651–652；獨立查核步驟：23:52:05.710–23:53:27.405。這是節點記錄時間，非逐篇耗時估計。後續提交／回讀紀錄以實際GitHub回傳為準。

## 授權與完成範圍

已先讀取遠端AGENTS.md、sources.md、report.md。使用者明確核准01、02、03、05、08、09，覆蓋任務01／02「尚未核准ingest」的舊階段限制；未擴張至04、06、07或正式Wiki生成。

08／09 DOI實際從sources.md取得，分別為10.1007/s10103-026-04950-0與10.1186/s12903-023-03519-5，再與出版社全文核對。所有六篇作者、年份、研究類型、版本與來源均列於卡片A；本文不把回顧當成新RCT。

## 結果與成功數量

| ID | 全文匯入 | 卡片查核 | 定位完整性／主要待決問題 |
| --- | --- | --- | --- |
| 01 | INGESTED | PASS_WITH_LIMITS | 本卡主張均有section／figure；屬機轉綜述，原始實驗未重審；全文再散布授權未確認 |
| 02 | INGESTED | NEEDS_HUMAN_REVIEW | 主要結果有Table 2–6；劑量、時程及Table 5計數矛盾已定位，不能解除 |
| 03 | INGESTED | NEEDS_HUMAN_REVIEW | Methods與PDF p.5 Table 2；功率／時間／能量矛盾、病人內多牙群聚待核 |
| 05 | INGESTED | NEEDS_HUMAN_REVIEW | §2–5／Table 4；VAS CI、AO數字、Q／I²與骨結果矛盾已定位，不能解讀成可靠合併療效 |
| 08 | INGESTED | NEEDS_HUMAN_REVIEW | Methods／PDF p.4、7 Table 1、3–5；登錄時序、配對分析與生活品質歸因待核 |
| 09 | INGESTED | PASS_WITH_LIMITS | Methods／PMC Table 1、4／Fig.5及結果文字；HA＋guard共介入，非獨立PBM療效 |

- 全文取得並解析：6／6；六張A–K Evidence Cards已建立。
- 來源取得失敗：0／6。03、08、09的部分表格入口失敗經局部fallback解決，不把失敗入口算成功，也不把整篇重做。
- 卡片表述通過有限度查核：2／6（01、09）；醫學QA需人工：4／6（02、03、05、08）。
- 每張卡片擷取的重要主張均具section／table／figure或PDF頁定位；來源本身衝突的數值標CONFLICT，不因「找到位置」而稱正確。
- 未報告欄位使用Not reported；綜述統一protocol等不適用者使用Not applicable。08的irradiance沒有由tip面積推成作者實測值。
- 01全文CC再散布未確認；03 CC版本未明。本次只提交自撰文字／連結，不將原始HTML、圖或PDF提交。
- INGESTED僅指取得完整研究正文並解析到卡片；未建立向量資料庫或保存原文檔案，不等於醫學QA或後續發布已核准。

## 實際Loop與局部退回

1. FETCH六篇官方HTML。
2. PARSE分頁閱讀完整研究正文；不足的表格只回到該篇PARSE_TABLE。
3. CARD_DRAFT生成六張卡，初稿已保留原文數字衝突。
4. VERIFY_INDEPENDENT_STEP另做原文優先複核，逐項核DOI／設計、族群、參數單位、結果方向、證據分層、位置與矛盾。
5. 保留來源疑點／修訂卡片QA註記，交人工決策。
6. 保存文字、提交、回讀後停止。詳細時間、來源與動作見 [wiki/log.md](wiki/log.md)。

| 問題 | 初次 | 真實重試 | 最終處理 |
| --- | --- | --- | --- |
| 03 Table 2 | PMC驗證頁 | 1次：官方PDF | p.5 Table 2可解析 |
| 08 Table 1／4／5 | HTML anchor無cells | 1次standalone table URL失敗；2次官方PDF成功 | PDF p.4／7定位；PMC仍受阻但不繞過 |
| 09 Table 1／4 | HTML anchor無cells | 1次standalone URL失敗；2次PDF／PMC成功 | Table 1／4可核對 |
| 02／03劑量、05統計、08時序 | 解析時辨識來源疑點 | 查核步驟重新讀原文確認；沒有做假修正／反覆重試 | NEEDS_HUMAN_REVIEW，非替作者補造資料 |

重試最高2，未超過3。來源內部衝突即使重開同一頁也無法自動修正，確認後直接標人工審核，沒有為湊3次虛構錯誤。正常分頁及第二查核步驟不計為重試。其他已完成卡片未因局部表格問題重做。

## 嚴格查核的實際發現

- **02**：摘要16人，完成14人；已分開。Table 1劑量／面積不一致，Table 5日0 laser計數10+14不等於14完成者；保留原記載，不算出血風險率。早期RWA改善不等於疼痛改善。
- **03**：50 mW、1.23分鐘與11 J／點不一致；摘要11 J/cm²亦與Methods的11 J不同。未將算術稽核值補作作者量測。101顆牙不是101位獨立患者；群聚與等效分析需核。
- **05**：VAS的CI98–99%、AO0.52%、YES／NO編碼下的Q=0，以及Table 4骨修復YES對正文無組間差異，均不可直接用為臨床療效結論。
- **08**：登錄日期晚於文中收案期間，但未另查登錄網站，僅標原文時序衝突；split-mouth配對分析需核。Table 3的滿意度／OHIP前後改善不能歸因PBM。傷口與疼痛組間不顯著不代表已證明等效。
- **09**：HA與guard共介入，兩組均PBM；只能解讀為組合差異。原來源摘要說26位點，Methods確認26患者，卡片按具體Methods列26人並避免加總為額外樣本。
- **01**：機轉綜述含前臨床例子；圖中的劑量不能當口腔臨床處方。

獨立查核「步驟」由同一助理在初稿之後執行，限原始來源與卡片作判斷；不是獨立人類／另一個模型，也未宣稱完成專家審稿或正式RoB 2／AMSTAR 2評分。具體矩陣見 [reviews/task03-audit.md](reviews/task03-audit.md)。

## 跨文獻差異

02為腭供區二期癒合且早期RWA較小；08為翻瓣骨切除後一期癒合且未見組間優勢；03測疼痛；09比較HA＋guard附加效果。不同組織、癒合方式、共介入與參數不強行統一。05的回顧標籤不凌駕其統計疑點；01只作機轉背景。

## 文件與GitHub提交

Repository：nycuhhtc-debug/pbm-oral-wound-wiki，重新查詢仍為private、main、push可用。
新增六張指定cards、wiki/log.md、reviews/task03-audit.md；更新sources.md、report.md、README.md、AGENTS.md。現行狀態位於各檔頂部，任務01／02歷史保留。wiki/只建立log，未建立正式六章正文。

已依main原base tree建立文字變更並提交；未覆寫其他檔案、未force push。工作提交與12檔遠端回讀皆已成功，真實SHA與時間見下列回執。

## 任務 03 提交成功回執

- 2026-11-23T23:58:46.977+08:00：GitHub建立工作提交 [b7a86c98ed55fe95f4d3eb9c1e4eeec41e387a6c](https://github.com/nycuhhtc-debug/pbm-oral-wound-wiki/commit/b7a86c98ed55fe95f4d3eb9c1e4eeec41e387a6c)，main以expected-head檢查、force=false更新成功。
- 2026-11-23T23:58:59.285+08:00：以該commit為ref逐一回讀12個文字檔，內容全部一致；遞迴tree未截斷、恰有6張cards，wiki只有log.md；沒有PDF／原始HTML／圖像或literature全文。
- 此回執是工作提交後的真實驗證，另以紀錄提交保存；紀錄提交自己的最終SHA由交付回覆提供，不預填自我指涉值。現在停止等待人工審核。

## 人工審核清單

- [ ] 審閱六張卡及K定位，接受INGESTED與QA結果是分開欄位。
- [ ] 02／03參數疑點是否查勘誤／作者；在釐清前是否禁止列為臨床protocol。
- [ ] 05是否只作批判案例，不採其合併療效／AO數字。
- [ ] 08登錄／配對分析與生活品質歸因如何處理；是否只保留陰性結果。
- [ ] 01／03後續原文再利用權限與版本限制。
- [ ] 09是否以合併治療分類保留，避免推論獨立PBM效果。
- [ ] 另行授權下一階段；本次不生成正式Wiki正文、HTML簡報或部署。

任務03完成後停止等待人工審核。未公開PDF、未啟用GitHub Pages、未將Repository改為Public。

## 檔案驗證補記

六篇研究正文的分頁覆蓋無缺行，六卡均具A–K。一次本機內容驗證因大量輸出開頭出現Warning而無法解析JSON；重試1改用小量路徑／字元數成功，12檔皆相符。此為技術驗證問題，不是捏造的醫學錯誤，亦未重做其他卡。最終仍需GitHub全文回讀一致才宣稱提交成功。真實時間見wiki/log.md。

---

# 任務 01／02 歷史報告

下方為舊任務原文，當時的未核准ingest／0篇與目前授權狀態不同；目前以本頁任務03為準。

# 任務 02：補充 Open Access 文獻與重新檢查來源

查核日期：2026-11-23（Asia/Taipei）。狀態：AWAITING_HUMAN_REVIEW。
任務 01 的 sources.md 已由使用者人工審核；任務 02 新增文獻與本輪報告尚待人工審核。本輪未執行正式 ingest。

## 退回來源取得節點的實際流程

本次不是將上一輪視為全文已齊備後繼續生成。實際流程如下，沒有捏造已進行的文獻匯入或審核：

| 順序 | 實際節點／動作 | 觀察與決定 |
| --- | --- | --- |
| 1 | 使用者人工審核任務 01 sources.md | 確認 7 篇中僅 4 篇有可讀 HTML，04／06／07 為訂閱預覽；少於至少 5 篇目標 |
| 2 | 退回來源取得節點 | 使用者明確下達任務 02：保留 7 篇並補找 2 篇 OA，不開始 ingest |
| 3 | 讀取 Repository 的 AGENTS、sources、report | 以遠端現況為準，保留原 ID 與查核記錄；另確認 Repository 仍為 private、main 分支可讀寫 |
| 4 | 重新開啟原始 7 篇官方來源 | 01／02／03／05 仍可讀正文；04／06／07 仍為 subscription preview；不將摘要／部分圖表當成全文 |
| 5 | 搜尋與候選篩選 | 搜尋 oral／palatal wound healing、gingivectomy、flap viability、PBM parameters 相關研究；依實際全文與文章級授權篩選 |
| 6 | 核對新增 08、09 | 兩篇均在出版社與 PMC 核對書目、Methods 正文及 CC BY 4.0；各自的研究設計限制寫入 sources.md |
| 7 | 重新盤點來源數量 | 9 篇候選中 6 篇合法 HTML 可讀；5 篇具文章級再利用聲明（03 的 CC 版本仍待核） |
| 8 | 更新文件並停止 | 提交 sources.md、report.md，並同步 README／AGENTS 的當前範圍；等待本輪人工審核 |

「3 篇無法取得全文」指本次可用的未登入官方入口無法取得全文，不代表所有合法機構、購買或作者授權途徑都不存在。本輪未購買、未聯絡作者、未使用機構登入，也未繞過限制。

## 新增兩篇與選擇理由

| ID | 書目定位／DOI | 研究類型與主題 | 全文及授權 | 保留限制 |
| --- | --- | --- | --- | --- |
| 08 | da Silva Azevedo et al. 2026；10.1007/s10103-026-04950-0 | 人體 pilot split-mouth RCT；口腔全厚瓣＋骨切除後一期癒合／PBM 參數 | 出版社與 PMC HTML 正文可讀；CC BY 4.0 | 不是缺血皮瓣存活率模型；傷口癒合結果非顯著正向，不因結果而排除 |
| 09 | Yakout et al. 2023；10.1186/s12903-023-03519-5 | 人體 RCT；牙齦切除後二期癒合／PBM 參數 | 出版社與 PMC HTML 正文可讀；CC BY 4.0 | PBM＋HA 對 PBM，無無照光對照；不能隔離 PBM 效果；回溯性登錄 |

完整作者、題名、日期、PMID／PMCID、官方 URL 及簡要參數見 [sources.md](sources.md)。本輪僅查核來源與主題適配，未建立全文資料庫或進行完整療效整合。

本次也查看到其他搜尋候選：大鼠皮瓣研究 Inhibitory effects of low-level laser therapy on skin-flap survival in a rat model 的搜尋結果顯示 all rights reserved，未將可讀等同開放再利用；另一篇 dual-wavelength palatal donor-site RCT（10.1007/s10103-025-04665-8）讀到 PubMed 書目，但本輪沒有完成出版社全文／授權確認，因此未新增為已核驗 OA 來源。以上不是全面系統性檢索；未宣稱排除所有其他文獻。

實際搜尋包含：
- photobiomodulation oral palatal wound healing randomized trial open access parameters gingivectomy 2023
- photobiomodulation skin flap viability randomized experimental study open access Creative Commons parameters
- photobiomodulation palatal donor wound healing randomized clinical trial 2024 2025 open access BMC
- 新候選完整題名搜尋，並直接開啟出版社與 PMC。

## 數量目標與授權分開計算

| 口徑 | 任務 01 | 任務 02 後 |
| --- | --- | --- |
| 候選文獻總數 | 7 | 9，原 7 篇未刪除或取代 |
| 合法可讀 HTML | 4 | 6：01、02、03、05、08、09 |
| 可讀且有文章級再利用聲明 | 3 | 5：02、03、05、08、09；03 版本未明 |
| 明確 CC BY 4.0 且 HTML 可讀 | 2 | 4：02、05、08、09 |
| 只有訂閱預覽／全文未取得 | 3 | 3：04、06、07 |
| 正式 ingest 已完成 | 0 | 0 |

按使用者指出的「合法可讀 HTML 全文」門檻，來源取得數量由 4 增至 6，超過至少 5 篇。若下一階段採「全文可讀且有再利用聲明」為來源池，則有 5 篇，但必須揭露 03 的 CC 版本尚未確認；如要求全部明確 CC BY 4.0，則僅 4 篇，不能宣稱達標。這些數量都不代表新增候選已審核通過或已獲 ingest 許可。

保留兩個尚未解除的範圍限制：原始皮瓣文獻 06、07 的全文缺口仍存在；新增 08 補的是口腔翻瓣一期癒合而非缺血存活率，09 補的是二期癒合與參數，未宣稱補齊所有 flap viability 證據。

## 本輪存取與驗證限制

- 新增 08 的 PMC 文章最初可讀到書目、授權及正文；後續 Table 1 定位請求遇驗證頁。改以已可讀的出版社 Methods 與授權核對，未繞過驗證。
- 新增 09 的出版社與 PMC 均可讀正文及 CC BY 4.0 聲明。
- 本輪未測試新增文獻 PDF 二進位檔案；只記官方 PDF 入口。未保存或提交 PDF／HTML 全文。
- 原有 PDF 成功／受阻狀態屬任務 01 記錄，本輪沒有重測，不冒充重新驗證。
- 原有 04、06 的 PMID 完整頁面覆核、03 的 CC 確切版本、01 的開放再利用授權仍未解決。
- 本輪再次讀取 06 的權利聲明；07 的權利判定沿用任務 01，未宣稱本輪重查。

## Repository 變更與核驗

指定 Repository：[nycuhhtc-debug/pbm-oral-wound-wiki](https://github.com/nycuhhtc-debug/pbm-oral-wound-wiki)；ID 1468942621。本輪 GitHub 查詢再次回傳 visibility: private、default_branch: main、push: true。讀取遠端 sources.md 與 report.md 成功。

更新檔案：
- sources.md：保留 01–07，新增 08–09、7 篇重新檢查與不同口徑的來源數量。
- report.md：本節記錄實際退回來源取得的流程；任務 01 舊報告保留於下方，明確標示為歷史。
- README.md：同步任務 02 狀態及 9 篇／6 篇可讀／5 篇具再利用聲明。
- AGENTS.md：依使用者此次明確授權，新增任務 02 可補 2 篇的範圍，保留所有禁止事項。

是否上傳成功，以工具回傳的 commit SHA 與提交後遠端回讀一致為準；不預造本報告自身提交 SHA。交付回覆提供實際最後提交。

## 本輪人工審核清單

- [ ] 接受新增 08、09 的書目、全文入口與 CC BY 4.0 查核。
- [ ] 接受 08 的口腔翻瓣／09 的 HA 共介入適用範圍，不將它們等同缺血 flap viability 的完整替代。
- [ ] 決定「至少 5 篇」採全文可讀、有再利用聲明，或全部明確 CC BY 4.0 的口徑。
- [ ] 決定是否補查 03 的授權版本，以及原有其他未解決欄位。
- [ ] 另行明確下達下一階段授權；本輪審核與來源數量達標均不自動啟動 ingest。

## 停止點

任務 02 結束，等待人工審核。正式 ingest、Wiki、HTML 簡報、公開發布及公開 PDF 均未執行；文獻全文沒有保存到本機或 Repository。

---

# 任務 01 歷史報告（原文保留）

下方狀態、數量與未勾選審核項目代表任務 01 當時記錄。使用者已在任務 02 指令中明確確認 sources.md 經人工審核；當前狀態以上方任務 02 為準，不把來源審核延伸成 ingest 授權。

# 任務 01：執行與人工審核報告

查核日期：2026-11-23（Asia/Taipei）。
狀態：AWAITING_HUMAN_REVIEW — 任務 01 查核已結束；以下未解決事項保留，不宣稱全部取得全文或完整授權。

## GitHub 連線與指定儲存庫

- 已重新呼叫 GitHub 帳號與儲存庫查詢，成功回傳，非僅依瀏覽器畫面推定。
- 帳號：nycuhhtc-debug；GitHub 使用者 ID：344819036。
- 儲存庫：[nycuhhtc-debug/pbm-oral-wound-wiki](https://github.com/nycuhhtc-debug/pbm-oral-wound-wiki)。
- Repository ID：1468942621；visibility：private；default_branch：main；archived：false；回傳 push、pull、admin 權限皆為 true。
- 骨架檔案逐一建立時，GitHub 皆回傳成功及 commit SHA。初始骨架最後一筆提交：0e1be779b7be31fa248141bbff4dc062857d3a56。
- 其後讀取遠端 AGENTS.md 成功，並讀取 main 的遞迴 tree；truncated 為 false，含全部 9 個初始檔案，確認不是只存於本機。
- 本報告、sources.md 與 README 的本輪更新，以 GitHub main 上實際提交紀錄為準；提交 SHA 應由交付回覆列出，不在檔案中預先編造自身 commit SHA。

## 交付內容

| 檔案／目錄 | 用途與狀態 |
| --- | --- |
| README.md | 專案範圍、結構、審核停止點 |
| AGENTS.md | 禁止未核准 ingest、正式 Wiki／HTML、公開 PDF 與變更 Public 的規則 |
| sources.md | 指定 7 篇書目、合法全文入口、授權與未解決事項 |
| report.md | 本報告；完成範圍、限制及人工審核清單 |
| evidence/ | 僅保留空目錄；可追溯證據 URL 與觀察寫在 sources.md，未保存全文或網站快照 |
| metadata/ | 空目錄；未建立可匯入文獻庫 |
| reviews/ | 空目錄；本輪人工審核決定尚未收到 |
| literature/ | 僅 .gitkeep；沒有 PDF、HTML 全文或其他文獻內容 |
| .gitignore | 忽略 literature 下全文、PDF、EPUB 與常見憑證檔 |

Repository 只保存本次撰寫的書目與查核紀錄。沒有建立網站、GitHub Pages、HTML 簡報、向量索引或正式 Wiki。

## 查核結果

七個 DOI 均在出版社或 PMC 找到題名、作者與出版定位，與使用者候選作者相符；未替換任何候選文獻。逐篇結果與來源見 [sources.md](sources.md)。

| 項目 | 結果 |
| --- | --- |
| 核心書目 | 7／7 已以出版社或 PMC 核對 |
| 合法免登入 HTML 全文 | 4／7 已確認：01、02、03、05 |
| PDF 遠端檔案成功驗證 | 2／7：02（13 頁）、03（8 頁）；沒有下載保存 |
| 官方 PDF 入口但檔案未驗證 | 01、05；不能計入 PDF 成功驗證 |
| 出版社訂閱預覽／全文未取得 | 04、06、07；存在合法機構／購買途徑，本次未使用 |
| 明確文章級開放授權 | 02、05：CC BY 4.0；03：CC Attribution，版本未確認 |
| 未確認開放再利用／散布授權 | 01、04、06、07；06、07 另有 exclusive-rights 聲明 |
| PMID 待完整頁面覆核 | 04、06；目前僅讀到 PubMed 搜尋索引，沒有將索引當作完整頁面核驗 |

「未取得」不等於「不存在」；機構訂閱、作者授權稿等途徑可能存在，但本次沒有測試或取得授權。免費閱讀與取得 CC 授權是分開判定；Private Repository 也不能取代全文保存或再散布授權。

## 書目差異與範圍提醒

1. Batista：使用者標籤為 2025；線上發表日為 2025-12-29，出版社正式卷年為 2026、41 卷、文章號 5。sources.md 同時保存兩者，不擅自改變候選身分。
2. Hamblin：Wiley First published 2017-11-22、PubMed Epub 2018-01-19、期次 2018-03；正式引用保留 2018。PMC 提供作者接受稿，須與出版社版本區分。
3. Isolan：線上日期 2020-12-19、期次 2021-05；正式引用採 2021。CC Attribution 版本未在所讀文章聲明中明示。
4. 候選包含機轉回顧（01）、系統性回顧（05、06）、大鼠實驗（07）與臨床試驗（02、03、04）。06、07 為皮瓣研究，不能視為直接口腔臨床證據；03 主要為疼痛評估。此處僅做範圍標記，沒有完成療效證據整合或臨床建議。

## 實際遇到的存取限制

- PMC Hamblin HTML 最初遇瀏覽器驗證頁；後續再次讀取成功，未繞過驗證。
- PMC Isolan PDF 回傳 Preparing to download 中介頁，未視為 PDF 成功；改由出版社官方 PDF 成功遠端檢視。
- PMC Giansiracusa PDF 遇瀏覽器驗證頁，MDPI /pdf 入口工具回傳無法存取；HTML 和文章授權可直接讀取，PDF 仍標未驗證。
- 04、06 的 PubMed 直接頁面只回傳頁尾，另試 PubMed 格式入口仍不可存取。其核心書目由出版社確認，PMID 僅保留為搜尋索引資料。
- 02、03、05 的 PubMed 頁面亦有相同回傳問題，但其 PMID／PMCID 已從成功讀取的 PMC 文章頁核對。
- 曾嘗試 Crossref API 作額外交叉核對，執行環境 DNS 無法解析 api.crossref.org。未取得 Crossref 資料，未將其列為成功查核來源。
- 對 04、06、07 進行 DOI 定向全文／repository 搜尋；未確認可合法公開閱讀的替代版本。沒有使用未明授權的第三方 PDF，沒有聯絡作者、購買或登入機構帳號。

## 人工審核事項

- [ ] 接受七篇書目與上述日期／版本差異記錄，尤其 Batista 正式卷年 2026。
- [ ] 接受 01、05 的 PDF 狀態暫為「官方入口已確認，檔案未驗證」。
- [ ] 決定是否補核 03 的 CC 版本，以及 04、06 的完整 PubMed PMID 記錄。
- [ ] 決定如何合法取得 04、06、07 全文，及 01 的後續再利用範圍。
- [ ] 確認是否保留回顧、動物皮瓣與疼痛文章作為後續專案的不同證據層次。
- [ ] 明確核准下一階段工作範圍後，才可開始任何正式 ingest。候選清單先前已人工審核，不視為此項核准。

## 停止點

本輪只完成任務 01 的書目、可取得性、授權查核及骨架交付。所有未能核實的欄位均保留未確認狀態。現在停止，等待使用者人工審核；不自動執行 ingest、生成 Wiki／HTML 簡報或公開發布。
