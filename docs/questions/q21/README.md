<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q21 | تعریف KPIها</span></p>
<p><span dir="rtl">آیا KPIها واقعاً Outcome را اندازه می‌گیرند و تعریف عملیاتی قابل اندازه‌گیری دارند؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">در این فصل، معیارها از Vanity Metrics جدا می‌شوند. برای دستیار انتخاب محصول، هدف فقط کلیک روی Feature نیست؛ باید از Exposure تا Purchase یک Funnel قابل ردیابی داشته باشیم و در نهایت اثر روی تصمیم خرید را بسنجیم.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• Primary outcome candidate: Purchase Conversion در کاربران Eligible/Exposed با مقایسه مناسب.</span>
>
> <span dir="rtl">• Diagnostic funnel: Exposure → CTA Click → Start → Completion → Recommendation Click → Add to Cart → Purchase.</span>
>
> <span dir="rtl">• Quality signals: Recommendation acceptance، External comparison proxy، feedback usefulness.</span>
>
> <span dir="rtl">• هر KPI باید numerator، denominator، event definition و time window داشته باشد.</span>
>
> <span dir="rtl">• Target عددی تا وقتی baseline یا experiment نداریم باید TBD / Hypothesis بماند.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>                    | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>            | <span dir="rtl">نقش در تصمیم</span>             |
|------------------------------------------------------|----------------------------|-----------------------------------------|-------------------------------------------------|
| <span dir="rtl">Primary outcome</span>               | <span dir="rtl">20٪</span> | <span dir="rtl">داریم</span>            | <span dir="rtl">تشخیص Outcome</span>            |
| <span dir="rtl">Funnel metrics</span>                | <span dir="rtl">20٪</span> | <span dir="rtl">داریم</span>            | <span dir="rtl">تشخیص نقطه شکست</span>          |
| <span dir="rtl">Event taxonomy</span>                | <span dir="rtl">15٪</span> | <span dir="rtl">تا حد زیادی</span>      | <span dir="rtl">قابلیت instrumentation</span>   |
| <span dir="rtl">Baseline</span>                      | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>           | <span dir="rtl">هدف‌گذاری و uplift</span>        |
| <span dir="rtl">Time windows</span>                  | <span dir="rtl">10٪</span> | <span dir="rtl">داریم/قابل تعریف</span> | <span dir="rtl">قابل مقایسه شدن</span>          |
| <span dir="rtl">Segment eligibility</span>           | <span dir="rtl">10٪</span> | <span dir="rtl">داریم</span>            | <span dir="rtl">denominator درست</span>         |
| <span dir="rtl">Attribution/experiment design</span> | <span dir="rtl">10٪</span> | <span dir="rtl">نسبی</span>             | <span dir="rtl">نسبت دادن اثر به Feature</span> |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>             | <span dir="rtl">وضعیت</span>   | <span dir="rtl">طبقه Missing</span>     | <span dir="rtl">اثر</span>                     |
|-----------------------------------------------|--------------------------------|-----------------------------------------|------------------------------------------------|
| <span dir="rtl">Funnel definitions</span>     | <span dir="rtl">موجود</span>   | <span dir="rtl">—</span>                | <span dir="rtl">قوی</span>                     |
| <span dir="rtl">Baseline purchase rate</span> | <span dir="rtl">ناموجود</span> | <span dir="rtl">Critical Unknown</span> | <span dir="rtl">برای Target و Uplift</span>    |
| <span dir="rtl">Event implementation</span>   | <span dir="rtl">نامعلوم</span> | <span dir="rtl">Estimable</span>        | <span dir="rtl">نیاز به Analytics audit</span> |
| <span dir="rtl">Exact target</span>           | <span dir="rtl">ناموجود</span> | <span dir="rtl">Ignorable فعلاً</span>   | <span dir="rtl">TBD تا baseline</span>         |
| <span dir="rtl">Experiment attribution</span> | <span dir="rtl">نسبی</span>    | <span dir="rtl">Estimable</span>        | <span dir="rtl">با Holdout/A-B</span>          |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• مسئله Decision Confidence از پژوهش کاربر، Funnel مناسب را تعیین می‌کند.</span>
>
> <span dir="rtl">• MVP flow از Q15–Q16 eventها را مشخص می‌کند.</span>
>
> <span dir="rtl">• داده رسمی کسب‌وکار جهت Outcome را می‌دهد، اما baseline feature-specific موجود نیست.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• KPI بدون numerator/denominator/window ناقص است.</span>
>
> <span dir="rtl">• Target عددی بدون baseline باید Hypothesis/TBD باشد.</span>
>
> <span dir="rtl">• CTR به‌تنهایی Success Metric نهایی نیست و اگر به‌جای Outcome استفاده شود حداکثر Confidence = 59.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>                  | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>    | <span dir="rtl">دلیل</span>                            |
|-----------------------------------------------|------------------------------------|-------------------------------|--------------------------------------------------------|
| <span dir="rtl">Baseline CVR</span>           | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">روی target و uplift اثر مستقیم</span>  |
| <span dir="rtl">Eligibility definition</span> | <span dir="rtl">High</span>        | <span dir="rtl">Medium</span> | <span dir="rtl">denominator را تغییر می‌دهد</span>      |
| <span dir="rtl">Event implementation</span>   | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">اندازه‌گیری را ممکن/ناممکن می‌کند</span> |
| <span dir="rtl">Exact target</span>           | <span dir="rtl">Medium</span>      | <span dir="rtl">High</span>   | <span dir="rtl">بعد از baseline ارزشمند می‌شود</span>   |

