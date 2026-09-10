<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q27 | مدل هزینه</span></p>
<p><span dir="rtl">هزینه را از Scope و Effort بسنجیم؛ نه با یک عدد کلِ بدون زنجیره محاسبه.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">نسخه قبلی برآورد ۴۰۰–۸۰۰ میلیون تومان مبنای کافی نداشت و کنار گذاشته می‌شود. مدل درست از Scope شروع می‌کند، هر Component را به Role و Effort می‌شکند، Rate را از benchmark یا هزینه واقعی تیم می‌گیرد و فقط هزینه‌های incremental و causal را جمع می‌کند.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• Stage A — Fake Door: Design + Front/Experiment + Analytics + Ops محدود.</span>
>
> <span dir="rtl">• Stage B — Concierge/Wizard-of-Oz: عملیات دستی + script + data capture.</span>
>
> <span dir="rtl">• Stage C — Rule-based MVP: Product/Design/Front/Back/Data/QA + instrumentation.</span>
>
> <span dir="rtl">• Stage D — Production Scale: infra، governance، automation و operations؛ فعلاً خارج از MVP commitment.</span>
>
> <span dir="rtl">• Benchmark حقوق بازار فقط Anchor است؛ هزینه واقعی خانومی باید از payroll/loaded cost یا نرخ قراردادی تیم بیاید.</span>
>
> <span dir="rtl">• Total Cost = Σ(Role × Allocation × Duration × Loaded Rate) + Infra/Vendor + Operations + Contingency.</span>

| <span dir="rtl">اصلاح مهم :: برآورد قبلی ۴۰۰–۸۰۰ میلیون و Base = ۵۰۰ میلیون به‌دلیل نبود زنجیره Effort × Rate کنار گذاشته شده است. این سند آن اعداد را معتبر نمی‌داند.</span> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Benchmark حقوق — فقط برای Anchor</span>

| <span dir="rtl">Benchmark ۱۴۰۵</span>                                  | <span dir="rtl">عدد گزارش‌شده</span>                      | <span dir="rtl">نحوه استفاده</span>                        |
|------------------------------------------------------------------------|----------------------------------------------------------|------------------------------------------------------------|
| <span dir="rtl">Median سطح کارشناس</span>                              | <span dir="rtl">۳۵ میلیون تومان/ماه</span>               | <span dir="rtl">Anchor عمومی بازار، نه هزینه خانومی</span> |
| <span dir="rtl">Median سطح مدیر</span>                                 | <span dir="rtl">۶۵ میلیون تومان/ماه</span>               | <span dir="rtl">Anchor عمومی بازار</span>                  |
| <span dir="rtl">تهران — IT/Software/Infrastructure، سطح کارشناس</span> | <span dir="rtl">حدود ۴۵ میلیون تومان «حقوق نرمال»</span> | <span dir="rtl">برای cross-check role rate</span>          |
| <span dir="rtl">تهران — R&D/Product/Innovation، سطح کارشناس</span>     | <span dir="rtl">حدود ۳۷ میلیون تومان «حقوق نرمال»</span> | <span dir="rtl">برای Product/Data roles</span>             |
| <span dir="rtl">تهران — UX، سطح کارشناس</span>                         | <span dir="rtl">حدود ۳۵ میلیون تومان «حقوق نرمال»</span> | <span dir="rtl">برای Design benchmark</span>               |

