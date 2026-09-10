<span dir="rtl">سؤال 16</span>

<span dir="rtl">قابلیت‌ها و بخش‌های اصلی MVP</span>

<span dir="rtl">MVP Core Capabilities</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">خلاصه فصل</span></p>
<p><span dir="rtl">در این فصل MVP به Capabilityهای قابل ساخت و تست شکسته شد. هر Capability یا باید Hypothesis اصلی را آزمایش کند، یا measurement را ممکن کند، یا Guardrail باشد. هر چیزی غیر از این، Nice-to-have است و از MVP حذف می‌شود.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

| <span dir="rtl">Confidence نهایی</span> | <span dir="rtl">کلاس</span>                  | <span dir="rtl">امتیاز خام</span> | <span dir="rtl">روش</span>                       |
|-----------------------------------------|----------------------------------------------|-----------------------------------|--------------------------------------------------|
| <span dir="rtl">93 / 100</span>         | <span dir="rtl">A — قابل پذیرش و دفاع</span> | <span dir="rtl">93.0</span>       | <span dir="rtl">DECAF Quantification v1.0</span> |

<span dir="rtl"></span>

<span dir="rtl">این نمره احتمال آماری موفقیت نیست؛ یک Decision Confidence Score ترتیبی است که کیفیت Evidence، پوشش داده لازم، Triangulation، فرض‌ها و حساسیت به Missing Data را خلاصه می‌کند.</span>

<span dir="rtl">۱. روایت فصل — چه اتفاقی افتاد؟</span>

<span dir="rtl">در این فصل MVP به Capabilityهای قابل ساخت و تست شکسته شد. هر Capability یا باید Hypothesis اصلی را آزمایش کند، یا measurement را ممکن کند، یا Guardrail باشد. هر چیزی غیر از این، Nice-to-have است و از MVP حذف می‌شود.</span>

<span dir="rtl">۲. سؤال تصمیمی</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Decision Question</span></p>
<p><span dir="rtl">MVP دقیقاً چه بخش‌هایی لازم دارد تا تجربه Guided Decision را بسازد، اندازه بگیرد و ایمن نگه دارد؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<span dir="rtl">۳. نتیجه پروژه در این مرحله</span>

| <span dir="rtl">موضوع</span>                             | <span dir="rtl">وضعیت</span> | <span dir="rtl">Evidence / جایگاه</span>                            | <span dir="rtl">تفسیر</span>                 |
|----------------------------------------------------------|------------------------------|---------------------------------------------------------------------|----------------------------------------------|
| <span dir="rtl">1. Entry / Eligibility</span>            | <span dir="rtl">ضروری</span> | <span dir="rtl">CTA + exposure tracking</span>                      | <span dir="rtl">Demand gate.</span>          |
| <span dir="rtl">2. Need Capture</span>                   | <span dir="rtl">ضروری</span> | <span dir="rtl">concern / goal</span>                               | <span dir="rtl">ورودی تصمیم.</span>          |
| <span dir="rtl">3. Short Question Flow</span>            | <span dir="rtl">ضروری</span> | <span dir="rtl">۴–۶ سؤال + back/edit</span>                         | <span dir="rtl">Preference capture.</span>   |
| <span dir="rtl">4. Recommendation Logic</span>           | <span dir="rtl">ضروری</span> | <span dir="rtl">manual/rule-based + in-stock + safety</span>        | <span dir="rtl">هسته hypothesis.</span>      |
| <span dir="rtl">5. Result Page</span>                    | <span dir="rtl">ضروری</span> | <span dir="rtl">۳ پیشنهاد + Why this product + alternative</span>   | <span dir="rtl">Explainability.</span>       |
| <span dir="rtl">6. Commerce Handoff</span>               | <span dir="rtl">ضروری</span> | <span dir="rtl">PDP / cart path</span>                              | <span dir="rtl">Business signal.</span>      |
| <span dir="rtl">7. Analytics</span>                      | <span dir="rtl">ضروری</span> | <span dir="rtl">exposure/start/completion/click/ATC/purchase</span> | <span dir="rtl">Measurement.</span>          |
| <span dir="rtl">8. Feedback & Safety States</span>       | <span dir="rtl">ضروری</span> | <span dir="rtl">مناسب بود/نبود، fallback، medical boundary</span>   | <span dir="rtl">Guardrail + learning.</span> |
| <span dir="rtl">9. Rich profile / AI / cross-sell</span> | <span dir="rtl">بعدی</span>  | <span dir="rtl">Scale features</span>                               | <span dir="rtl">برای MVP لازم نیست.</span>   |

