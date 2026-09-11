# Success Metrics و Guardrails

این بخش معیارهای موفقیت و محدودیت‌های Guided Beauty Decision Assistant را تعریف می‌کند. Target عددی تا زمان دسترسی به Baseline، حجم ترافیک و MDE ثبت نمی‌شود.

## North Star پیشنهادی

**Qualified Recommendation to Purchase Rate**

تعداد Sessionهایی که کاربر Recommendation واجد شرایط را دیده و در پنجره Attribution تعریف‌شده خرید مرتبط انجام داده است، تقسیم بر Sessionهای واجد شرایطی که Recommendation را دریافت کرده‌اند.

این Metric فقط با تعریف دقیق Eligibility، Attribution Window، SKU relation و کنترل Repeat Session معتبر است.

## Funnel اصلی

| مرحله | تعریف رویداد | Metric |
|---|---|---|
| Exposure | نمایش Entry راهنمای انتخاب به کاربر واجد شرایط | Eligible Exposure |
| Start | شروع Guide پس از Exposure | Start Rate |
| Answer | ثبت پاسخ معتبر هر مرحله | Step Completion |
| Complete | تکمیل تمام سؤال‌های لازم | Guide Completion Rate |
| Recommendation | مشاهده Result و دلایل پیشنهاد | Recommendation View |
| Engagement | کلیک روی Recommendation یا Why This Product | Recommendation CTR |
| PDP | ورود به PDP مرتبط | PDP Click Rate |
| Cart | افزودن SKU پیشنهادی به سبد | Recommendation ATC |
| Purchase | خرید SKU مرتبط در Window تعریف‌شده | Qualified Recommendation to Purchase |
| Feedback | ثبت مفید یا نامفید بودن پیشنهاد | Helpful Rate |

## Guardrailهای تجربه

| Guardrail | تعریف | علامت خطر |
|---|---|---|
| Curious Click | Start بالا بدون Completion یا تعامل با Result | CTA توجه می‌گیرد اما ارزش ادامه ندارد |
| Step Drop off | خروج در هر سؤال | سؤال مبهم، طولانی یا کم‌ارزش است |
| Invalid Answer | پاسخ ناسازگار یا ناقص | منطق ورودی برای کاربر روشن نیست |
| No Match | نبود SKU مناسب | Coverage موجودی یا Ruleها ناکافی است |
| Edit Loop | ویرایش چندباره پاسخ‌ها بدون انتخاب | نتیجه برای کاربر قابل فهم یا قابل اعتماد نیست |
| Negative Feedback | نامفید یا نامرتبط | Recommendation Quality پایین است |

## Guardrailهای اعتماد و ایمنی

| Guardrail | تعریف | اقدام |
|---|---|---|
| Hidden Advertising Perception | کاربر نتیجه را تبلیغ پنهان می‌داند | نمایش دلیل، Sponsorship و منطق رتبه‌بندی |
| Unsupported Claim | Claim بدون منبع درباره سازگاری یا اثر محصول | حذف Claim و بررسی محتوایی |
| Medical Risk | نیاز پزشکی یا نشانه پرریسک | توقف Recommendation و Referral |
| Authenticity Concern | افزایش سؤال یا شکایت اصالت | بررسی Source و پیام تضمین اصالت |
| Unsafe Recommendation | پیشنهاد ناسازگار با Constraint ثبت‌شده | Kill Switch برای Rule یا SKU |

## Guardrailهای تجاری و عملیاتی

| Guardrail | تعریف | دلیل |
|---|---|---|
| Return Rate | مرجوعی SKUهای پیشنهادشده | CTR بالا با Wrong Fit موفقیت نیست |
| Cancellation Rate | لغو سفارش مرتبط | کیفیت یا موجودی Recommendation را کنترل می‌کند |
| Complaint Rate | تماس یا شکایت پس از پیشنهاد | آسیب اعتماد را آشکار می‌کند |
| Out of Stock Exposure | پیشنهاد SKU ناموجود | Reliability تجربه را کاهش می‌دهد |
| Margin Dilution | افت Contribution Margin در سبدهای مرتبط | رشد Revenue بدون کیفیت اقتصادی کافی نیست |
| Support Load | افزایش تماس مرتبط با Guide | Complexity یا ابهام راه‌حل را نشان می‌دهد |

## Decision Rule

نتیجه آزمایش فقط با یک Metric تعیین نمی‌شود:

- Demand باید با Start و Completion دیده شود.
- Recommendation Quality باید با Engagement، Helpful Rate و No Match کنترل شود.
- اثر رفتاری باید در PDP، Cart یا Purchase ظاهر شود.
- شکایت، مرجوعی، لغو، ایمنی و اعتماد نباید بدتر شوند.

اگر CTR افزایش یابد اما مرجوعی، شکایت یا Wrong Fit بالا برود، Feature موفق محسوب نمی‌شود.

## وضعیت عددها

Baseline، MDE، Sample Size و Thresholdهای Go یا Iterate یا Stop هنوز به داده واقعی خانومی نیاز دارند. هر عدد فعلی Prototype فقط برای نمایش UI است و Target آزمایش محسوب نمی‌شود.

## منابع داخلی پروژه

- [Q21 KPI](../../docs/questions/q21/)
- [Q22 Success Metrics و Guardrails](../../docs/questions/q22/)
- [Validation Plan](../../solution/validation/)
- [Quantification Guide](../../docs/methodology/quantification-guide.md)