> <span dir="rtl">• اول Event Taxonomy و baseline funnel را اندازه بگیریم.</span>
>
> <span dir="rtl">• سپس با A/B یا holdout، Incremental impact را از رفتار طبیعی جدا کنیم.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                        | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|-----------------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Outcome Alignment</span>            | <span dir="rtl">25٪</span> | <span dir="rtl">94</span>     | <span dir="rtl">23.5</span>     |
| <span dir="rtl">Metric Definition Quality</span>    | <span dir="rtl">20٪</span> | <span dir="rtl">92</span>     | <span dir="rtl">18.4</span>     |
| <span dir="rtl">Funnel Coverage</span>              | <span dir="rtl">20٪</span> | <span dir="rtl">94</span>     | <span dir="rtl">18.8</span>     |
| <span dir="rtl">Baseline Evidence</span>            | <span dir="rtl">15٪</span> | <span dir="rtl">35</span>     | <span dir="rtl">5.2</span>      |
| <span dir="rtl">Attribution Readiness</span>        | <span dir="rtl">10٪</span> | <span dir="rtl">72</span>     | <span dir="rtl">7.2</span>      |
| <span dir="rtl">Guard against Vanity Metrics</span> | <span dir="rtl">10٪</span> | <span dir="rtl">95</span>     | <span dir="rtl">9.5</span>      |

| <span dir="rtl">Confidence نهایی: 86/100 — کلاس A :: ساختار KPI و Funnel روشن و Outcome-oriented است؛ نبود baseline مانع تعریف KPI نیست، اما مانع تعیین Target قطعی است.</span> |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">حتی اگر Feature نهایی یا UX تغییر کند، نیاز به سنجش Exposure → Engagement → Commerce Outcome پابرجاست. بخش کم‌ثبات، Targetهای عددی و uplift مورد انتظار است.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: Event dictionary نهایی شود و از داده داخلی، baseline برای Eligible Sessions، PDP→ATC و ATC→Purchase استخراج شود؛ سپس Targetها تعریف شوند.</span> |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

# <span dir="rtl">راهنمای تفسیر نمره</span>

| <span dir="rtl">کلاس</span> | <span dir="rtl">بازه</span>   | <span dir="rtl">معنا</span>                                                                                |
|-----------------------------|-------------------------------|------------------------------------------------------------------------------------------------------------|
| <span dir="rtl">A</span>    | <span dir="rtl">80–100</span> | <span dir="rtl">قابل پذیرش و دفاع؛ عدم‌قطعیت باقی‌مانده معمولاً تصمیم را برنمی‌گرداند.</span>                  |
| <span dir="rtl">B</span>    | <span dir="rtl">60–79</span>  | <span dir="rtl">قابل استفاده با Caveat؛ چند داده مهم هنوز می‌تواند جزئیات یا شدت تصمیم را تغییر دهد.</span> |
| <span dir="rtl">C</span>    | <span dir="rtl">30–59</span>  | <span dir="rtl">فرضیه/استنتاج؛ برای تصمیم قطعی نیاز به Validation یا داده جدید دارد.</span>                |
| <span dir="rtl">D</span>    | <span dir="rtl">0–29</span>   | <span dir="rtl">فاقد ارزش آماری یا معنایی برای تصمیم قطعی.</span>                                          |

## <span dir="rtl">مرز ادعا</span>

<span dir="rtl">Fact = داده مستقیم یا منبع رسمی. Evidence = مشاهده‌ای که یک Claim را پشتیبانی می‌کند. Logical Inference = نتیجه منطقی اما غیرمستقیم. Hypothesis = ادعایی که هنوز باید آزمون شود. در ارائه نهایی این چهار وضعیت نباید با هم مخلوط شوند.</span>

## <span dir="rtl">Source Registry</span>

> <span dir="rtl">• پروژه رسمی بوتکمپ همراه اول — ۱۲ گام و ۳۰ سؤال اتمی</span>
>
> <span dir="rtl">• Evidence و Decision Log پروژه خانومی در Confluence</span>
>
> <span dir="rtl">• Survey Current Buyers و Never/Lapsed — convenience samples با محدودیت تعمیم</span>
>
> <span dir="rtl">• VOC cleaned dataset و UX expert review</span>
>
> <span dir="rtl">• گزارش‌های رسمی خانومی و گزارش‌های مدیریتی با تفکیک تعریف و دوره زمانی</span>
>
> <span dir="rtl">• How to Measure Anything — uncertainty / VOI / range thinking</span>
>
> <span dir="rtl">• Escaping the Build Trap — outcome-oriented roadmap و validation before scale</span>
