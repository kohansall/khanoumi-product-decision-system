**راهنمای کوانتیفیکیشن گام‌های پروژه نهایی**

**بوتکمپ مدیریت محصول آکادمی همراه اول — وب‌سایت خانومی**

**DECAF Quantification v1.0**

راهنمای ساده، علمی و قابل دفاع برای ۳۰ فصل پروژه

**مقدمه**

این راهنما برای یک سؤال ساده ساخته شده است: وقتی در پروژه مدیریت محصول یک نتیجه، اولویت، Feature، KPI یا عدد اقتصادی ارائه می‌کنیم، دقیقاً چقدر باید به آن اعتماد کنیم و چرا؟ هدف این سند ایجاد «عددهای بیشتر» نیست؛ هدف این است که هر عدد، امتیاز یا تصمیم، مسیر روشنی از شواهد تا نتیجه داشته باشد.

پروژه رسمی بوتکمپ از شناخت جریان کاربر و مسئله شروع می‌شود، سپس به تحلیل رقبا و انتخاب Feature می‌رسد و در ادامه MVP، Roadmap، Jira، KPI، Journey، Low-Fi، Acquisition/Retention و مدل مالی را می‌خواهد. بنابراین همه ۳۰ فصل ماهیت یکسان ندارند: بعضی فصل‌ها ادعای پژوهشی و تصمیمی دارند و نیازمند کوانتیفیکیشن‌اند؛ بعضی فصل‌ها Artifact اجرایی یا طراحی‌اند و نمره Confidence برای خود Artifact معنای علمی ندارد.

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>اصل کلیدی<br />
</strong>هر چیزی که قابل اندازه‌گیری است الزاماً نباید اندازه‌گیری شود. کوانتیفیکیشن زمانی ارزش دارد که عدم‌قطعیت تصمیم را کم کند. اگر یک نمره فقط ظاهر علمی بسازد و تصمیم را بهتر نکند، بهتر است از Checklist، Traceability یا Validation Test استفاده شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**DECAF چیست؟**

DECAF مخفف Decision Evidence, Confidence & Assumption Framework است. این نام یک استاندارد جهانیِ آماده نیست؛ یک چارچوب تلفیقی برای این پروژه است که از منطق Evidence Mapping، Triangulation، Sensitivity Analysis، Decision Analysis و Value of Information استفاده می‌کند. هدف آن این است که بین «Fact»، «Evidence»، «Inference» و «Hypothesis» مرز روشن ایجاد کند.

در این چارچوب، Triangulation یعنی یک نتیجه با چند خانواده مستقل شواهد بررسی شود. Survey، Interview، VOC، مشاهده UX، داده رسمی و Product Analytics می‌توانند Evidence Familyهای مستقل باشند؛ اما سه نمودار ساخته‌شده از یک Survey سه منبع مستقل نیستند.

**قاعده مشترک Confidence**

| **کلاس** | **بازه** | **معنا**                                               |
|----------|----------|--------------------------------------------------------|
| A        | 80–100   | قابل پذیرش و دفاع؛ شواهد قوی و محدودیت‌ها کنترل شده‌اند. |
| B        | 60–79    | قابل استفاده با Caveat؛ برای تصمیم موقت مناسب است.     |
| C        | 30–59    | فرضیه/استنتاج؛ Validation بیشتر لازم است.              |
| D        | 0–29     | فاقد ارزش آماری یا معنایی برای تصمیم قطعی.             |

**موتور پایه کوانتیفیکیشن**

برای فصل‌هایی که Confidence Score لازم دارند، منطق پایه ثابت می‌ماند اما وزن ورودی‌ها متناسب با سؤال همان فصل تغییر می‌کند. این باعث می‌شود هم مقایسه‌پذیری حفظ شود و هم سؤال‌های متفاوت به‌زور با یک Weight Map یکسان سنجیده نشوند.

> • Required Data Map: چه داده‌ای واقعاً برای پاسخ لازم است؟
>
> • Available / Missing: چه چیزی داریم و چه چیزی نداریم؟
>
> • Estimable / Ignorable / Critical Unknown: داده گمشده را بر اساس اثرش دسته‌بندی می‌کنیم.
>
> • Evidence Quality: منبع چقدر مستقیم، معتبر و تازه است؟
>
> • Evidence Triangulation: آیا چند خانواده مستقل به نتیجه مشابه رسیده‌اند؟
>
> • Importance Weight: هر ورودی چقدر در تصمیم اهمیت دارد؟
>
> • Decision Sensitivity: اگر این ورودی اشتباه باشد، آیا تصمیم عوض می‌شود؟
>
> • Cap Rule: بعضی Missingهای حیاتی سقف Confidence ایجاد می‌کنند.
>
> • Double-counting Control: یک منبع یا Dataset نباید چند بار امتیاز بگیرد.
>
> • VOI: کدام داده جدید بیشترین ارزش را برای کاهش عدم‌قطعیت دارد؟
>
> • Decision Robustness: آیا نتیجه با تغییر فرض‌های معقول هنوز پابرجاست؟

**Rubric عمومی کیفیت Evidence**

| **امتیاز تقریبی** | **نوع شواهد**                                                     |
|-------------------|-------------------------------------------------------------------|
| 90–100            | داده داخلی مستقیم، telemetry، مشاهده رفتاری معتبر یا آزمایش مناسب |
| 75–89             | منبع رسمی تازه، مشاهده مستقیم، پژوهش ساختاریافته با محدودیت روشن  |
| 50–74             | Proxy معتبر، نمونه Convenience، Benchmark یا شواهد غیرمستقیم      |
| 30–49             | Expert inference یا استنتاج با شواهد محدود                        |
| 0–29              | فرض بدون پشتوانه، داده superseded یا ادعای غیرقابل ردیابی         |

**چرا بعضی فصل‌ها نمره Confidence ندارند؟**

Confidence برای «ادعا درباره واقعیت» یا «تصمیم تحت عدم‌قطعیت» معنا دارد. اما Epic، User Story، Sprint Plan، Journey و Low-Fi در اصل Artifact هستند. برای آن‌ها بهتر است کیفیت ساختاری، Traceability و Testability بررسی شود. اگر به خود Wireframe مثلاً ۸۷٪ Confidence بدهیم، معلوم نیست ۸۷٪ دقیقاً احتمال چه چیزی است؛ این همان precision مصنوعی است که این راهنما می‌خواهد از آن جلوگیری کند.

**نقشه ۳۰ فصل**