<span dir="rtl"></span>

<span dir="rtl">۴. Evidence Base و مرز استنتاج</span>

<span dir="rtl">• صورت سؤال رسمی پروژه نهایی بوتکمپ مدیریت محصول آکادمی همراه.</span>

<span dir="rtl">• Survey خریداران اخیر خانومی — n=46؛ نمونه Convenience و فقط توصیف‌کننده همان نمونه.</span>

<span dir="rtl">• Survey Never/Lapsed — n=28؛ 17 Never و 11 Lapsed؛ نمونه Convenience.</span>

<span dir="rtl">• khanoumi-comments-cleaned.csv — 39,737 کامنت تمیزشده؛ Dataset مرجع VOC.</span>

<span dir="rtl">• مصاحبه‌های عمیق کاربران پروژه خانومی؛ استفاده به‌صورت Evidence رفتاری و نه برآورد شیوع.</span>

<span dir="rtl">• UX Review پروژه — Landing، Chatbot و Purchase/Checkout؛ مشاهده کارشناسی، نه Usability Test.</span>

<span dir="rtl">• گزارش مدیر محصول و گزارش مدیرعامل — Context داخلی؛ بدون استفاده از نام افراد.</span>

<span dir="rtl">• گزارش‌های رسمی خانومی ۱۴۰۲ تا ۱۴۰۴ و Benchmarkهای معتبر پروژه برای Context بازار و عملکرد.</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">مرز مهم</span></p>
<p><span dir="rtl">هرجا داده مستقیم نداریم، نتیجه با برچسب «استنتاج» یا «فرضیه» بیان می‌شود. مشتقات یک Dataset به‌عنوان منابع مستقل در Triangulation شمرده نمی‌شوند.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<span dir="rtl">۵. داده‌های لازم و وضعیت دسترسی</span>

| <span dir="rtl">ورودی لازم</span>              | <span dir="rtl">وزن اهمیت</span> | <span dir="rtl">وضعیت فعلی</span>           | <span dir="rtl">Evidence Score</span> |
|------------------------------------------------|----------------------------------|---------------------------------------------|---------------------------------------|
| <span dir="rtl">Entry</span>                   | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">95/100</span>         |
| <span dir="rtl">Question Flow</span>           | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">95/100</span>         |
| <span dir="rtl">Preference Capture</span>      | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">92/100</span>         |
| <span dir="rtl">Recommendation Output</span>   | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">95/100</span>         |
| <span dir="rtl">Why This Product</span>        | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">92/100</span>         |
| <span dir="rtl">PDP/Cart Handoff</span>        | <span dir="rtl">10٪</span>       | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">95/100</span>         |
| <span dir="rtl">Analytics</span>               | <span dir="rtl">8٪</span>        | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">90/100</span>         |
| <span dir="rtl">Safety / Failure States</span> | <span dir="rtl">7٪</span>        | <span dir="rtl">داریم / قابل استفاده</span> | <span dir="rtl">85/100</span>         |

<span dir="rtl"></span>

<span dir="rtl">۶. Missing Data: چه چیزی را می‌توانیم و نمی‌توانیم حل کنیم؟</span>

<span dir="rtl">• schema دقیق سؤالات بر اساس Category</span>

<span dir="rtl">• catalog/API constraints واقعی</span>

<span dir="rtl">• failure states واقعی بعد از tech discovery</span>

<span dir="rtl">طبقه‌بندی:</span>

<span dir="rtl">• قابل برآورد: فقط وقتی range یا proxy معتبر داریم و نتیجه نسبت به آن Robust باشد.</span>

<span dir="rtl">• قابل اغماض: داده‌ای که نبودنش تصمیم این فصل را تغییر نمی‌دهد.</span>

