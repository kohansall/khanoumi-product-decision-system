# Data Lineage

| مرحله | Canonical artifact | تبدیل | محدودیت |
|---|---|---|---|
| Raw | `voc/raw/khanoumi-comments-anonymized.csv` | فقط Privacy scrub | داده خام اصلی دارای PII خارج Repo است |
| Cleaned | `voc/cleaned/khanoumi-comments-cleaned-anonymized.csv` | cleaning + classification + Privacy scrub | 39,737 rows؛ self-selected reviews |
| Analysis | `voc/analysis/` و Dashboard | aggregation/filter | نه نماینده کل کاربران |
| Synthesis | Q02–Q09 | triangulation | Survey files مستقل ناقص‌اند |
| Decision | Q10–Q16 | opportunity/feature selection | Selected for Validation |