| **شماره** | **فصل**                         | **روش ارزیابی**                         |
|-----------|---------------------------------|-----------------------------------------|
| 1         | بازسازی جریان‌های فعلی کاربر     | کوانتیفیکیشن لازم                       |
| 2         | کشف مشکلات تجربه فعلی           | کوانتیفیکیشن لازم                       |
| 3         | اعتبارسنجی و اولویت‌بندی مسائل   | کوانتیفیکیشن لازم                       |
| 4         | استخراج نیازهای مشترک           | کوانتیفیکیشن لازم                       |
| 5         | تعریف رقبا و جایگزین‌ها          | کوانتیفیکیشن لازم                       |
| 6         | مقایسه قابلیت‌های رقبا           | کوانتیفیکیشن لازم                       |
| 7         | الگوهای رهبران جهانی            | کوانتیفیکیشن لازم                       |
| 8         | روندهای جهانی                   | کوانتیفیکیشن لازم                       |
| 9         | استخراج Opportunityها           | کوانتیفیکیشن لازم                       |
| 10        | انتخاب Feature Candidate        | کوانتیفیکیشن لازم                       |
| 11        | اثبات Pain و Market Need        | کوانتیفیکیشن لازم                       |
| 12        | استدلال پژوهشی برای Feature     | کوانتیفیکیشن لازم                       |
| 13        | برآورد Impact مورد انتظار       | کوانتیفیکیشن لازم                       |
| 14        | چرا توسعه این Feature ارزش دارد | کوانتیفیکیشن لازم                       |
| 15        | تعریف Scope MVP                 | کوانتیفیکیشن لازم                       |
| 16        | قابلیت‌ها و بخش‌های اصلی MVP      | کوانتیفیکیشن لازم                       |
| 17        | Roadmap از MVP تا Launch        | کوانتیفیکیشن لازم                       |
| 18        | تعریف Epicها                    | ارزیابی ساختاری / بدون Confidence Score |
| 19        | تعریف User Storyها              | ارزیابی ساختاری / بدون Confidence Score |
| 20        | برنامه Sprintهای دو هفته‌ای      | ارزیابی ساختاری / بدون Confidence Score |
| 21        | تعریف KPIها                     | کوانتیفیکیشن لازم                       |
| 22        | Success Metrics و Guardrails    | کوانتیفیکیشن لازم                       |
| 23        | طراحی User Journey جدید         | ارزیابی ساختاری / بدون Confidence Score |
| 24        | Low-Fidelity Wireframe          | ارزیابی ساختاری / بدون Confidence Score |
| 25        | برنامه Acquisition              | کوانتیفیکیشن لازم                       |
| 26        | برنامه Retention                | کوانتیفیکیشن لازم                       |
| 27        | مدل هزینه                       | کوانتیفیکیشن لازم                       |
| 28        | پیش‌بینی درآمد                   | کوانتیفیکیشن لازم                       |
| 29        | ROI و Payback                   | کوانتیفیکیشن لازم                       |
| 30        | یکپارچه‌سازی و ارائه نهایی       | کوانتیفیکیشن لازم                       |

**فصل 1 — بازسازی جریان‌های فعلی کاربر**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>در این فصل مسیرهای اصلی کاربر در خانومی از نیاز تا خرید و پس از خرید بازسازی می‌شوند. هدف، ترسیم چیزی است که می‌دانیم؛ نه حدس درباره نرخ افت یا رفتارهایی که داده مستقیم برایشان نداریم.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                      | **وزن** |
|--------------------------------|---------|
| مشاهده مستقیم Flowها           | 30٪     |
| پوشش داده‌های لازم              | 25٪     |
| Evidence Triangulation         | 20٪     |
| استقلال از فرض                 | 15٪     |
| Robustness در برابر داده گمشده | 10٪     |

**داده‌های لازم**

> • Landing/Home
>
> • Search/Browse
>
> • PDP/Evaluation
>
> • Chatbot/Support
>
> • Cart/Checkout
>
> • Login/OTP/Address/Payment
>
> • Delivery/Post-purchase
>
> • Repurchase/Switching
>
> • Behavioral analytics
>
> • Edge/failure states

**قواعد تفسیر**

> • Flow مشاهده‌شده را از Flow استنتاجی جدا کن.
>
> • بدون Product Analytics درباره Drop-off یا Frequency ادعا نکن.
>
> • اگر یک Flow فقط از expert review آمده، آن را «فرضیه جریان» بنام.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون Behavioral Analytics می‌توان Flow را بازسازی کرد، اما درباره نرخ افت یا فراوانی رفتار Confidence بالا مجاز نیست.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 2 — کشف مشکلات تجربه فعلی**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل از جریان‌ها به مسئله می‌رسد. هر مشکل باید فراتر از یک برداشت UX باشد و تا حد ممکن با داده کاربر، رفتار، VOC و منابع مستقل پشتیبانی شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| شواهد کاربر فعلی       | 20٪     |
| Never/Lapsed           | 10٪     |
| VOC                    | 15٪     |
| مصاحبه                 | 15٪     |
| UX Observation         | 10٪     |
| پیامد رفتاری           | 10٪     |
| Evidence Triangulation | 10٪     |
| کنترل تعارض            | 5٪      |
| تازگی و Lineage        | 5٪      |

**داده‌های لازم**

> • Current buyer evidence
>
> • Never/Lapsed evidence
>
> • VOC
>
> • Interviews
>
> • UX review
>
> • Behavioral consequences
>
> • Contradictions
>
> • Source lineage

**قواعد تفسیر**

> • فراوانی شکایت به‌تنهایی مساوی اهمیت نیست.
>
> • Problem فقط UX-based حداکثر یک فرضیه متوسط است.
>
> • یک Dataset با چند نمودار، چند منبع مستقل محسوب نمی‌شود.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Problem فقط UX-based: حداکثر 49.
>
> • Problem فقط از یک Evidence Family: معمولاً حداکثر 69.
>
> • نادیده‌گرفتن Counter-evidence مهم: Penalty حداقل 15 امتیاز.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 3 — اعتبارسنجی و اولویت‌بندی مسائل**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>اینجا فقط نمی‌پرسیم «آیا مشکل وجود دارد؟»؛ می‌پرسیم «کدام مشکل آن‌قدر معتبر، رفتاری، قابل اثرگذاری و مهم است که باید جلوتر قرار گیرد؟».</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| Evidence مستقیم        | 20٪     |
| شدت پیامد رفتاری       | 15٪     |
| فراوانی                | 10٪     |
| Evidence Triangulation | 15٪     |
| کیفیت منبع             | 10٪     |
| اثر بیزینسی            | 10٪     |
| Product Addressability | 8٪      |
| تعارض                  | 5٪      |
| Bias Control           | 4٪      |
| Recency                | 3٪      |

