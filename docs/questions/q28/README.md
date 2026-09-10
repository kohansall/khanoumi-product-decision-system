<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q28 | پیش‌بینی درآمد</span></p>
<p><span dir="rtl">Forecast باید از Funnel و Contribution ساخته شود، نه از GMV کل شرکت یا درصدهای دلخواه.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">برای این Feature هنوز درآمد Incremental مشاهده‌شده نداریم. بنابراین Q28 باید مدل قابل پرشدن بسازد و از Fake Precision دوری کند. ورودی‌های کلیدی Eligible Sessions، Adoption، Completion، Baseline Purchase Rate، Incremental Uplift، AOV و Contribution Margin هستند.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• Incremental Orders = Eligible Sessions × Adoption × Completion × Baseline Purchase Rate × Incremental Effect.</span>
>
> <span dir="rtl">• Incremental GMV = Incremental Orders × AOV.</span>
>
> <span dir="rtl">• Incremental Contribution = Incremental Orders × Contribution per Order.</span>
>
> <span dir="rtl">• GMV، Revenue و Contribution سه مفهوم متفاوت‌اند و نباید جای هم استفاده شوند.</span>
>
> <span dir="rtl">• تا قبل از Experiment، Uplift باید Range/Distribution باشد نه یک درصد قطعی.</span>
>
> <span dir="rtl">• در وضعیت فعلی بهتر است Break-even input table ارائه شود تا Revenue forecast جعلی.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>                | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>         | <span dir="rtl">نقش در تصمیم</span>       |
|--------------------------------------------------|----------------------------|--------------------------------------|-------------------------------------------|
| <span dir="rtl">Eligible sessions</span>         | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>        | <span dir="rtl">حجم فرصت</span>           |
| <span dir="rtl">Adoption/CTR</span>              | <span dir="rtl">10٪</span> | <span dir="rtl">نداریم</span>        | <span dir="rtl">ورود به feature</span>    |
| <span dir="rtl">Completion</span>                | <span dir="rtl">10٪</span> | <span dir="rtl">نداریم</span>        | <span dir="rtl">استفاده واقعی</span>      |
| <span dir="rtl">Baseline purchase rate</span>    | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>        | <span dir="rtl">مبنای اثر</span>          |
| <span dir="rtl">Incremental uplift</span>        | <span dir="rtl">20٪</span> | <span dir="rtl">نداریم</span>        | <span dir="rtl">driver اصلی</span>        |
| <span dir="rtl">AOV</span>                       | <span dir="rtl">10٪</span> | <span dir="rtl">context داریم</span> | <span dir="rtl">ارزش سفارش</span>         |
| <span dir="rtl">Contribution margin/order</span> | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>        | <span dir="rtl">ارزش اقتصادی واقعی</span> |
| <span dir="rtl">Seasonality/mix</span>           | <span dir="rtl">5٪</span>  | <span dir="rtl">نسبی</span>          | <span dir="rtl">range forecast</span>     |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>          | <span dir="rtl">وضعیت</span>      | <span dir="rtl">طبقه Missing</span>           | <span dir="rtl">اثر</span>                          |
|--------------------------------------------|-----------------------------------|-----------------------------------------------|-----------------------------------------------------|
| <span dir="rtl">Eligible traffic</span>    | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">driver حجم</span>                   |
| <span dir="rtl">Adoption</span>            | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Estimable با Fake Door</span> | <span dir="rtl">VOI بسیار بالا</span>               |
| <span dir="rtl">Completion</span>          | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Estimable با Concierge</span> | <span dir="rtl">VOI بالا</span>                     |
| <span dir="rtl">Baseline CVR</span>        | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">باید از analytics بیاید</span>      |
| <span dir="rtl">Uplift</span>              | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">نیاز experiment</span>              |
| <span dir="rtl">AOV</span>                 | <span dir="rtl">بخشی موجود</span> | <span dir="rtl">Estimable</span>              | <span dir="rtl">باید cohort-specific شود</span>     |
| <span dir="rtl">Contribution margin</span> | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">GMV را به اقتصاد تبدیل می‌کند</span> |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• Official business report برای scale/context، نه feature uplift.</span>
>
> <span dir="rtl">• Fake Door/Concierge برای adoption و completion.</span>
>
> <span dir="rtl">• A/B یا holdout برای causal uplift؛ بدون آن benchmark فقط prior است.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• بدون Baseline Purchase Rate و Contribution Margin، forecast اقتصادی قطعی حداکثر C است.</span>
>
> <span dir="rtl">• Uplift بدون experiment باید Range باشد.</span>
>
> <span dir="rtl">• GMV به‌تنهایی Revenue/Profit نیست.</span>
>
> <span dir="rtl">• Q28 نباید با اعداد قدیمی 5.44B/816M ادامه یابد؛ آن سناریو superseded است.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>               | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>       | <span dir="rtl">دلیل</span>                         |
|--------------------------------------------|------------------------------------|----------------------------------|-----------------------------------------------------|
| <span dir="rtl">Incremental uplift</span>  | <span dir="rtl">Very High</span>   | <span dir="rtl">Very High</span> | <span dir="rtl">driver اصلی forecast</span>         |
| <span dir="rtl">Eligible sessions</span>   | <span dir="rtl">High</span>        | <span dir="rtl">High</span>      | <span dir="rtl">حجم فرصت</span>                     |
| <span dir="rtl">Contribution margin</span> | <span dir="rtl">High</span>        | <span dir="rtl">Very High</span> | <span dir="rtl">اقتصاد واقعی</span>                 |
| <span dir="rtl">Adoption</span>            | <span dir="rtl">High</span>        | <span dir="rtl">Very High</span> | <span dir="rtl">Fake Door سریع اندازه می‌گیرد</span> |
| <span dir="rtl">AOV</span>                 | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span>    | <span dir="rtl">اثر خطی</span>                      |