<span dir="rtl">• Critical Unknown: داده‌ای که می‌تواند Ranking، Feature Selection یا توصیه Build/Test را عوض کند؛ برای آن عددسازی نمی‌کنیم.</span>

<span dir="rtl">۷. مدل کوانتیفیکیشن اختصاصی فصل</span>

<span dir="rtl">وزن معیارها بین فصل‌ها متفاوت است چون سؤال تصمیمی متفاوت است؛ اما قواعد پایه DECAF، تعریف Confidence، Triangulation، Cap Rule و Double-counting Control ثابت می‌مانند.</span>

| <span dir="rtl">معیار</span>                   | <span dir="rtl">وزن</span> | <span dir="rtl">نمره ۰–۱۰۰</span> | <span dir="rtl">سهم وزنی</span> |
|------------------------------------------------|----------------------------|-----------------------------------|---------------------------------|
| <span dir="rtl">Entry</span>                   | <span dir="rtl">15٪</span> | <span dir="rtl">95</span>         | <span dir="rtl">14.2</span>     |
| <span dir="rtl">Question Flow</span>           | <span dir="rtl">15٪</span> | <span dir="rtl">95</span>         | <span dir="rtl">14.2</span>     |
| <span dir="rtl">Preference Capture</span>      | <span dir="rtl">15٪</span> | <span dir="rtl">92</span>         | <span dir="rtl">13.8</span>     |
| <span dir="rtl">Recommendation Output</span>   | <span dir="rtl">15٪</span> | <span dir="rtl">95</span>         | <span dir="rtl">14.2</span>     |
| <span dir="rtl">Why This Product</span>        | <span dir="rtl">15٪</span> | <span dir="rtl">92</span>         | <span dir="rtl">13.8</span>     |
| <span dir="rtl">PDP/Cart Handoff</span>        | <span dir="rtl">10٪</span> | <span dir="rtl">95</span>         | <span dir="rtl">9.5</span>      |
| <span dir="rtl">Analytics</span>               | <span dir="rtl">8٪</span>  | <span dir="rtl">90</span>         | <span dir="rtl">7.2</span>      |
| <span dir="rtl">Safety / Failure States</span> | <span dir="rtl">7٪</span>  | <span dir="rtl">85</span>         | <span dir="rtl">6.0</span>      |

<span dir="rtl"></span>

<span dir="rtl">امتیاز خام = 93.0 از 100</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Confidence نهایی</span></p>
<p><span dir="rtl">93/100 — A — قابل پذیرش و دفاع</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<span dir="rtl">۸. Rubric ثابت Evidence Quality</span>

| <span dir="rtl">بازه</span>   | <span dir="rtl">تفسیر</span>                                                                |
|-------------------------------|---------------------------------------------------------------------------------------------|
| <span dir="rtl">90–100</span> | <span dir="rtl">داده مستقیم/رسمی تازه یا رفتار مشاهده‌شده معتبر؛ محدودیت‌ها روشن.</span>      |
| <span dir="rtl">75–89</span>  | <span dir="rtl">Evidence قوی ولی با یک یا چند gap غیرکشنده.</span>                          |
| <span dir="rtl">50–74</span>  | <span dir="rtl">Proxy معتبر، نمونه محدود یا Evidence تک‌روشی؛ قابل استفاده با Caveat.</span> |
| <span dir="rtl">30–49</span>  | <span dir="rtl">استنتاج کارشناسی یا داده ضعیف؛ Hypothesis.</span>                           |
| <span dir="rtl">0–29</span>   | <span dir="rtl">بدون پشتوانه کافی؛ فاقد ارزش برای تصمیم قطعی.</span>                        |

<span dir="rtl"></span>

<span dir="rtl">۹. Evidence Triangulation و Double Counting</span>

<span dir="rtl">Triangulation یعنی رسیدن خانواده‌های مستقل Evidence به یک نتیجه مشابه. استقلال مهم‌تر از تعداد فایل‌هاست. Survey، Interview و VOC می‌توانند سه خانواده مستقل باشند؛ اما Chart، Persona و Summary ساخته‌شده از همان Survey سه منبع مستقل نیستند.</span>