**داده‌های لازم**

> • Validation strength
>
> • Behavior impact
>
> • Frequency
>
> • Business impact
>
> • Addressability
>
> • Bias risks
>
> • Contradictions

**قواعد تفسیر**

> • Frequency ≠ Priority.
>
> • مسئله بزرگ اما خارج از کنترل محصول، اولویت محصول لزوماً بالایی ندارد.
>
> • بدون پیامد رفتاری، Confidence اولویت باید محدود شود.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • فقط Frequency بالا: حداکثر 59.
>
> • بدون Behavioral Consequence: حداکثر 74.
>
> • فقط نظر مدیریت یا expert review: حداکثر 59.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 4 — استخراج نیازهای مشترک**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>در این فصل شکایت‌ها و رفتارها به Need و JTBD تبدیل می‌شوند. هدف پیدا کردن نیازهای پایدار است، نه تبدیل یک درخواست Feature به نیاز عمومی همه کاربران.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| مصاحبه                 | 20٪     |
| Current Buyer Survey   | 15٪     |
| Never/Lapsed Survey    | 10٪     |
| VOC                    | 10٪     |
| Behavioral Evidence    | 15٪     |
| Evidence Triangulation | 12٪     |
| Need Abstraction       | 8٪      |
| Segment/Contradiction  | 5٪      |
| Lineage                | 5٪      |

**داده‌های لازم**

> • Interview evidence
>
> • Survey evidence
>
> • VOC patterns
>
> • Observed coping behavior
>
> • Segment coverage
>
> • JTBD abstraction

**قواعد تفسیر**

> • Common Need با Universal Need یکی نیست.
>
> • Feature request را قبل از امتیازدهی به Need مستقل از راه‌حل بازنویسی کن.
>
> • نمونه Convenience را به کل جامعه تعمیم نده.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Need فقط از یک Interview: حداکثر 49.
>
> • Need فقط Survey-based: حداکثر 69.
>
> • تعمیم Need یک Segment به همه کاربران: Penalty حداقل 20.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 5 — تعریف رقبا و جایگزین‌ها**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل مجموعه رقابتی را تعریف می‌کند: رقیب مستقیم، غیرمستقیم، جایگزین و Benchmark. معیار اصلی، شباهت سایت نیست؛ اشتراک در Job و رفتار Switching کاربر است.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                      | **وزن** |
|--------------------------------|---------|
| Market Boundary                | 15٪     |
| Direct competitors             | 20٪     |
| Indirect competitors           | 12٪     |
| Substitutes                    | 12٪     |
| Switching evidence             | 15٪     |
| Business model similarity      | 8٪      |
| Assortment/Positioning overlap | 7٪      |
| Market relevance               | 6٪      |
| Source quality/recency         | 5٪      |

**داده‌های لازم**

> • Market definition
>
> • Direct set
>
> • Indirect set
>
> • Substitutes
>
> • Switching behavior
>
> • Business model
>
> • Positioning

**قواعد تفسیر**

> • Global leader را رقیب مستقیم ایران ننام.
>
> • Substituteهای آفلاین را حذف نکن.
>
> • Scale مساوی relevance رقابتی نیست.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • فقط شباهت وب‌سایت: حداکثر 49.
>
> • حذف Substituteها: Confidence کل مجموعه رقابتی حداکثر 79.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 6 — مقایسه قابلیت‌های رقبا**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>مقایسه رقبا باید از جدول تیک و ضربدر فراتر برود. موضوع اصلی Capability، عمق اجرا، ارتباط با نیاز و نقش آن به‌عنوان Table Stake یا Differentiator است.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Capability taxonomy       | 15٪     |
| Direct coverage           | 15٪     |
| Global benchmark coverage | 10٪     |
| Functional comparability  | 10٪     |
| Verified evidence         | 10٪     |
| Feature depth             | 10٪     |
| User relevance            | 10٪     |
| Strategic relevance       | 8٪      |
| Parity/Differentiation    | 7٪      |
| Recency                   | 5٪      |

**داده‌های لازم**

> • Capability definitions
>
> • Direct competitors
>
> • Global benchmarks
>
> • Feature maturity
>
> • User need mapping
>
> • Strategic role

**قواعد تفسیر**

> • وجود Feature ≠ بلوغ Feature.
>
> • FAQ Chatbot را با Shopping Assistant هم‌ارز نکن.
>
> • Global benchmark اثبات Demand محلی نیست.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Feature بدون verification: حداکثر 49.
>
> • Checklist صرفاً تیک/ضربدر: Confidence کل حداکثر 59.
>
> • Global benchmark به‌عنوان proof of local demand: Penalty حداقل 20.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 7 — الگوهای رهبران جهانی**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>اینجا از چند شرکت موفق، Pattern استخراج می‌کنیم. Pattern وقتی معتبر است که در چند شرکت و با منابع رسمی تکرار شود و برای مسئله خانومی معنای قابل انتقال داشته باشد.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Leader selection          | 15٪     |
| Official evidence         | 15٪     |
| Cross-company replication | 15٪     |
| Strategic significance    | 12٪     |
| User relevance            | 12٪     |
| Business impact evidence  | 10٪     |
| Transferability           | 10٪     |
| Execution maturity        | 6٪      |
| Recency                   | 5٪      |

**داده‌های لازم**

> • Leader rationale
>
> • Official reports
>
> • Replicated patterns
>
> • Business evidence
>
> • Transferability

**قواعد تفسیر**

> • یک Feature تک‌شرکتی را Trend یا Pattern عمومی اعلام نکن.
>
> • Business impact را از صرف وجود Feature جدا کن.
>
> • Transferability به ایران را مستقل ارزیابی کن.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Pattern فقط در یک شرکت: حداکثر 59.
>
> • بدون منبع رسمی: حداکثر 69.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 8 — روندهای جهانی**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>در این فصل Trend واقعی را از Hype جدا می‌کنیم. Trend باید تداوم زمانی، تکرار بین بازارها/شرکت‌ها، اثر رفتاری یا اقتصادی و ارتباط با Beauty Commerce داشته باشد.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Multi-year evidence       | 15٪     |
| Cross-market replication  | 15٪     |
| Cross-company replication | 12٪     |
| Consumer behavior         | 15٪     |
| Business relevance        | 12٪     |
| Technology maturity       | 8٪      |
| Beauty relevance          | 8٪      |
| Transferability           | 8٪      |
| Source quality/recency    | 7٪      |

**داده‌های لازم**

> • Time persistence
>
> • Market replication
>
> • Company replication
>
> • Behavior shift
>
> • Economics
>
> • Tech maturity

