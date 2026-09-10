# Data Lineage

| مرحله | Canonical artifact | تبدیل | محدودیت |
|---|---|---|---|
| Raw | `voc/raw/manifest.json` + ordered CSV shards | فقط Privacy scrub | داده خام اصلی دارای PII خارج Repo است |
| Cleaned | `voc/cleaned/manifest.json` + ordered CSV shards | cleaning + classification + Privacy scrub | 39,737 rows؛ self-selected reviews |
| Analysis | `voc/analysis/` و Dashboard | aggregation/filter | نه نماینده کل کاربران |
| Synthesis | Q02–Q09 | triangulation | Survey files مستقل ناقص‌اند |
| Decision | Q10–Q16 | opportunity/feature selection | Selected for Validation |
