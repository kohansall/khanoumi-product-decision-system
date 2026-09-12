# گزارش Audit نهایی

## منتقل‌شده

- Q01 تا Q30 به‌صورت Markdown کامل و DOCX منبع
- Prototype canonical، Presentation، نقشه‌های Discovery، NiniSite analysis، Benchmark و Opportunity Map
- VOC raw و cleaned به‌صورت anonymized و CSV shardهای دارای Manifest؛ یک Dataset منطقی برای هر لایه
- ۷۶٬۸۳۷ کامنت خام Crawl‌شده و ۳۹٬۷۳۷ رکورد Cleaned و Canonical با نقش‌های جدا در Lineage
- خروجی تعاملی دو Survey شامل Current Buyers با `n=46` و Never/Lapsed با `n=28`
- Jira mapping و لینک‌های Issue-level

## Deduplicate‌شده

- فایل cleaned با ۳۹٬۷۳۷ ردیف به‌عنوان نسخه canonical پس از کنترل Lineage و Deduplication انتخاب شد؛ نسخه ۱۱۵٬۹۷۹ ردیفی به‌دلیل تعارض Lineage وارد Repo نشد. عدد ۷۶٬۸۳۷ فقط تعداد کامنت خام Crawl‌شده است.
- Prototype HTML فقط در `design/prototype/index.html` نگهداری و از `solution/prototype` لینک شده است.
- Qها فقط یک نسخه canonical دارند و بخش‌های موضوعی به آن‌ها لینک می‌دهند.

## Anonymized‌شده

- نام کاربر، شناسه Comment، تصویر و ستون‌های تماس حذف شدند.
- الگوهای Email، موبایل، شماره ده‌رقمی و Handle در متن کامنت Redact شدند.

## وارد Repo نشده

- PDFهای تجاری، کتاب‌ها و گزارش‌های دارای Copyright؛ فقط citation و یادداشت استفاده ثبت شده است.
- نسخه‌های VOC دارای PII.
- Raw response-level دارای قابلیت بازتولید کامل برای Surveyهای Current Buyers و Never/Lapsed؛ خروجی تحلیلی قابل‌ارائه آن‌ها در Repo موجود است.
- مصاحبه داروخانه به‌صورت فایل مستقل چون Artifact منبع پیدا نشد.
- Speaker Notes محرمانه؛ وجود آن بررسی شد اما مطابق Privacy policy در Repo عمومی منتشر نشد.

## Gapهای باز

- Baseline داخلی Funnel، MDE و Sample Size
- Capacity و Estimate واقعی Engineering
- اقتصاد واحد Feature-specific برای Q27 تا Q29
- Export مستقل FigJam داخل Repo موجود نیست؛ لینک مستقیم FigJam و Figma V2 ثبت شده‌اند
- Validation واقعی؛ وضعیت Feature همچنان Selected for Validation است
- Raw response-level Surveyها و Pharmacy Interview فقط در صورت بازیابی، بررسی PII و مجازبودن انتشار افزوده شوند
