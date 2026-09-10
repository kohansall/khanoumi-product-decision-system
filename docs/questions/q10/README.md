<span dir="rtl">سؤال 10</span>

<span dir="rtl">انتخاب Feature Candidate</span>

<span dir="rtl">Feature Selection</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">خلاصه فصل</span></p>
<p><span dir="rtl">از Opportunity اصلی، چند Solution candidate ساخته و مقایسه شدند. خروجی این مرحله «Guided Beauty Decision Assistant» است؛ اما فقط به‌عنوان Selected for Validation. AI خودِ Feature نیست و implementation نهایی هنوز باز است. امتیاز بالای یک candidate در Decision Index، احتمال موفقیت یا اثبات Market Fit نیست.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

| <span dir="rtl">Confidence نهایی</span> | <span dir="rtl">کلاس</span>                       | <span dir="rtl">امتیاز خام</span> | <span dir="rtl">روش</span>                       |
|-----------------------------------------|---------------------------------------------------|-----------------------------------|--------------------------------------------------|
| <span dir="rtl">72 / 100</span>         | <span dir="rtl">B — قابل استفاده با Caveat</span> | <span dir="rtl">83.0</span>       | <span dir="rtl">DECAF Quantification v1.0</span> |

<span dir="rtl"></span>

<span dir="rtl">این نمره احتمال آماری موفقیت نیست؛ یک Decision Confidence Score ترتیبی است که کیفیت Evidence، پوشش داده لازم، Triangulation، فرض‌ها و حساسیت به Missing Data را خلاصه می‌کند.</span>

<span dir="rtl">۱. روایت فصل — چه اتفاقی افتاد؟</span>

<span dir="rtl">از Opportunity اصلی، چند Solution candidate ساخته و مقایسه شدند. خروجی این مرحله «Guided Beauty Decision Assistant» است؛ اما فقط به‌عنوان Selected for Validation. AI خودِ Feature نیست و implementation نهایی هنوز باز است. امتیاز بالای یک candidate در Decision Index، احتمال موفقیت یا اثبات Market Fit نیست.</span>

<span dir="rtl">۲. سؤال تصمیمی</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Decision Question</span></p>
<p><span dir="rtl">آیا Guided Beauty Decision Assistant بهترین Candidate فعلی برای Validation است، با توجه به User Value، Business Value، Feasibility و Testability؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<span dir="rtl">۳. نتیجه پروژه در این مرحله</span>

| <span dir="rtl">موضوع</span>                            | <span dir="rtl">وضعیت</span>                          | <span dir="rtl">Evidence / جایگاه</span> | <span dir="rtl">تفسیر</span>                                                                  |
|---------------------------------------------------------|-------------------------------------------------------|------------------------------------------|-----------------------------------------------------------------------------------------------|
| <span dir="rtl">Guided Beauty Decision Assistant</span> | <span dir="rtl">Selected for Validation</span>        | <span dir="rtl">Decision Index 96</span> | <span dir="rtl">به Opportunity اصلی نزدیک، قابل Fake Door/Concierge و قابل اندازه‌گیری.</span> |
| <span dir="rtl">Human Consultation</span>               | <span dir="rtl">Alternative</span>                    | <span dir="rtl">77</span>                | <span dir="rtl">Evidence نیاز دارد ولی operationally سنگین‌تر.</span>                          |
| <span dir="rtl">Trust Layer</span>                      | <span dir="rtl">Alternative / supporting</span>       | <span dir="rtl">74</span>                | <span dir="rtl">برای بخشی از users مهم؛ کمتر از Decision Support جامع.</span>                 |
| <span dir="rtl">AI Advisor</span>                       | <span dir="rtl">Implementation-heavy candidate</span> | <span dir="rtl">67</span>                | <span dir="rtl">AI mechanism است؛ قبل از demand validation زود است.</span>                    |
| <span dir="rtl">Loyalty</span>                          | <span dir="rtl">Lower priority</span>                 | <span dir="rtl">55</span>                | <span dir="rtl">Retention value دارد اما به root pre-purchase friction کمتر نزدیک است.</span> |

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

| <span dir="rtl">ورودی لازم</span>                     | <span dir="rtl">وزن اهمیت</span> | <span dir="rtl">وضعیت فعلی</span>              | <span dir="rtl">Evidence Score</span> |
|-------------------------------------------------------|----------------------------------|------------------------------------------------|---------------------------------------|
| <span dir="rtl">Opportunity Fit</span>                | <span dir="rtl">20٪</span>       | <span dir="rtl">داریم / قابل استفاده</span>    | <span dir="rtl">95/100</span>         |
| <span dir="rtl">User Value</span>                     | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span>    | <span dir="rtl">90/100</span>         |
| <span dir="rtl">Business Relevance</span>             | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span>    | <span dir="rtl">80/100</span>         |
| <span dir="rtl">Testability</span>                    | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم / قابل استفاده</span>    | <span dir="rtl">95/100</span>         |
| <span dir="rtl">Feasibility Knowledge</span>          | <span dir="rtl">10٪</span>       | <span dir="rtl">داریم اما ناقص</span>          | <span dir="rtl">70/100</span>         |
| <span dir="rtl">Evidence Triangulation</span>         | <span dir="rtl">10٪</span>       | <span dir="rtl">داریم / قابل استفاده</span>    | <span dir="rtl">90/100</span>         |
| <span dir="rtl">Alternative Comparison</span>         | <span dir="rtl">8٪</span>        | <span dir="rtl">داریم / قابل استفاده</span>    | <span dir="rtl">85/100</span>         |
| <span dir="rtl">Behavioral Solution Validation</span> | <span dir="rtl">7٪</span>        | <span dir="rtl">Critical Unknown / ضعیف</span> | <span dir="rtl">20/100</span>         |

