# مستند Prototype تعاملی

وضعیت طراحی :: **کامل‌شده**  
وضعیت Feature :: **Selected for Validation — نه Validation‌شده**

- [اجرای Prototype](index.html)
- [Figma V2](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl)
- [FigJam — نقشه تصمیم](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3)
- [Q23 — User Journey](../../docs/questions/q23/)
- [Q24 — Low-Fidelity و Prototype](../../docs/questions/q24/)
- [MVP Definition](../../solution/mvp/)
- [Jira Delivery Map](../../delivery/jira/)

## هدف Prototype

Prototype نشان می‌دهد کاربر چگونه از یک نیاز مبهم به فهرست کوتاه و توضیح‌پذیر محصول می‌رسد، بدون اینکه مسیر عادی خرید خانومی حذف شود. این Artifact برای ارزیابی Flow، فهم‌پذیری پیشنهاد، اعتماد و آمادگی ورود به PDP ساخته شده است؛ نه برای اثبات اثر تجاری Feature.

## مسیر اصلی تجربه

**Entry → Need → Questions → Shortlist → Why this product → Alternative → PDP / Cart → Feedback**

کاربر در تمام مسیر باید بتواند:

- از Flow خارج شود و به Browse عادی برگردد
- پاسخ قبلی را اصلاح کند
- دلیل هر پیشنهاد را ببیند
- محصول جایگزین را با Trade-off روشن بررسی کند
- فقط محصول موجود و قابل خرید دریافت کند
- در حالت نبود پیشنهاد معتبر، پیام صادقانه No-match ببیند

## محدوده پیاده‌شده در Prototype

| بخش | رفتار مورد انتظار |
|---|---|
| Entry | ارزش راهنما را کوتاه توضیح می‌دهد و ورود اجباری نیست |
| Question Flow | هر Screen یک تصمیم اصلی، Progress و مسیر Back دارد |
| Recommendation | حداکثر سه پیشنهاد متناسب با پاسخ‌های ثبت‌شده نمایش می‌دهد |
| Explainability | «چرا این محصول؟» را به نیاز و محدودیت کاربر متصل می‌کند |
| Alternative | تفاوت گزینه جایگزین مانند Fit، قیمت یا ترجیح را روشن می‌کند |
| Commerce handoff | مسیر انتقال به PDP و ادامه خرید موجود خانومی را حفظ می‌کند |
| Feedback | مفیدبودن نتیجه و دلیل بازخورد منفی را جمع‌آوری می‌کند |
| Recovery | امکان ویرایش پاسخ‌ها بدون شروع کامل از ابتدا را فراهم می‌کند |
| No-match | به‌جای پیشنهاد ساختگی، نبود گزینه معتبر را اعلام می‌کند |

## قواعد Recommendation

Prototype منطق تجربه را نمایش می‌دهد. موتور پیشنهادی MVP باید Rule-based یا Concierge باشد و این قواعد را رعایت کند:

1. پاسخ‌های مؤثر کاربر به Rule Set نگاشت شوند.
2. SKU ناموجود یا فاقد Product Data کافی حذف شود.
3. پیشنهادها از سه گزینه بیشتر نشوند.
4. دلیل پیشنهاد فقط از داده معتبر محصول و پاسخ کاربر ساخته شود.
5. ادعای پزشکی، قطعیت درمان و اعتماد کاذب تولید نشود.
6. در نبود Match معتبر، سیستم به No-match یا Browse هدایت کند.
7. AI در این مرحله Feature محسوب نمی‌شود و تنها پس از اثبات ارزش MVP می‌تواند روش پیاده‌سازی احتمالی باشد.

## شفافیت و اعتماد

هر Recommendation باید به این سه سؤال پاسخ دهد:

- چرا این محصول به نیاز من مربوط است؟
- این نتیجه بر اساس کدام پاسخ من ساخته شده؟
- اگر مناسب نبود، چه انتخاب یا مسیر جایگزینی دارم؟

اصالت یا ایمنی نباید صرفاً به شکل ادعای تبلیغاتی نمایش داده شود. هر Claim باید به Product Data معتبر، سیاست رسمی یا منبع قابل ردیابی متصل باشد.

## Guardrailها