**قواعد تفسیر**

> • Tech novelty ≠ strategic value.
>
> • یک خبر یا کمپین، Trend نیست.
>
> • Trend جهانی بدون transferability ممکن است فقط Background باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Signal فقط در یک شرکت یا یک سال: حداکثر 49.
>
> • بدون Consumer Behavior evidence: حداکثر 69.
>
> • Tech hype بدون maturity: حداکثر 59.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 9 — استخراج Opportunityها**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل نقطه اتصال Discovery به Solution Space است. Opportunity باید از Problem و Need معتبر بیرون بیاید و هنوز به یک راه‌حل مشخص قفل نشده باشد.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| Problem evidence       | 18٪     |
| User need strength     | 15٪     |
| Evidence Triangulation | 15٪     |
| Behavioral consequence | 12٪     |
| Business relevance     | 12٪     |
| Market gap             | 10٪     |
| Product addressability | 8٪      |
| Strategic fit          | 5٪      |
| Solution independence  | 5٪      |

**داده‌های لازم**

> • Root problem
>
> • User need
>
> • Evidence families
>
> • Behavioral consequence
>
> • Market gap
>
> • Addressability
>
> • Strategic fit

**قواعد تفسیر**

> • Competitor gap به‌تنهایی Opportunity نیست.
>
> • «ساخت AI Chatbot» Opportunity نیست؛ Solution است.
>
> • اگر Problem پایه ضعیف باشد Opportunity نمی‌تواند بسیار مطمئن باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Opportunity فقط از Competitor Gap: حداکثر 59.
>
> • بدون Behavioral Evidence: حداکثر 74.
>
> • Opportunity که در واقع Solution است: Penalty حداقل 15.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 10 — انتخاب Feature Candidate**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>در این فصل چند مسیر حل مسئله مقایسه می‌شوند و یک Feature Candidate برای Validation انتخاب می‌شود. انتخاب نهایی به معنی Validated Solution نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Opportunity fit           | 20٪     |
| Problem coverage          | 15٪     |
| User value potential      | 15٪     |
| Business value potential  | 15٪     |
| Evidence Triangulation    | 10٪     |
| Feasibility               | 10٪     |
| Strategic fit             | 8٪      |
| Testability/reversibility | 7٪      |

**داده‌های لازم**

> • Top opportunities
>
> • Candidate solutions
>
> • User value
>
> • Business value
>
> • Feasibility
>
> • Testability

**قواعد تفسیر**

> • AI را Feature تعریف نکن؛ Mechanism پیاده‌سازی است.
>
> • قبل از Validation از واژه «برنده قطعی» استفاده نکن.
>
> • Score این فصل ordinal decision index است، نه probability.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Feature Candidate بدون Opportunity معتبر نمی‌تواند Confidence بالا بگیرد.
>
> • انتخاب با Score بالا همچنان Selected for Validation است، نه Validated Solution.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 11 — اثبات Pain و Market Need**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل نشان می‌دهد مسئله منتخب فقط یک UX inconvenience نیست و برای بخشی از بازار پیامد واقعی دارد. باید شدت، تکرار، coping behavior و بازار جایگزین بررسی شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                  | **وزن** |
|----------------------------|---------|
| Pain evidence              | 20٪     |
| Behavioral cost            | 20٪     |
| Segment reach              | 15٪     |
| Market/substitute evidence | 15٪     |
| Evidence Triangulation     | 15٪     |
| Recency/source quality     | 10٪     |
| Counter-evidence control   | 5٪      |

**داده‌های لازم**

> • Pain signals
>
> • Coping behaviors
>
> • Switching
>
> • Segment evidence
>
> • Market/substitute evidence

**قواعد تفسیر**

> • Pain را از «نظر مثبت نسبت به ایده» جدا کن.
>
> • Convenience sample prevalence نیست.
>
> • وجود substitute رفتاری، evidence مهم Market Need است.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Pain فقط opinion-based یا hypothetical: حداکثر 59.
>
> • بدون coping/switching behavior، ادعای Market Need باید Caveat داشته باشد.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 12 — استدلال پژوهشی برای Feature**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل زنجیره استدلال را شفاف می‌کند: Evidence → Problem → Need → Opportunity → Candidate. ارزش اصلی این فصل Traceability است، نه ساخت نمره جدید از صفر.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Traceability completeness | 30٪     |
| Source quality            | 20٪     |
| Evidence Triangulation    | 20٪     |
| Contradiction handling    | 10٪     |
| Assumption visibility     | 10٪     |
| Alternative explanations  | 10٪     |

**داده‌های لازم**

> • Evidence-to-decision links
>
> • Contradictions
>
> • Assumptions
>
> • Rejected alternatives

**قواعد تفسیر**

> • این فصل نباید همان Evidence را دوباره به‌عنوان منبع جدید بشمارد.
>
> • هدف نشان دادن منطق تصمیم است، نه تولید precision مصنوعی.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • اگر زنجیره Evidence→Decision شکسته باشد، Confidence این فصل از ضعیف‌ترین لینک بالاتر نمی‌رود.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 13 — برآورد Impact مورد انتظار**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>در این فصل مسیر اثر Feature بر رفتار و KPI مدل می‌شود. چون Feature هنوز Validation نشده، Impact عددی باید سناریویی یا Range باشد، نه وعده قطعی.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**             | **وزن** |
|-----------------------|---------|
| Mechanism clarity     | 20٪     |
| Metric linkage        | 20٪     |
| Baseline availability | 15٪     |
| Effect-size evidence  | 15٪     |
| Scenario quality      | 10٪     |
| Guardrails            | 10٪     |
| Sensitivity           | 10٪     |

**داده‌های لازم**

> • Causal mechanism
>
> • Baseline metrics
>
> • Expected behavior change
>
> • Benchmarks/experiments
>
> • Guardrails

**قواعد تفسیر**

> • Benchmark competitor را مستقیم به uplift خانومی تبدیل نکن.
>
> • بدون baseline و experiment از عدد قطعی uplift پرهیز کن.
>
> • Impact Map می‌تواند معتبر باشد حتی اگر اثر عددی هنوز نامعلوم است.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون baseline و experiment، uplift عددی حداکثر در سطح scenario/hypothesis است.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 14 — چرا توسعه این Feature ارزش دارد**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل یک Investment Thesis می‌سازد: مسئله مهم است، راه‌حل بالقوه مناسب است، آزمون ارزان ممکن است و upside ارزش بررسی دارد. هنوز Build approval نهایی نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| User value evidence    | 20٪     |
| Business value logic   | 20٪     |
| Strategic fit          | 15٪     |
| Opportunity cost       | 10٪     |
| Feasibility            | 10٪     |
| Risk/uncertainty       | 10٪     |
| Testability            | 10٪     |
| Alternative comparison | 5٪      |

