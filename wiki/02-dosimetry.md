# 第 2 章｜PBM 參數、劑量與雙相劑量反應

[Wiki 首頁](README.md) · [上一章](01-mechanisms.md) · [下一章](03-secondary-healing.md)

## 學習目標

分辨 nm、mW、mW/cm²、J、J/cm²，讀出時間、照射幾何與療程範圍，並用單位核對辨認需要人工確認的欄位。

## 基礎解說

| 欄位 | 閱讀時要問的問題 |
| --- | --- |
| 波長（wavelength，nm） | 光譜位置在哪裡？ |
| 功率（power，mW） | 光源輸出的功率是多少？ |
| 功率密度（irradiance，mW/cm²） | 每單位面積入射多少功率？ |
| 能量（energy，J） | 原文指每點、每次、每顆牙，還是全療程？ |
| 能量密度（fluence，J/cm²） | 用哪個面積定義或估計？ |

在固定功率的簡化情況下，能量可用 W × 秒做單位檢查。對同一位置，若 irradiance 固定，W/cm² × 秒可用來檢查能量密度。光斑、傷口與掃描涵蓋面積各有意義。先辨認單點、單次全區、掃描或多次療程，再判斷原文量值可否互相比對。[Card 02 K2](../cards/02-morshedzadeh-2022.md#k-來源定位驗證) · [02 Radiation protocol／Table 1](https://pmc.ncbi.nlm.nih.gov/articles/PMC9131644/) · [Card 08 K2](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證) · [08 PDF p.4 Table 1／Surface area determination](https://link.springer.com/content/pdf/10.1007/s10103-026-04950-0.pdf)

### 計算示例：相同能量可以分布在不同面積

功率描述每秒傳遞的能量。照射時間決定累積了多少秒，照射面積則決定這些能量分布的範圍。以下是**假設的教學數字**，用於練習單位換算，未取自研究，也不作為照射建議。假設光束均勻、功率固定，且所列功率均入射到指定的照射面積。

1. **換算功率**：100 mW ÷ 1,000＝0.100 W。1 W 等於每秒 1 J。
2. **算總能量**：0.100 W × 20 秒＝2 J。若只把照射時間延長為 40 秒，能量就變成 4 J。
3. **算能量密度**：若這 2 J 均勻分布在 2 cm²，平均 fluence 為 2 J ÷ 2 cm²＝1 J/cm²。若同樣的 2 J 分布在 4 cm²，則為 0.5 J/cm²。總能量相同，單位面積所得能量減半。
4. **用功率密度交叉檢算**：在 2 cm² 的例子，0.100 W ÷ 2 cm²＝0.050 W/cm²，再乘 20 秒，同樣得到 1 J/cm²。

研究報告中的分母要看作者如何界定。若光斑、傷口或掃描涵蓋面積不同，分別記下各自的名稱與數值，避免互相代用。下列案例中的**原文報告值**照錄，**稽核算式**只檢查欄位能否互相吻合，結果不填回原報告。

## 研究案例：先保留原值，再核對單位

- **02 腭側供區**：原文報告 0.21 W、0.075 W/cm²、30 秒、6.3 J、5 J/cm²，光斑 2.8 cm²，傷口 1.26 cm²。稽核算式 0.075 × 30＝2.25 J/cm² 與原報告不同。6.3 J 在正文與表中的總劑量／累計措辭也有歧義。保留 `CONFLICT`，2.25 為檢算結果。[Card 02 K2](../cards/02-morshedzadeh-2022.md#k-來源定位驗證) · [原文 Radiation protocol／Table 1](https://pmc.ncbi.nlm.nih.gov/articles/PMC9131644/)
- **03 拔牙疼痛**：原文以 50 mW 描述 average power density，實測 irradiance 為 `Not reported`。Methods 記 1.23 min／點、11 J／點與 66 J／牙，摘要記 11 J/cm²。稽核算式 0.050 × 1.23 × 60＝3.69 J 仍與 11 J 不一致。並列原值，保留 `CONFLICT`。[Card 03 K2](../cards/03-isolan-2021.md#k-來源定位驗證) · [原文 Abstract／Methods, Study groups，官方 PDF p.3](https://medicinaoral.com/medoralfree01/aop/24228.pdf)
- **08／09 照射範圍**：08 採掃描，離散點數 `Not applicable`，2.04 cm² 為幾何估計，irradiance `Not reported`。09 報告能量 12 J，四次累計能量與離散點數均為 `Not reported`，保留缺欄。[Card 08 K2](../cards/08-da-silva-azevedo-2026.md#k-來源定位驗證) · [08 PDF p.4 Table 1、Fig. 2](https://link.springer.com/content/pdf/10.1007/s10103-026-04950-0.pdf) · [Card 09 K2](../cards/09-yakout-2023.md#k-來源定位驗證) · [09 原文 Table 1](https://pmc.ncbi.nlm.nih.gov/articles/PMC10612174/)

## 證據限制

01 的雙相反應例子來自細胞模型。反應可能隨劑量上升後下降，其中 3 J/cm² 是該例的反應峰值。05 回顧的統一療程為 `Not applicable`，逐篇劑量為 `Not reported in a reproducible dosimetry table`。02、03、05、08 維持 `NEEDS_HUMAN_REVIEW`。這些資料無法用來挑選人體最佳劑量或拼接臨床療程。[Card 01 K2](../cards/01-hamblin-2018.md#k-來源定位驗證) · [01 原文 Fig. 4](https://pmc.ncbi.nlm.nih.gov/articles/PMC5844808/) · [Card 05 K2](../cards/05-giansiracusa-2024.md#k-來源定位驗證) · [05 原文 §3.6–3.7、Table 4](https://www.mdpi.com/2077-0383/13/18/5402)

## 重點整理

先核對單位、面積與時間，再確認照射和累計範圍。計算可指出疑點，作者未報出的欄位仍維持原標記。

## 來源追溯

依上方各 Card 的 A 節確認 DOI 與版本，並由 K2 回到原文表圖。兩項算式的推算身分見 [任務 03 查核](../reviews/task03-audit.md#未解除問題及最小處理範圍)。
