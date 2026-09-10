# گزارش Audit نهایی

## منتقل‌شده

- Q01 تا Q30 به‌صورت Markdown کامل و DOCX منبع
- Prototype canonical، Presentation، نقشه‌های Discovery، NiniSite analysis، Benchmark و Opportunity Map
- VOC raw و cleaned به‌صورت anonymized
- Jira mapping و لینک‌های Issue-level

## Deduplicate‌شده

- فایل cleaned با ۳۹٬۷۳۷ ردیف به‌عنوان نسخه canonical انتخاب شد؛ نسخه ۱۱۵٬۹۷۹ ردیفی به‌دلیل تعارض با Source-of-Truth و Lineage وارد Repo نشد.
- Prototype HTML فقط در `design/prototype/index.html` نگهداری و از `solution/prototype` لینک شده است.
- Qها فقط یک نسخه canonical دارند و بخش‌های موضوعی به آن‌ها لینک می‌دهند.

## Anonymized‌شده

- نام کاربر، شناسه Comment، تصویر و ستون‌های تماس حذف شدند.
- الگوهای Email، موبایل، شماره ده‌رقمی و Handle در متن کامنت Redact شدند.

## وارد Repo نشده

- PDFهای تجاری، کتاب‌ها و گزارش‌های دارای Copyright؛ فقط citation و یادداشت استفاده ثبت شده است.
- نسخه‌های VOC دارای PII.
- Surveyهای Current Buyers و Never/Lapsed چون فایل مستقل آن‌ها در موجودی قابل بازیابی نبود.
- مصاحبه داروخانه به‌صورت فایل مستقل چون Artifact منبع پیدا نشد.

## Gapهای باز

- Baseline داخلی Funnel، MDE و Sample Size
- Capacity و Estimate واقعی Engineering
- اقتصاد واحد Feature-specific برای Q27 تا Q29
- لینک مستقیم FigJam مستقل؛ Figma V2 موجود است
- Validation واقعی؛ وضعیت Feature همچنان Selected for Validation است
- Survey Current Buyers، Survey Never/Lapsed و Pharmacy Interview باید در صورت یافتن فایل اصل افزوده شوند
