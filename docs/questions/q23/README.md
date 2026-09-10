**سؤال 23 — User Journey Feature جدید**

**نحوه تعامل کاربر با Guided Beauty Decision Assistant**

نسخه مستقل و قابل ارائه \| مبتنی بر Evidence Base پروژه خانومی

**نمره دفاع‌پذیری فعلی: 95 از ۱۰۰**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>صورت سؤال بوتکمپ<br />
</strong>«جهت‌نمای مسیر کاربری را برای نشان دادن نحوه تعامل کاربران با قابلیت جدید رسم کنید. همچنین وایرفریم‌های Low-Fidelity برای نمایش این ویژگی ایجاد کنید.»</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

منبع: پروژه پایانی بوتکمپ مدیریت محصول آکادمی همراه، گام نهم.

**استوری‌لاین**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>هدف Journey<br />
</strong>Feature باید دقیقاً در شکاف بین Discovery و Confident Decision وارد شود؛ نه اینکه مسیر خرید موجود را از نو بسازد.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سناریوی اصلی**

کاربر نیاز دارد یک محصول Beauty مناسب پیدا کند، Need را می‌داند اما SKU قطعی ندارد، و می‌خواهد قبل از خرید بفهمد کدام گزینه مناسب‌تر است.

**Journey پیشنهادی**

| **مرحله**      | **کار کاربر**                     | **سیستم**                              | **ریسک/فرصت**              |
|----------------|-----------------------------------|----------------------------------------|----------------------------|
| 1\. Entry      | CTA راهنمای انتخاب را می‌بیند      | Eligibility و context تشخیص داده می‌شود | CTA باید مرتبط باشد        |
| 2\. Need       | نیاز را انتخاب می‌کند              | Question path مناسب فعال می‌شود         | taxonomy نباید پیچیده باشد |
| 3\. Questions  | ۴–۶ سؤال پاسخ می‌دهد               | فضای recommendation محدود می‌شود        | drop-off                   |
| 4\. Results    | ۳ گزینه می‌بیند                    | فقط SKU موجود + explanation            | overload/irrelevance       |
| 5\. Confidence | دلیل و alternative را بررسی می‌کند | why-this-product نمایش داده می‌شود      | trust/explainability       |
| 6\. PDP        | روی گزینه کلیک می‌کند              | ورود به PDP موجود                      | continuity                 |
| 7\. Purchase   | سبد/پرداخت موجود                  | Feature از commerce flow خارج می‌شود    | checkout guardrail         |
| 8\. Feedback   | نتیجه را مفید/نامفید می‌زند        | learning signal ثبت می‌شود              | feedback bias              |

**Happy Path**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Flow<br />
</strong>Need → Start → Questions → Shortlist → Why → PDP → Cart → Purchase</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Alternative Paths**

• کاربر وسط سؤال‌ها منصرف می‌شود → بازگشت امن به Browse.

• Recommendation مناسب نیست → Alternative یا Edit Answers.

• SKU ناموجود می‌شود → گزینه حذف و replacement.

• کاربر توضیح بیشتری می‌خواهد → PDP/Reviews.

• نیاز پزشکی/پرریسک مطرح می‌شود → عدم recommendation و referral/escalation.

**Touchpoints و Metrics**

| **Touchpoint** | **Metric**                 |
|----------------|----------------------------|
| CTA            | Start Rate                 |
| Question Flow  | Completion / Step drop-off |
| Results        | Recommendation CTR         |
| PDP Bridge     | ATC                        |
| Purchase       | Purchase Rate              |
| Feedback       | Helpful Rate / mismatch    |

**نریتیو ارائه**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Talk Track<br />
</strong>«Journey جدید مسیر خرید خانومی را عوض نمی‌کند؛ فقط بین Discovery و Decision یک لایه guidance اضافه می‌کند. کاربر نیازش را می‌گوید، چند سؤال کوتاه جواب می‌دهد، سه پیشنهاد توضیح‌پذیر می‌گیرد و بعد به PDP و checkout فعلی برمی‌گردد. برای هر مرحله مسیر خروج و metric هم تعریف شده است.»</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Audit و نمره**

**نمره فعلی: ۹۵ از ۱۰۰**

• Journey به Problem و MVP trace می‌شود.

• کمبود: مشاهده usability واقعی برای اصلاح micro-steps لازم است.

**رفرنس‌ها**

• پروژه پایانی بوتکمپ مدیریت محصول آکادمی همراه — صورت سؤال رسمی.

• Survey خریداران ۱۲ ماه اخیر خانومی — n=46.

• Survey Never/Lapsed — n=28.

• khanoumi-comments-cleaned.csv — 39,737 کامنت Cleaned.

• مصاحبه‌های عمیق کاربران پروژه خانومی.

• گزارش مدیر محصول — Product Data Gap، recommendation usage، friction خرید و KPIهای داخلی.

• گزارش مدیرعامل — جهت‌گیری profitability/efficiency/resilience و context بیزینس.

• UX Review پروژه خانومی.

• گزارش رسمی خانومی ۱۴۰۴ — users، repeat/return، NPS، OTD، Return Rate، BNPL و basket metrics.

• Benchmark پروژه — Ulta، Sephora، Nykaa و نمونه‌های داخلی.

نسخه: شهریور ۱۴۰۵
