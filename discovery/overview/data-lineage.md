# Data Lineage

| مرحله | Canonical artifact | تبدیل | محدودیت |
|---|---|---|---|
| Raw | `../voc/raw/manifest.json` + ordered CSV shards | فقط Privacy scrub | 76,837 کامنت Crawl‌شده؛ داده دارای PII خارج Repo است |
| Cleaned | `../voc/cleaned/manifest.json` + ordered CSV shards | Lineage control + cleaning + deduplication + classification + Privacy scrub | 39,737 رکورد canonical؛ self-selected reviews |
| Analysis | `../voc/analysis/` و `../voc/interactive-dashboard/` | aggregation/filter | نه نماینده کل کاربران |
| Synthesis | `../../docs/questions/q02/` تا `../../docs/questions/q09/` | triangulation | Surveyها موجودند اما Raw response-level عمومی نیست؛ محدودیت بازتولید حفظ شود |
| Decision | `../../docs/questions/q10/` تا `../../docs/questions/q16/` | opportunity/feature selection | Selected for Validation |

تعداد ۷۶٬۸۳۷ مربوط به Commentهای خام Crawl‌شده است و تعداد ۳۹٬۷۳۷ به Dataset پاک‌سازی‌شده و Canonical مربوط است؛ هیچ‌کدام تعداد User نیست.
