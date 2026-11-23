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