**داده‌های لازم**

> • User value
>
> • Business logic
>
> • Strategy
>
> • Risks
>
> • Alternatives
>
> • Testability

**قواعد تفسیر**

> • Worth testing را با Worth fully building یکی نکن.
>
> • Opportunity cost را فراموش نکن.
>
> • اگر uncertainty بالا است، توصیه باید Experiment باشد نه Build.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • اگر uncertainty بالا باشد، خروجی درست «ارزش تست دارد» است نه «ارزش ساخت قطعی دارد».

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 15 — تعریف Scope MVP**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل کمترین Scope لازم برای آزمودن فرضیه ارزش را مشخص می‌کند. MVP قرار نیست نسخه ناقص محصول نهایی باشد؛ باید کمترین چیزی باشد که یادگیری معتبر ایجاد کند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                | **وزن** |
|--------------------------|---------|
| Hypothesis coverage      | 25٪     |
| Minimum scope discipline | 20٪     |
| User value completeness  | 15٪     |
| Measurability            | 15٪     |
| Feasibility              | 10٪     |
| Risk/safety              | 10٪     |
| Reversibility            | 5٪      |

**داده‌های لازم**

> • Core hypothesis
>
> • Minimum experience
>
> • Measurement events
>
> • Safety rules
>
> • Excluded scope

**قواعد تفسیر**

> • هر Feature اضافه باید دلیل آزمایشی داشته باشد.
>
> • Fake Door/Concierge می‌تواند MVP معتبر باشد اگر سؤال تصمیمی را جواب دهد.
>
> • Minimum به معنی بی‌کیفیت نیست.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • MVP که فرضیه اصلی را نمی‌آزماید، حتی اگر کوچک باشد MVP معتبر این پروژه نیست.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 16 — قابلیت‌ها و بخش‌های اصلی MVP**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>در این فصل MVP به Capabilityهای روشن شکسته می‌شود: ورودی، سؤال کوتاه، پیشنهاد، دلیل پیشنهاد، اتصال به PDP/Cart و اندازه‌گیری. هدف جلوگیری از Scope creep است.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**             | **وزن** |
|-----------------------|---------|
| Core value coverage   | 25٪     |
| Capability necessity  | 20٪     |
| Flow completeness     | 15٪     |
| Measurement readiness | 15٪     |
| Data dependency       | 10٪     |
| Safety/edge states    | 10٪     |
| Complexity control    | 5٪      |

**داده‌های لازم**

> • Entry
>
> • Question flow
>
> • Preference capture
>
> • Recommendation output
>
> • Why this product
>
> • PDP/cart handoff
>
> • Analytics
>
> • Safety states

**قواعد تفسیر**

> • Capability لازم را از Nice-to-have جدا کن.
>
> • هر Capability باید به Hypothesis یا Guardrail وصل باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Capability بدون اتصال به Hypothesis/Guardrail باید از MVP حذف یا Nice-to-have شود.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 17 — Roadmap از MVP تا Launch**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Roadmap در این پروژه سند تعهد زمانی قطعی نیست؛ نقشه یادگیری و کاهش ریسک است. مراحل باید بر اساس dependency و evidence gate مرتب شوند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**         | **وزن** |
|-------------------|---------|
| Outcome alignment | 20٪     |
| Learning sequence | 20٪     |
| Dependency logic  | 15٪     |
| Stage gates       | 15٪     |
| Feasibility       | 10٪     |
| Risk reduction    | 10٪     |
| Time realism      | 10٪     |

**داده‌های لازم**

> • Phases
>
> • Dependencies
>
> • Exit criteria
>
> • Validation gates
>
> • Risks

**قواعد تفسیر**

> • Roadmap را Feature calendar نساز.
>
> • بدون ظرفیت واقعی تیم، تاریخ دقیق را با Caveat ارائه کن.
>
> • هر مرحله باید شرط عبور داشته باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون ظرفیت واقعی تیم، تاریخ/velocity دقیق Confidence پایینی دارد.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 18 — تعریف Epicها**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Epicها واحدهای بزرگ Execution هستند، نه بخش‌های گزارش. باید Feature را به قابلیت‌های معنی‌دار قابل تحویل بشکنند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**آیا این فصل نیاز به کوانتیفیکیشن دارد؟**

خیر، برای خود Artifact نمره Confidence توصیه نمی‌شود. دلیل این است که این فصل در درجه اول «چیزی برای اجرا یا تست» می‌سازد، نه یک ادعای احتمالی درباره واقعیت. عدد درصدی در اینجا احتمالاً precision مصنوعی تولید می‌کند.

**روش ارزیابی مناسب‌تر**

> • برای Epic عدد confidence مستقل لازم نیست؛ کیفیت آن با معیارهای ساختاری بررسی می‌شود: پوشش Scope، مرزبندی روشن، dependency و قابلیت شکستن به Story.
>
> • اگر خواستی Score بدهی، آن Score باید «Execution Quality» باشد، نه Evidence Confidence.

| **معیار کیفیت Epic** | **پرسش کنترل**                           |
|----------------------|------------------------------------------|
| Scope coverage       | آیا Epic بخشی لازم از MVP را پوشش می‌دهد؟ |
| Boundary             | آیا با Epicهای دیگر overlap مبهم ندارد؟  |
| Decomposability      | آیا به Storyهای قابل اجرا شکسته می‌شود؟   |
| Dependency           | وابستگی‌ها روشن‌اند؟                       |
| Traceability         | به MVP/Opportunity لینک دارد؟            |

**فصل 19 — تعریف User Storyها**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Story باید یک نیاز کاربر و outcome قابل مشاهده را بیان کند و Acceptance Criteria داشته باشد. این فصل بیشتر مهندسی اجراست تا استنتاج پژوهشی.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**آیا این فصل نیاز به کوانتیفیکیشن دارد؟**

خیر، برای خود Artifact نمره Confidence توصیه نمی‌شود. دلیل این است که این فصل در درجه اول «چیزی برای اجرا یا تست» می‌سازد، نه یک ادعای احتمالی درباره واقعیت. عدد درصدی در اینجا احتمالاً precision مصنوعی تولید می‌کند.

**روش ارزیابی مناسب‌تر**

