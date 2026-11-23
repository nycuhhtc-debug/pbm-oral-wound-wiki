# 任務 03：來源優先的獨立查核步驟

查核起始：2026-11-23T23:52:05.710+08:00；結束記錄：2026-11-23T23:53:27.405+08:00。
範圍：卡片初稿建立後，重新定位原始來源並與卡片比較。由同一助理另做此步驟，沒有第二位人類／獨立模型，也不是正式專家審稿。先前生成的 sources／推論未作為醫學主張的證據。

## 狀態定義

- INGESTED：本輪已取得合法可讀的完整研究正文（方法、結果、討論／結論，或綜述相應全文）並解析為卡片；不等於下載保存原始全文、不等於完成向量庫，也不等於查核通過。
- VERIFIED_TO_SOURCE：原文存在該記載，並非證明記載正確。
- PASS_WITH_LIMITS：本卡目前忠實呈現可定位的來源內容與限制，不代表研究低偏差／建議可臨床採用。
- NEEDS_HUMAN_REVIEW：來源層級衝突／重要方法疑問尚不能解除；保持原值及保守解讀。
- Not reported：查閱的原文未報告該欄位；與「表格因工具未解析」不同。Not applicable用於非單一試驗／非離散點等不適用情況。

## 八項核對

| ID | DOI／作者／類型 | 族群／樣本／比較 | 單位／劑量 | 統計與結論 | 證據分層 | 定位 | 矛盾保留 | 來源優先複核結果 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 01 | 一致 | 單一試驗N/A | 統一protocol N/A；例子標被引細胞研究 | 無自造臨床效果 | 綜述／前臨床間接 | Introduction、Redox effects、Fig.4–5 | 不將3 J/cm²當臨床處方 | PASS_WITH_LIMITS |
| 02 | 一致 | 16納入／14完成，配對 | 原值忠實；作者dosimetry未能一致 | 早期RWA較小；疼痛不顯著 | 人體供區RCT | Table 1–6、Limitations、Conclusion | 出血計數／時程／劑量保留 | NEEDS_HUMAN_REVIEW |
| 03 | 一致 | 44人101牙、51／50牙，無sham | 原文單位與能量不一致 | VAS差異≠癒合；群聚未確認 | 人體疼痛RCT | Methods、PDF p.3、p.5 Table 2 | 摘要fluence與Methods energy保留 | NEEDS_HUMAN_REVIEW |
| 05 | 一致 | 3研究124人，非本篇新試驗 | 無可重建逐研究protocol表 | CI／AO／異質性／骨修復不可直接採信 | 二次整合 | §2–5、Table 4 | 所有報告問題明示 | NEEDS_HUMAN_REVIEW |
| 08 | 一致 | 27人54半弓，sham，非54獨立病人 | Table 1確認；irradiance NR | 組間無差異；QoL為手術前後變化 | 人體pilot RCT | Methods、PDF p.4、7 | 登錄／配對方法及敘述歧義保留 | NEEDS_HUMAN_REVIEW |
| 09 | 一致 | 26人13／組，PBM＋HA／guard vs PBM | PMC及PDF Table 1核對 | 癒合組間改善；疼痛不顯著 | 人體合併治療RCT | Table 1、4、Fig.5文字 | 不宣稱獨立PBM效果 | PASS_WITH_LIMITS |

## 未解除問題及最小處理範圍

| 問題ID | 原始證據 | 實際處理／保留結果 |
| --- | --- | --- |
| 02-dose | [原文](https://pmc.ncbi.nlm.nih.gov/articles/PMC9131644/) Radiation protocol／Table 1：0.21 W、0.075 W/cm²、30 s、6.3 J、5 J/cm²；spot 2.8 vs wound 1.26 cm² | 僅審02-E：0.075×30=2.25 J/cm²是本專案算術檢查，不是作者實測，也不取代5；cumulative 6.3 J的範圍待核 |
| 02-count | 同文 Table 5：日0 laser bleeding10、no bleeding14；完成者14人 | 僅保留作者p值與方向、拒算風險率；10+14=24為核對警訊，不自改14為4 |
| 03-dose | [原文](https://pmc.ncbi.nlm.nih.gov/articles/PMC8141316/) Abstract與Methods/Study groups | 50 mW×1.23 min×60=3.69 J只是稽核算式，與11 J不符；原值並列，不填成替代處方 |
| 03-analysis | 同文 Randomization／Statistical analyses | 牙為分派單位、病人可多牙；未見群聚調整與等效界值，留人工判讀 |
| 05-stats | [原文](https://www.mdpi.com/2077-0383/13/18/5402) §3.4、§3.6 | YES／NO編碼Q=0、VAS CI98–99%、AO0.52%皆保留為來源問題；未重算meta-analysis，未編造效應量 |
| 05-bone | 同文 Table 4寫YES，但§3.6／Discussion無骨組間差異 | 拒將YES寫成骨療效；只標矛盾，未另匯入其3篇原始RCT |
| 08-registration | [原文](https://link.springer.com/article/10.1007/s10103-026-04950-0) Methods與Results：收案2022-11-25至2024-05-13，稱prospective的登錄日2024-07-29 | 只記時序衝突；未查登錄網站，不斷言真實登錄歷史或研究不誠實 |
| 08-analysis | 同文 Statistical analysis及PDF Table 3–5 | split-mouth卻用Mann–Whitney組間比較需核；滿意度／OHIP前後變化不能歸因PBM |
| 01-rights | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC5844808/) author manuscript／[Wiley](https://onlinelibrary.wiley.com/doi/10.1111/php.12864) Free Access | 未確認CC再散布授權；只提交自撰事實摘要／連結，全文與圖不提交 |
| 03-rights | PMC Copyright and License information | CC Attribution版本仍未明，無自造版本；PDF不提交 |

未解除的來源問題在複核確認後直接交人工；沒有為了湊滿3次而重試同一段文字。表格取得的真實局部重試另見 [log](../wiki/log.md)。

## 跨文獻差異

02的早期腭供區RWA與08的一期翻瓣傷口結果不同；03是疼痛，09是HA＋guard附加效果；不混成一種共同療效。01機轉不替代臨床證據；05的回顧結論不覆蓋其數值問題。

## 人工決策

確認02／03的劑量是否須查作者／勘誤、05是否僅作批判教材、08是否僅呈陰性結果與方法疑問；決定01／03後續再利用範圍。未獲指示前不聯絡作者、不另生成Wiki正文。