<span dir="rtl">• Data Triangulation: چند منبع/نمونه مستقل.</span>

<span dir="rtl">• Method Triangulation: ترکیب Survey، Interview، Observation/Behavior و تحلیل اسنادی.</span>

<span dir="rtl">• یک Evidence Family فقط یک‌بار در شمارش استقلال لحاظ می‌شود.</span>

<span dir="rtl">۱۰. Cap Rules ویژه این فصل</span>

<span dir="rtl">• Capability بدون اتصال به Hypothesis یا Guardrail باید حذف یا Nice-to-have شود.</span>

<span dir="rtl">• فقط SKU موجود/قابل خرید در recommendation نمایش داده شود.</span>

<span dir="rtl">• هیچ تشخیص پزشکی در MVP نباشد.</span>

<span dir="rtl">۱۱. Sensitivity، Robustness و VOI</span>

<span dir="rtl">Sensitivity می‌پرسد اگر یک ورودی اشتباه باشد، آیا تصمیم عوض می‌شود؟ Robustness می‌پرسد آیا نتیجه با تغییر فرض‌های معقول پابرجا می‌ماند؟ VOI مشخص می‌کند جمع‌آوری کدام داده جدید بیشترین احتمال کاهش عدم‌قطعیت تصمیم را دارد.</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">بالاترین VOI فعلی</span></p>
<p><span dir="rtl">پس از انتخاب Category، Question schema و product-data requirements را با تیم فنی/محتوا finalize و Acceptance Criteria را در Jira بشکنیم.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<span dir="rtl">۱۲. آنچه این فصل هنوز ثابت نمی‌کند</span>

<span dir="rtl">• Selected for Validation به معنی Validated Solution نیست.</span>

<span dir="rtl">• بدون Experiment، causal uplift یا ROI قطعی ادعا نمی‌شود.</span>

<span dir="rtl">• Benchmark یا نظر مدیریت به‌تنهایی جای behavior واقعی کاربر را نمی‌گیرد.</span>

<span dir="rtl">۱۳. جمع‌بندی قابل ارائه</span>

<span dir="rtl">نتیجه Q16: در این فصل MVP به Capabilityهای قابل ساخت و تست شکسته شد. هر Capability یا باید Hypothesis اصلی را آزمایش کند، یا measurement را ممکن کند، یا Guardrail باشد. هر چیزی غیر از این، Nice-to-have است و از MVP حذف می‌شود.</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Next Evidence Action</span></p>
<p><span dir="rtl">پس از انتخاب Category، Question schema و product-data requirements را با تیم فنی/محتوا finalize و Acceptance Criteria را در Jira بشکنیم.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<span dir="rtl">۱۴. Source Registry</span>

<span dir="rtl">• صورت سؤال رسمی پروژه نهایی بوتکمپ مدیریت محصول آکادمی همراه.</span>

<span dir="rtl">• Survey خریداران اخیر خانومی — n=46؛ نمونه Convenience و فقط توصیف‌کننده همان نمونه.</span>

<span dir="rtl">• Survey Never/Lapsed — n=28؛ 17 Never و 11 Lapsed؛ نمونه Convenience.</span>

<span dir="rtl">• khanoumi-comments-cleaned.csv — 39,737 کامنت تمیزشده؛ Dataset مرجع VOC.</span>

<span dir="rtl">• مصاحبه‌های عمیق کاربران پروژه خانومی؛ استفاده به‌صورت Evidence رفتاری و نه برآورد شیوع.</span>

<span dir="rtl">• UX Review پروژه — Landing، Chatbot و Purchase/Checkout؛ مشاهده کارشناسی، نه Usability Test.</span>

<span dir="rtl">• گزارش مدیر محصول و گزارش مدیرعامل — Context داخلی؛ بدون استفاده از نام افراد.</span>

<span dir="rtl">• گزارش‌های رسمی خانومی ۱۴۰۲ تا ۱۴۰۴ و Benchmarkهای معتبر پروژه برای Context بازار و عملکرد.</span>

<span dir="rtl">نسخه: شهریور ۱۴۰۵ \| روش: DECAF Quantification v1.0 \| وضعیت: سند مستقل Q16</span>