- جلوگیری از Medical Claim
- جلوگیری از نمایش کالای ناموجود
- جلوگیری از Recommendation بدون دلیل قابل نمایش
- حفظ مسیر عادی خرید و وضعیت سبد
- ثبت و نمایش No-match
- امکان خروج، Back و Edit
- عدم ذخیره ترجیحات حساس بدون رضایت
- امکان Rollback منطق پیشنهاد در Pilot

## رویدادهای لازم برای Validation

| مرحله | Event پیشنهادی |
|---|---|
| مشاهده ورودی واجد شرایط | guide_exposed |
| شروع راهنما | guide_started |
| پاسخ به سؤال | question_answered |
| بازگشت یا اصلاح پاسخ | answer_edited |
| تکمیل Flow | guide_completed |
| نمایش نتیجه | recommendation_viewed |
| مشاهده دلیل | recommendation_reason_opened |
| انتخاب جایگزین | alternative_selected |
| ورود به PDP | recommendation_pdp_clicked |
| افزودن به سبد | recommended_item_added |
| عدم وجود نتیجه معتبر | no_match_shown |
| بازخورد نتیجه | recommendation_feedback_submitted |
| خروج از Flow | guide_exited |

نام نهایی Eventها باید با Taxonomy واقعی Analytics خانومی هماهنگ شود.

## سناریوهای QA و تست کاربردپذیری

### Happy Path

کاربر وارد Flow می‌شود، سؤال‌ها را کامل می‌کند، دلیل پیشنهاد را می‌فهمد و وارد PDP می‌شود.

### Edit Path

کاربر به مرحله قبل برمی‌گردد، یک پاسخ مؤثر را تغییر می‌دهد و نتیجه تازه دریافت می‌کند.

### Alternative Path

کاربر پیشنهاد اصلی را نمی‌پسندد و تفاوت جایگزین را پیش از انتخاب می‌فهمد.

### No-match Path

هیچ محصول معتبر و موجودی مطابق قواعد وجود ندارد و سیستم پیشنهاد ساختگی نمایش نمی‌دهد.

### Exit Path

کاربر در هر مرحله خارج می‌شود و Browse یا سبد قبلی او از بین نمی‌رود.

### Safety Path

ورودی دارای ریسک پزشکی یا نیاز خارج از Scope به مسیر امن و پیام محدودیت هدایت می‌شود.

## معیار پذیرش Prototype

- تمام مسیرهای اصلی قابل کلیک و قابل بازگشت باشند
- CTA اصلی هر Screen واضح باشد
- کاربر بدون توضیح طراح بتواند Flow را ادامه دهد
- دلیل Recommendation قابل فهم و متصل به پاسخ کاربر باشد
- Alternative و No-match رفتار تعریف‌شده داشته باشند
- مسیر PDP، خروج و ویرایش پاسخ‌ها بن‌بست نداشته باشد
- هیچ Claim پزشکی یا موفقیت قطعی Feature نمایش داده نشود
- Prototype در Desktop و Mobile قابل مشاهده باشد

## برنامه تست مشاهده‌ای

Prototype کامل است، اما موفقیت راه‌حل هنوز باید با تست سنجیده شود:

- ۵ تست کاربردپذیری برای کشف مشکل Flow
- Task Completion و نقطه‌های Hesitation و Backtrack
- فهم «چرا این محصول؟»
- توانایی تشخیص تفاوت Alternative
- تمایل به ورود از Recommendation به PDP
- سنجش اعتماد بدون القای اصالت یا قطعیت ساختگی

## مرز ادعا

**Fact:** Prototype تعاملی و مسیرهای طراحی ساخته شده‌اند.  
**Evidence:** مسئله Decision Confidence و نیاز به راهنمایی از سنتز چندمنبعی پروژه پشتیبانی می‌شود.  
**Logical Inference:** توضیح‌پذیری و Shortlist احتمالاً effort انتخاب را کاهش می‌دهند.  
**Hypothesis:** این تجربه Conversion، Retention یا Revenue را افزایش می‌دهد؛ این بخش فقط با آزمایش رفتاری قابل اثبات است.

## Definition of Done این Artifact

- Prototype کلیک‌پذیر موجود است
- Flow اصلی و Edge Stateها مستند شده‌اند
- قواعد Recommendation و Guardrailها مشخص‌اند
- Eventهای لازم برای Validation تعریف شده‌اند
- لینک Figma، Q23، Q24، MVP و Jira برقرار است
- تفاوت «Prototype کامل» و «Feature Validation‌نشده» صریح است
