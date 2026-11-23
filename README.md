# pbm-oral-wound-wiki

PBM 與口腔傷口癒合文獻專案。

## 任務 01 狀態

AWAITING_HUMAN_REVIEW。指定七篇文獻已完成書目、合法全文可取得性與授權查核；存取障礙、授權未確認及日期差異均保留在報告，並非七篇全文都已取得。

指定獨立儲存庫：[nycuhhtc-debug/pbm-oral-wound-wiki](https://github.com/nycuhhtc-debug/pbm-oral-wound-wiki)。GitHub 回傳 visibility 為 private，預設分支 main。

## 查閱

- [sources.md](sources.md)：逐篇完整作者、題名、DOI、卷頁／文章號、日期、HTML／PDF 入口、授權與證據 URL。
- [report.md](report.md)：GitHub 確認、交付結果、存取限制與人工審核事項。
- [AGENTS.md](AGENTS.md)：後續工作必須遵守的限制。

## 資料夾

| 路徑 | 用途 | 目前內容 |
| --- | --- | --- |
| metadata/ | 未來結構化書目 | 僅 .gitkeep；未匯入 |
| evidence/ | 未來證據紀錄 | 僅 .gitkeep；本次證據 URL 記於 sources.md |
| reviews/ | 人工審核決定 | 僅 .gitkeep；等待本輪審核 |
| literature/ | 核准後才可保存的全文 | 僅 .gitkeep；全文預設由 Git 忽略 |

## 停止點

使用者已審核的是「候選清單」，目前仍禁止正式 ingest、生成 Wiki 或 HTML 簡報、公開發布。即使個別文章有 CC 授權，也不代表下一階段已獲核准。完成本輪查核後停止，等待人工審核。

專案沒有包含文章全文、PDF、正式 Wiki 或 HTML 簡報。