> • کوانتیفیکیشن Evidence برای هر Story ضروری نیست.
>
> • بهتر است از Checklist کیفیت استفاده شود: Actor روشن، Need روشن، Value روشن، AC تست‌پذیر، وابستگی مشخص.
>
> • اگر Story مستقیماً یک فرضیه را آزمایش می‌کند، لینک Evidence/Experiment ثبت شود.

| **معیار کیفیت Story** | **پرسش کنترل**                |
|-----------------------|-------------------------------|
| Actor                 | برای چه کاربری است؟           |
| Need                  | چه نیازی را بیان می‌کند؟       |
| Value                 | چه ارزشی ایجاد می‌شود؟         |
| Acceptance Criteria   | آیا تست‌پذیر است؟              |
| Traceability          | به Epic/Hypothesis لینک دارد؟ |

**فصل 20 — برنامه Sprintهای دو هفته‌ای**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Sprint plan نشان می‌دهد کار چگونه به قطعات اجرایی تبدیل می‌شود. عددسازی درباره hours یا velocity بدون داده واقعی تیم علمی نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**آیا این فصل نیاز به کوانتیفیکیشن دارد؟**

خیر، برای خود Artifact نمره Confidence توصیه نمی‌شود. دلیل این است که این فصل در درجه اول «چیزی برای اجرا یا تست» می‌سازد، نه یک ادعای احتمالی درباره واقعیت. عدد درصدی در اینجا احتمالاً precision مصنوعی تولید می‌کند.

**روش ارزیابی مناسب‌تر**

> • این فصل نیاز به Confidence Score پژوهشی ندارد.
>
> • معیار درست: ظرفیت واقعی، dependency، Sprint Goal، DoD و ریسک.
>
> • اگر ظرفیت/velocity نداریم، Sprintها «planning proposal» هستند نه forecast قطعی.

| **معیار Sprint** | **پرسش کنترل**                  |
|------------------|---------------------------------|
| Sprint Goal      | یک outcome روشن دارد؟           |
| Capacity realism | با ظرفیت واقعی سازگار است؟      |
| Dependencies     | ترتیب کار منطقی است؟            |
| DoD              | تعریف پایان روشن است؟           |
| Risk             | ریسک‌های مسدودکننده دیده شده‌اند؟ |

**فصل 21 — تعریف KPIها**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>KPI باید موفقیت Feature را به رفتار و outcome وصل کند. اینجا کمّی‌سازی ضروری است چون بدون تعریف numerator، denominator، window و baseline، KPI قابل سنجش نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| Metric-to-outcome fit  | 25٪     |
| Operational definition | 20٪     |
| Baseline availability  | 15٪     |
| Sensitivity to feature | 15٪     |
| Data availability      | 10٪     |
| Lag/lead balance       | 10٪     |
| Gaming resistance      | 5٪      |

**داده‌های لازم**

> • North-star/primary metric
>
> • Funnel metrics
>
> • Baselines
>
> • Event definitions
>
> • Time windows

**قواعد تفسیر**

> • Vanity metric را KPI ننام.
>
> • هر KPI باید فرمول و window داشته باشد.
>
> • اگر baseline نداریم، KPI معتبر است ولی target عددی باید موقت یا TBD باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون تعریف دقیق numerator/denominator/window، KPI از نظر اندازه‌گیری ناقص است.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 22 — Success Metrics و Guardrails**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Success فقط رشد Conversion نیست. Guardrailها بررسی می‌کنند Feature هم‌زمان به تجربه، ایمنی، مرجوعی، شکایت یا اعتماد آسیب نزند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Primary success metric    | 25٪     |
| Guardrail coverage        | 20٪     |
| Threshold rationale       | 15٪     |
| Measurement feasibility   | 15٪     |
| Statistical detectability | 10٪     |
| Risk relevance            | 10٪     |
| Decision rule             | 5٪      |

**داده‌های لازم**

> • Primary outcome
>
> • Guardrails
>
> • Thresholds
>
> • Sample requirements
>
> • Decision rules

**قواعد تفسیر**

> • Threshold بی‌مبنای تاریخی نساز.
>
> • Success criteria باید قبل از آزمایش نوشته شود.
>
> • Guardrail کمّی اگر baseline ندارد می‌تواند ابتدا directional باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Threshold بی‌baseline یا بی‌منطق باید Hypothesis/TBD برچسب بخورد.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 23 — طراحی User Journey جدید**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Journey جدید یک مدل طراحی از تجربه آینده است. خود Journey لزوماً نیاز به Confidence Score ندارد؛ اما هر تغییر مهم در آن باید به Need یا Evidence قبلی Trace شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**آیا این فصل نیاز به کوانتیفیکیشن دارد؟**

خیر، برای خود Artifact نمره Confidence توصیه نمی‌شود. دلیل این است که این فصل در درجه اول «چیزی برای اجرا یا تست» می‌سازد، نه یک ادعای احتمالی درباره واقعیت. عدد درصدی در اینجا احتمالاً precision مصنوعی تولید می‌کند.

**روش ارزیابی مناسب‌تر**

> • کوانتیفیکیشن خود Journey ارزش کمی دارد و می‌تواند precision مصنوعی ایجاد کند.
>
> • به‌جای Score، Traceability Matrix بساز: Step → Need → Evidence → Intended outcome → Metric.
>
> • اگر درباره کاهش زمان یا drop-off ادعا می‌کنی، آن ادعا جداگانه Quantify شود.

| **معیار Journey**  | **پرسش کنترل**                |
|--------------------|-------------------------------|
| Need traceability  | هر Step به Need وصل است؟      |
| Friction reduction | چه frictionی قرار است کم شود؟ |
| Outcome            | نتیجه مورد انتظار چیست؟       |
| Metric link        | چگونه بعداً سنجیده می‌شود؟      |

**فصل 24 — Low-Fidelity Wireframe**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Low-Fi ابزار یادگیری است، نه نتیجه آماری. کیفیت آن با وضوح فرضیه، پوشش Flow، تست‌پذیری و کم‌هزینه‌بودن سنجیده می‌شود؛ نه Confidence درصدی.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**آیا این فصل نیاز به کوانتیفیکیشن دارد؟**

خیر، برای خود Artifact نمره Confidence توصیه نمی‌شود. دلیل این است که این فصل در درجه اول «چیزی برای اجرا یا تست» می‌سازد، نه یک ادعای احتمالی درباره واقعیت. عدد درصدی در اینجا احتمالاً precision مصنوعی تولید می‌کند.

**روش ارزیابی مناسب‌تر**