<span dir="rtl">منبع: گزارش حقوق و دستمزد ایران‌تلنت ۱۴۰۵. این اعداد حقوق دریافتی/بازاری‌اند و معادل Loaded Employer Cost نیستند. برای برآورد نهایی باید هزینه واقعی تیم خانومی یا نرخ پیمانکار جایگزین شود.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>             | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>           | <span dir="rtl">نقش در تصمیم</span>        |
|-----------------------------------------------|----------------------------|----------------------------------------|--------------------------------------------|
| <span dir="rtl">Scope/components</span>       | <span dir="rtl">15٪</span> | <span dir="rtl">داریم</span>           | <span dir="rtl">چه چیزی هزینه می‌شود</span> |
| <span dir="rtl">Role map</span>               | <span dir="rtl">15٪</span> | <span dir="rtl">قابل تعریف</span>      | <span dir="rtl">چه کسی لازم است</span>     |
| <span dir="rtl">Allocation</span>             | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>          | <span dir="rtl">درصد درگیری</span>         |
| <span dir="rtl">Duration/effort</span>        | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>          | <span dir="rtl">person-month/day</span>    |
| <span dir="rtl">Actual/benchmark rates</span> | <span dir="rtl">15٪</span> | <span dir="rtl">benchmark داریم</span> | <span dir="rtl">قیمت هر effort</span>      |
| <span dir="rtl">Infra/vendor</span>           | <span dir="rtl">8٪</span>  | <span dir="rtl">نامعلوم</span>         | <span dir="rtl">هزینه خارجی</span>         |
| <span dir="rtl">Ops/manual concierge</span>   | <span dir="rtl">7٪</span>  | <span dir="rtl">نامعلوم</span>         | <span dir="rtl">MVP human cost</span>      |
| <span dir="rtl">Contingency</span>            | <span dir="rtl">5٪</span>  | <span dir="rtl">قابل تعریف</span>      | <span dir="rtl">عدم‌قطعیت</span>            |
| <span dir="rtl">Loaded-cost rule</span>       | <span dir="rtl">5٪</span>  | <span dir="rtl">نامعلوم</span>         | <span dir="rtl">مزایا/سربار causal</span>  |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>                  | <span dir="rtl">وضعیت</span>       | <span dir="rtl">طبقه Missing</span>         | <span dir="rtl">اثر</span>                           |
|----------------------------------------------------|------------------------------------|---------------------------------------------|------------------------------------------------------|
| <span dir="rtl">MVP scope</span>                   | <span dir="rtl">موجود</span>       | <span dir="rtl">—</span>                    | <span dir="rtl">قوی</span>                           |
| <span dir="rtl">Role list</span>                   | <span dir="rtl">قابل برآورد</span> | <span dir="rtl">Estimable</span>            | <span dir="rtl">با tech/design review</span>         |
| <span dir="rtl">Allocation/effort</span>           | <span dir="rtl">ناموجود</span>     | <span dir="rtl">Critical Unknown</span>     | <span dir="rtl">driver اصلی cost</span>              |
| <span dir="rtl">Salary market benchmark</span>     | <span dir="rtl">موجود</span>       | <span dir="rtl">—</span>                    | <span dir="rtl">فقط Anchor</span>                    |
| <span dir="rtl">Khanoumi actual loaded rate</span> | <span dir="rtl">ناموجود</span>     | <span dir="rtl">Critical Unknown</span>     | <span dir="rtl">driver اصلی</span>                   |
| <span dir="rtl">Infra/API</span>                   | <span dir="rtl">نامعلوم</span>     | <span dir="rtl">Estimable</span>            | <span dir="rtl">برای rule-based احتمالاً محدود</span> |
| <span dir="rtl">Shared overhead</span>             | <span dir="rtl">ناموجود</span>     | <span dir="rtl">Ignorable مگر causal</span> | <span dir="rtl">نباید تخصیص مصنوعی</span>            |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• Q15–Q17 برای Scope و stage gate.</span>
>
> <span dir="rtl">• گزارش IranTalent 1405 برای benchmark بازار حقوق؛ نه هزینه واقعی خانومی.</span>
>
> <span dir="rtl">• JobVision 1404 می‌تواند cross-check benchmark باشد، ولی actual payroll بر هر دو مقدم است.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• بدون زنجیره Role → Effort → Rate، عدد کل هزینه «فاقد دفاع» است.</span>
>
> <span dir="rtl">• یک عدد نقطه‌ای برای ورودی‌های نامطمئن ممنوع؛ Range/Scenario لازم است.</span>
>
> <span dir="rtl">• Benchmark salary نباید به‌عنوان loaded employer cost خانومی جا زده شود.</span>
>
> <span dir="rtl">• Shared corporate overhead فقط وقتی وارد می‌شود که incremental و causal باشد.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>               | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>       | <span dir="rtl">دلیل</span>                                 |
|--------------------------------------------|------------------------------------|----------------------------------|-------------------------------------------------------------|
| <span dir="rtl">Effort/person-month</span> | <span dir="rtl">Very High</span>   | <span dir="rtl">Very High</span> | <span dir="rtl">بزرگ‌ترین driver</span>                      |
| <span dir="rtl">Loaded rate</span>         | <span dir="rtl">High</span>        | <span dir="rtl">High</span>      | <span dir="rtl">هزینه مستقیم</span>                         |
| <span dir="rtl">Scope stage</span>         | <span dir="rtl">Very High</span>   | <span dir="rtl">High</span>      | <span dir="rtl">Fake Door با production کاملاً متفاوت</span> |
| <span dir="rtl">Infra/vendor</span>        | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span>    | <span dir="rtl">در MVP ممکن است کوچک باشد</span>            |
| <span dir="rtl">Contingency</span>         | <span dir="rtl">Low/Medium</span>  | <span dir="rtl">Low</span>       | <span dir="rtl">به uncertainty buffer کمک می‌کند</span>      |

> <span dir="rtl">• بالاترین VOI: engineering/design/data effort estimate و actual loaded rate.</span>
>
> <span dir="rtl">• قبل از هر عدد نهایی، یک ۳۰ دقیقه estimation workshop می‌تواند uncertainty را شدیداً کم کند.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                      | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|---------------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Scope Clarity</span>              | <span dir="rtl">20٪</span> | <span dir="rtl">90</span>     | <span dir="rtl">18.0</span>     |
| <span dir="rtl">Role Mapping</span>               | <span dir="rtl">15٪</span> | <span dir="rtl">75</span>     | <span dir="rtl">11.2</span>     |
| <span dir="rtl">Effort Evidence</span>            | <span dir="rtl">20٪</span> | <span dir="rtl">25</span>     | <span dir="rtl">5.0</span>      |
| <span dir="rtl">Rate Evidence</span>              | <span dir="rtl">20٪</span> | <span dir="rtl">55</span>     | <span dir="rtl">11.0</span>     |
| <span dir="rtl">External/Operational Costs</span> | <span dir="rtl">10٪</span> | <span dir="rtl">35</span>     | <span dir="rtl">3.5</span>      |
| <span dir="rtl">Uncertainty Treatment</span>      | <span dir="rtl">15٪</span> | <span dir="rtl">92</span>     | <span dir="rtl">13.8</span>     |

| <span dir="rtl">Confidence نهایی: 58/100 — کلاس C :: فرمول و Scope اکنون علمی و قابل دفاع‌اند، ولی دو driver اصلی یعنی Effort و Actual Loaded Rate هنوز در دسترس نیستند؛ بنابراین عدد هزینه نهایی ساخته نمی‌شود.</span> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">اینکه Fake Door ارزان‌تر از Rule-based و Production است Robust است؛ اما اندازه ریالی فاصله بین Stageها بدون effort/rate واقعی Robust نیست.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: برای Stage A تا C، RACI و person-day estimate از تیم بگیریم؛ سپس actual loaded monthly cost یا نرخ پیمانکار را جایگزین benchmark کنیم و Low/Base/High بسازیم.</span> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
>
> <span dir="rtl">• IranTalent Salary Report 1405 — market salary benchmark؛ نه payroll خانومی</span>