<span dir="rtl"></span>

<span dir="rtl">۶. Missing Data: چه چیزی را می‌توانیم و نمی‌توانیم حل کنیم؟</span>

<span dir="rtl">• Fake Door demand</span>

<span dir="rtl">• Completion و recommendation click رفتار واقعی</span>

<span dir="rtl">• Feasibility/data readiness دقیق</span>

<span dir="rtl">• uplift واقعی روی commerce</span>

<span dir="rtl">طبقه‌بندی:</span>

<span dir="rtl">• قابل برآورد: فقط وقتی range یا proxy معتبر داریم و نتیجه نسبت به آن Robust باشد.</span>

<span dir="rtl">• قابل اغماض: داده‌ای که نبودنش تصمیم این فصل را تغییر نمی‌دهد.</span>

<span dir="rtl">• Critical Unknown: داده‌ای که می‌تواند Ranking، Feature Selection یا توصیه Build/Test را عوض کند؛ برای آن عددسازی نمی‌کنیم.</span>

<span dir="rtl">۷. مدل کوانتیفیکیشن اختصاصی فصل</span>

<span dir="rtl">وزن معیارها بین فصل‌ها متفاوت است چون سؤال تصمیمی متفاوت است؛ اما قواعد پایه DECAF، تعریف Confidence، Triangulation، Cap Rule و Double-counting Control ثابت می‌مانند.</span>

| <span dir="rtl">معیار</span>                          | <span dir="rtl">وزن</span> | <span dir="rtl">نمره ۰–۱۰۰</span> | <span dir="rtl">سهم وزنی</span> |
|-------------------------------------------------------|----------------------------|-----------------------------------|---------------------------------|
| <span dir="rtl">Opportunity Fit</span>                | <span dir="rtl">20٪</span> | <span dir="rtl">95</span>         | <span dir="rtl">19.0</span>     |
| <span dir="rtl">User Value</span>                     | <span dir="rtl">15٪</span> | <span dir="rtl">90</span>         | <span dir="rtl">13.5</span>     |
| <span dir="rtl">Business Relevance</span>             | <span dir="rtl">15٪</span> | <span dir="rtl">80</span>         | <span dir="rtl">12.0</span>     |
| <span dir="rtl">Testability</span>                    | <span dir="rtl">15٪</span> | <span dir="rtl">95</span>         | <span dir="rtl">14.2</span>     |
| <span dir="rtl">Feasibility Knowledge</span>          | <span dir="rtl">10٪</span> | <span dir="rtl">70</span>         | <span dir="rtl">7.0</span>      |
| <span dir="rtl">Evidence Triangulation</span>         | <span dir="rtl">10٪</span> | <span dir="rtl">90</span>         | <span dir="rtl">9.0</span>      |
| <span dir="rtl">Alternative Comparison</span>         | <span dir="rtl">8٪</span>  | <span dir="rtl">85</span>         | <span dir="rtl">6.8</span>      |
| <span dir="rtl">Behavioral Solution Validation</span> | <span dir="rtl">7٪</span>  | <span dir="rtl">20</span>         | <span dir="rtl">1.4</span>      |

<span dir="rtl"></span>

<span dir="rtl">امتیاز خام = 83.0 از 100</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">اعمال Cap / Penalty</span></p>
<p><span dir="rtl">Penalty / cap عملی به‌علت نبود Behavioral Solution Validation و Feasibility کامل؛ Selected for Validation، نه Validated.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Confidence نهایی</span></p>
<p><span dir="rtl">72/100 — B — قابل استفاده با Caveat</span></p></th>
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

<span dir="rtl">• بدون Opportunity معتبر، Feature Candidate نمی‌تواند Confidence بالا بگیرد.</span>

<span dir="rtl">• بدون Behavioral solution validation، نتیجه فقط Selected for Validation است.</span>

<span dir="rtl">• AI را Feature ننام؛ AI می‌تواند Mechanism پیاده‌سازی باشد.</span>

<span dir="rtl">• Decision Index ordinal است، نه probability.</span>

<span dir="rtl">۱۱. Sensitivity، Robustness و VOI</span>

<span dir="rtl">Sensitivity می‌پرسد اگر یک ورودی اشتباه باشد، آیا تصمیم عوض می‌شود؟ Robustness می‌پرسد آیا نتیجه با تغییر فرض‌های معقول پابرجا می‌ماند؟ VOI مشخص می‌کند جمع‌آوری کدام داده جدید بیشترین احتمال کاهش عدم‌قطعیت تصمیم را دارد.</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">بالاترین VOI فعلی</span></p>
<p><span dir="rtl">Fake Door با CTA «در ۲ دقیقه محصول مناسبم را پیدا کن» و سپس Concierge/Wizard-of-Oz برای سنجش Start، Completion، Recommendation Click و ATC.</span></p></th>
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

<span dir="rtl">نتیجه Q10: از Opportunity اصلی، چند Solution candidate ساخته و مقایسه شدند. خروجی این مرحله «Guided Beauty Decision Assistant» است؛ اما فقط به‌عنوان Selected for Validation. AI خودِ Feature نیست و implementation نهایی هنوز باز است. امتیاز بالای یک candidate در Decision Index، احتمال موفقیت یا اثبات Market Fit نیست.</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Next Evidence Action</span></p>
<p><span dir="rtl">Fake Door با CTA «در ۲ دقیقه محصول مناسبم را پیدا کن» و سپس Concierge/Wizard-of-Oz برای سنجش Start، Completion، Recommendation Click و ATC.</span></p></th>
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

<span dir="rtl">نسخه: شهریور ۱۴۰۵ \| روش: DECAF Quantification v1.0 \| وضعیت: سند مستقل Q10</span>