> • Low-Fi به‌خودی‌خود «نیاز به کوانتیفیکیشن» ندارد چون یک Artifact برای تست است، نه claim درباره واقعیت.
>
> • معیار درست: آیا سناریوی اصلی را نمایش می‌دهد؟ آیا کاربر می‌تواند Task را انجام دهد؟ آیا فرضیه‌های حساس را قابل تست می‌کند؟
>
> • بعد از Usability Test، نتایج تست کمّی/کیفی می‌شوند؛ نه خود Wireframe.

| **معیار Low-Fi**    | **پرسش کنترل**                        |
|---------------------|---------------------------------------|
| Hypothesis coverage | فرضیه حساس را قابل تست می‌کند؟         |
| Task completeness   | کاربر می‌تواند سناریوی اصلی را طی کند؟ |
| Fidelity discipline | جزئیات غیرضروری حذف شده‌اند؟           |
| Alternative states  | حالت خطا/عدم تطابق دیده شده؟          |
| Testability         | می‌توان usability test اجرا کرد؟       |

**فصل 25 — برنامه Acquisition**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Acquisition plan باید نشان دهد چه کسانی، از چه کانالی و با چه پیام/CTA وارد Feature می‌شوند. بدون CAC و channel baseline، forecast دقیق نباید ساخته شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**             | **وزن** |
|-----------------------|---------|
| Target segment fit    | 20٪     |
| Channel evidence      | 15٪     |
| Message-problem fit   | 15٪     |
| Reach feasibility     | 10٪     |
| CAC/traffic baseline  | 15٪     |
| Experimentability     | 10٪     |
| Attribution readiness | 10٪     |
| Risk                  | 5٪      |

**داده‌های لازم**

> • Target segment
>
> • Channels
>
> • Traffic baseline
>
> • CAC/CTR/CVR
>
> • Messaging
>
> • Attribution

**قواعد تفسیر**

> • بدون channel economics، برنامه را آزمایشی بنویس نه forecast قطعی.
>
> • Owned traffic برای Fake Door می‌تواند اولویت داشته باشد چون CAC incremental پایین‌تر است.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون CAC/traffic baseline، forecast Acquisition باید آزمایشی باشد.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 26 — برنامه Retention**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Retention باید به چرخه مصرف Beauty و ارزش تکرارشونده Feature وصل شود. صرف push notification یا loyalty idea برنامه Retention نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                 | **وزن** |
|---------------------------|---------|
| Repeat-job evidence       | 20٪     |
| Behavioral cycle evidence | 15٪     |
| Retention baseline        | 15٪     |
| Feature recurrence value  | 20٪     |
| Trigger quality           | 10٪     |
| Measurement plan          | 10٪     |
| Guardrails                | 5٪      |
| Feasibility               | 5٪      |

**داده‌های لازم**

> • Repurchase behavior
>
> • Usage cycle
>
> • Retention baselines
>
> • Triggers
>
> • Recurring value
>
> • Measurement

**قواعد تفسیر**

> • Retention mechanism باید به Job تکرارشونده وصل باشد.
>
> • بدون cohort baseline، target retention را قطعی اعلام نکن.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون cohort baseline، target retention قطعی ساخته نشود.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 27 — مدل هزینه**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>هزینه باید از Scope، نفر-ماه، نرخ معتبر و هزینه‌های incremental ساخته شود. عدد کل بدون این زنجیره، حتی اگر ظاهراً دقیق باشد، قابل دفاع نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**              | **وزن** |
|------------------------|---------|
| Scope decomposition    | 20٪     |
| Role/effort estimate   | 20٪     |
| Rate evidence          | 20٪     |
| Incremental cost logic | 15٪     |
| Vendor/infra/ops       | 10٪     |
| Contingency/range      | 10٪     |
| Sensitivity            | 5٪      |

**داده‌های لازم**

> • Scope
>
> • Roles
>
> • Allocation
>
> • Duration
>
> • Salary benchmarks
>
> • Infra/vendor
>
> • Operations
>
> • Contingency

**قواعد تفسیر**

> • روش: Scope → Components → People → Effort → Rate → Cost.
>
> • Shared overhead را فقط اگر causal است تخصیص بده.
>
> • Range و scenario بهتر از یک عدد ساختگی است.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون role-effort-rate chain، عدد کل هزینه فاقد دفاع است.
>
> • عدد یک‌نقطه‌ای بدون range برای ورودی‌های نامطمئن ممنوع.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 28 — پیش‌بینی درآمد**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>Revenue forecast باید از funnel و unit economics ساخته شود، نه از درصد رشد دلخواه. ورودی‌های نامعلوم باید Range و sensitivity داشته باشند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**                | **وزن** |
|--------------------------|---------|
| Eligible volume baseline | 15٪     |
| Adoption/completion      | 15٪     |
| Baseline purchase rate   | 15٪     |
| Effect-size assumption   | 15٪     |
| AOV/contribution         | 15٪     |
| Scenario/range design    | 10٪     |
| Sensitivity              | 10٪     |
| Evidence quality         | 5٪      |

**داده‌های لازم**

> • Eligible sessions
>
> • Adoption
>
> • Completion
>
> • Baseline CVR
>
> • Uplift
>
> • AOV
>
> • Contribution margin

**قواعد تفسیر**

> • GMV با Revenue و Contribution یکی نیست.
>
> • Uplift بدون experiment باید Range باشد.
>
> • Forecast باید Base/Bear/Bull یا distribution داشته باشد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • بدون baseline purchase rate و contribution economics، forecast قطعی مجاز نیست.
>
> • Uplift بدون experiment باید Range باشد.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 29 — ROI و Payback**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>این فصل خروجی مدل هزینه و درآمد است. چون دو مدل upstream نامطمئن‌اند، ROI باید عدم‌قطعیت را حمل کند و نتیجه به‌صورت Range/Probability/Break-even دیده شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**               | **وزن** |
|-------------------------|---------|
| Cost model quality      | 20٪     |
| Revenue model quality   | 20٪     |
| Contribution economics  | 15٪     |
| Time horizon            | 10٪     |
| Uncertainty propagation | 15٪     |
| Sensitivity             | 10٪     |
| Break-even logic        | 10٪     |

**داده‌های لازم**

> • Total incremental cost
>
> • Incremental contribution
>
> • Timing
>
> • Ranges/distributions
>
> • Break-even

**قواعد تفسیر**