> <span dir="rtl">• بالاترین VOI: Adoption و Uplift؛ Fake Door + controlled pilot می‌توانند این دو را اندازه بگیرند.</span>
>
> <span dir="rtl">• Contribution Margin باید از Finance گرفته شود؛ بدون آن تصمیم سرمایه‌گذاری ناقص است.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                         | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|------------------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Model Structure</span>               | <span dir="rtl">20٪</span> | <span dir="rtl">95</span>     | <span dir="rtl">19.0</span>     |
| <span dir="rtl">Traffic Evidence</span>              | <span dir="rtl">15٪</span> | <span dir="rtl">20</span>     | <span dir="rtl">3.0</span>      |
| <span dir="rtl">Adoption/Completion Evidence</span>  | <span dir="rtl">15٪</span> | <span dir="rtl">20</span>     | <span dir="rtl">3.0</span>      |
| <span dir="rtl">Baseline CVR Evidence</span>         | <span dir="rtl">15٪</span> | <span dir="rtl">20</span>     | <span dir="rtl">3.0</span>      |
| <span dir="rtl">Uplift Evidence</span>               | <span dir="rtl">20٪</span> | <span dir="rtl">10</span>     | <span dir="rtl">2.0</span>      |
| <span dir="rtl">Economics/AOV/Margin Evidence</span> | <span dir="rtl">15٪</span> | <span dir="rtl">35</span>     | <span dir="rtl">5.2</span>      |

| <span dir="rtl">Confidence نهایی: 49/100 — کلاس C :: مدل محاسباتی روشن است اما تقریباً تمام driverهای feature-specific هنوز اندازه‌گیری نشده‌اند؛ بنابراین Forecast عددی فعلاً باید Scenario/TBD بماند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">فرمول و اینکه uplift، eligible traffic و margin driverهای اصلی‌اند Robust است؛ هر عدد درآمد فعلی به‌شدت به فرض‌ها حساس است و Robust نیست.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: ابتدا Fake Door برای adoption/completion، سپس pilot controlled برای uplift؛ هم‌زمان Finance باید contribution margin/order و cohort AOV را تأمین کند.</span> |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