> • ROI یک عدد منفرد نده اگر ورودی‌ها Range هستند.
>
> • Break-even spend و payback scenario اغلب دفاع‌پذیرتر از precision جعلی است.
>
> • اگر Q27/Q28 ضعیف باشند، Q29 هم Cap می‌خورد.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • Confidence Q29 از کیفیت Q27 و Q28 بالاتر نمی‌رود.
>
> • ورودی‌های Range باید uncertainty خود را به ROI منتقل کنند.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**فصل 30 — یکپارچه‌سازی و ارائه نهایی**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>خلاصه روایت فصل<br />
</strong>فصل آخر تمام زنجیره را به یک روایت تصمیمی تبدیل می‌کند: چه می‌دانستیم، چه فهمیدیم، چه انتخاب کردیم، چه چیزی هنوز نامعلوم است و قدم بعدی چیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**سؤال کوانتیفیکیشن**

در این فصل می‌خواهیم بفهمیم آیا نتیجه به اندازه کافی بر شواهد، منطق و داده‌های لازم متکی است که بتوان از آن برای تصمیم بعدی استفاده کرد؛ و اگر نه، دقیقاً کدام عدم‌قطعیت مانع است.

**معیارها و وزن‌ها**

| **معیار**               | **وزن** |
|-------------------------|---------|
| Traceability end-to-end | 25٪     |
| Narrative coherence     | 15٪     |
| Evidence integrity      | 15٪     |
| Decision clarity        | 15٪     |
| Uncertainty honesty     | 10٪     |
| Artifact consistency    | 10٪     |
| Executive usability     | 10٪     |

**داده‌های لازم**

> • Brief coverage
>
> • 30-question traceability
>
> • Evidence registry
>
> • Decision log
>
> • Jira/Figma links
>
> • Final narrative

**قواعد تفسیر**

> • Presentation نباید uncertainty را پنهان کند.
>
> • Selected for Validation را Validated Solution معرفی نکن.
>
> • اعداد در اسلاید باید با Source/Assumption status سازگار باشند.

**روش محاسبه**

برای هر معیار یک نمره ۰ تا ۱۰۰ تعیین می‌شود. نمره هر معیار در وزن آن ضرب و مجموع وزنی محاسبه می‌شود. سپس Cap Ruleها و Penaltyهای از پیش تعریف‌شده اعمال می‌شوند. نمره نهایی «Confidence تصمیمی» است، نه احتمال آماری وقوع یک رویداد.

**کنترل Triangulation و Double Counting**

هر Evidence Family فقط یک‌بار در Triangulation شمرده می‌شود. مشتقات یک Dataset، فایل‌های تحلیلی ساخته‌شده از همان داده، یا مقاله‌هایی که یک منبع اصلی را بازنشر کرده‌اند مستقل محسوب نمی‌شوند.

**Sensitivity و VOI**

در پایان مشخص می‌شود کدام ورودی‌ها High / Medium / Low Sensitivity هستند. سپس برای داده‌های گمشده، VOI تعیین می‌شود: اگر جمع‌آوری یک داده احتمال تغییر تصمیم را بالا ببرد، اولویت اندازه‌گیری آن بیشتر است.

**Cap Ruleهای ویژه فصل**

> • تناقض بین Confluence/Jira/Figma/Presentation یا استفاده از ادعای superseded، Confidence نهایی را کاهش می‌دهد.

**خروجی پیشنهادی فصل**

> • خلاصه نتیجه
>
> • Required Data و وضعیت دسترسی
>
> • Evidence Families و Triangulation
>
> • Assumptions / Critical Unknowns
>
> • Score و کلاس A/B/C/D
>
> • Sensitivity و VOI
>
> • Next Evidence Action

**ضمیمه A — قالب ثابت هر فصل کوانتیفیکیشن‌دار**

> • ۱. خلاصه روایت فصل: چه اتفاقی افتاد و چرا این فصل وجود دارد؟
>
> • ۲. سؤال تصمیمی: دقیقاً چه چیزی را می‌خواهیم بدانیم؟
>
> • ۳. Required Data: چه داده‌هایی برای پاسخ لازم‌اند؟
>
> • ۴. Have / Missing: چه داریم و چه نداریم؟
>
> • ۵. Missing Classification: Estimable / Ignorable / Critical Unknown.
>
> • ۶. Weight Map: اهمیت هر ورودی.
>
> • ۷. Evidence Triangulation: خانواده‌های مستقل شواهد.
>
> • ۸. Score Calculation: امتیاز وزنی و کلاس Confidence.
>
> • ۹. Cap Rules / Penalties: محدودیت‌های سخت.
>
> • ۱۰. Sensitivity: کدام فرض می‌تواند تصمیم را عوض کند؟
>
> • ۱۱. VOI: ارزش جمع‌آوری داده بعدی.
>
> • ۱۲. Decision Robustness: آیا با تغییر فرض‌ها نتیجه پابرجاست؟
>
> • ۱۳. Next Evidence Action: قدم بعدی دقیق.

**ضمیمه B — برچسب وضعیت ادعاها**

| **برچسب**         | **تعریف**                                                   |
|-------------------|-------------------------------------------------------------|
| Fact              | مستقیماً در منبع معتبر یا داده مشاهده‌شده وجود دارد.          |
| Evidence          | مشاهده‌ای که یک نتیجه را پشتیبانی می‌کند اما خود نتیجه نیست.  |
| Logical Inference | استنتاج منطقی از شواهد؛ باید صریحاً برچسب بخورد.             |
| Hypothesis        | توضیح یا پیش‌بینی قابل آزمون که هنوز Validation کافی ندارد.  |
| Decision          | انتخاب مدیریتی بر اساس Evidence + Constraints + Trade-offs. |

**ضمیمه C — منابع روش‌شناختی و مبنای پروژه**

۱. فایل رسمی «پروژه پایانی — خانومی» آکادمی همراه: مبنای ۱۲ گام رسمی پروژه و Deliverableهای نهایی.

۲. Douglas W. Hubbard, How to Measure Anything, 2nd Ed.: مبنای فکری برای اندازه‌گیری عدم‌قطعیت، Value of Information، Range و تصمیم‌گیری تحت عدم‌قطعیت.

۳. The Product Book: مبنای تعریف MVP به‌عنوان کمترین Scope لازم برای ارائه ارزش/یادگیری، نه محصول ناقص.

۴. Escaping the Build Trap: مبنای جداسازی Outcome/Strategy از Feature output و اتصال Roadmap به ارزش و تصمیم.

۵. مواد دوره مدیریت محصول و کشف محصول: مبنای عملی برای KPI، Cohort، Discovery، User Research، Prototype و Experimentation.

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>یادآوری نهایی<br />
</strong>DECAF یک چارچوب سفارشی برای این پروژه است، نه استاندارد رسمی آکادمی همراه یا یک متد جهانی با این نام. ارزش آن در Traceability، کنترل فرض‌ها، جلوگیری از Double Counting و صادق‌ماندن درباره عدم‌قطعیت است.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
