<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q26 | برنامه Retention</span></p>
<p><span dir="rtl">آیا Feature می‌تواند ارزش تکرارشونده بسازد و آیا ادعای retention قابل اندازه‌گیری است؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">دستیار انتخاب محصول ذاتاً یک Feature تک‌جلسه‌ای نیست اگر به چرخه مصرف و تصمیم‌های بعدی وصل شود. شواهد فعلی نشان می‌دهد reminder و repurchase need وجود دارد، اما هنوز cohort baseline feature-specific نداریم؛ پس retention strategy را می‌توان طراحی کرد ولی uplift retention را نه.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• Mechanismهای محتمل: saved profile/preferences، repurchase reminder، routine continuity، next-best recommendation.</span>
>
> <span dir="rtl">• در نمونه Current Buyers، بخش قابل توجهی برای تمام‌شدن محصول reminder می‌خواستند؛ این Evidence توصیفی است، نه prevalence کل کاربران.</span>
>
> <span dir="rtl">• گزارش رسمی return/retention context داریم، ولی تعاریف مختلف مدیریتی را نباید مستقیم با هم مقایسه کرد.</span>
>
> <span dir="rtl">• Primary retention view باید cohort-based و با window روشن باشد.</span>
>
> <span dir="rtl">• Feature retention uplift فقط با holdout/cohort بعد از launch قابل ادعاست.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>                | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>       | <span dir="rtl">نقش در تصمیم</span>        |
|--------------------------------------------------|----------------------------|------------------------------------|--------------------------------------------|
| <span dir="rtl">Repurchase behavior</span>       | <span dir="rtl">18٪</span> | <span dir="rtl">داریم</span>       | <span dir="rtl">وجود job تکرارشونده</span> |
| <span dir="rtl">Usage cycle</span>               | <span dir="rtl">12٪</span> | <span dir="rtl">نسبی</span>        | <span dir="rtl">زمان trigger</span>        |
| <span dir="rtl">Cohort baseline</span>           | <span dir="rtl">18٪</span> | <span dir="rtl">نداریم</span>      | <span dir="rtl">اندازه اثر</span>          |
| <span dir="rtl">Trigger acceptance</span>        | <span dir="rtl">12٪</span> | <span dir="rtl">بخشی داریم</span>  | <span dir="rtl">طراحی reminder</span>      |
| <span dir="rtl">Recurring value mechanism</span> | <span dir="rtl">15٪</span> | <span dir="rtl">داریم/فرضیه</span> | <span dir="rtl">چرایی بازگشت</span>        |
| <span dir="rtl">Segment differences</span>       | <span dir="rtl">10٪</span> | <span dir="rtl">نسبی</span>        | <span dir="rtl">عدم تعمیم</span>           |
| <span dir="rtl">Measurement window</span>        | <span dir="rtl">10٪</span> | <span dir="rtl">قابل تعریف</span>  | <span dir="rtl">retention metric</span>    |
| <span dir="rtl">Incremental uplift</span>        | <span dir="rtl">5٪</span>  | <span dir="rtl">نداریم</span>      | <span dir="rtl">نیاز experiment</span>     |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>                       | <span dir="rtl">وضعیت</span>      | <span dir="rtl">طبقه Missing</span>     | <span dir="rtl">اثر</span>                  |
|---------------------------------------------------------|-----------------------------------|-----------------------------------------|---------------------------------------------|
| <span dir="rtl">Repurchase need</span>                  | <span dir="rtl">موجود</span>      | <span dir="rtl">—</span>                | <span dir="rtl">شواهد توصیفی</span>         |
| <span dir="rtl">Product depletion cycle</span>          | <span dir="rtl">نسبی</span>       | <span dir="rtl">Estimable</span>        | <span dir="rtl">برحسب category</span>       |
| <span dir="rtl">Cohort baseline feature-specific</span> | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span> | <span dir="rtl">برای target</span>          |
| <span dir="rtl">Reminder acceptance</span>              | <span dir="rtl">بخشی موجود</span> | <span dir="rtl">Estimable</span>        | <span dir="rtl">نیاز behavioral test</span> |
| <span dir="rtl">Incremental retention uplift</span>     | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span> | <span dir="rtl">بعد experiment</span>       |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• Current Buyer survey برای reminder/repurchase behavior.</span>
>
> <span dir="rtl">• Official business reporting برای بازگشت مشتری به‌عنوان context.</span>
>
> <span dir="rtl">• Management reports برای retention priorities با caveat تعریف و دوره زمانی.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• بدون cohort baseline، target retention قطعی ممنوع.</span>
>
> <span dir="rtl">• Self-report و official metric با definition متفاوت نباید مستقیم merge شوند.</span>
>
> <span dir="rtl">• Intent to use reminder به معنی retention uplift نیست.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>                | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>    | <span dir="rtl">دلیل</span>                 |
|---------------------------------------------|------------------------------------|-------------------------------|---------------------------------------------|
| <span dir="rtl">Cohort baseline</span>      | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">target و effect size</span> |
| <span dir="rtl">Consumption cycle</span>    | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">زمان trigger</span>         |
| <span dir="rtl">Reminder acceptance</span>  | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span> | <span dir="rtl">mechanism viability</span>  |
| <span dir="rtl">Segment/category mix</span> | <span dir="rtl">Medium</span>      | <span dir="rtl">High</span>   | <span dir="rtl">تکرارپذیری نیاز</span>      |

> <span dir="rtl">• بیشترین VOI: depletion cycle و cohort baseline در categoryهای پرتکرار.</span>
>
> <span dir="rtl">• یک pilot reminder ساده می‌تواند قبل از ساخت profile پیچیده، اثر روی revisit/repurchase را بسنجد.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                   | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|------------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Repurchase Evidence</span>     | <span dir="rtl">20٪</span> | <span dir="rtl">80</span>     | <span dir="rtl">16.0</span>     |
| <span dir="rtl">Recurring Mechanism Fit</span> | <span dir="rtl">20٪</span> | <span dir="rtl">82</span>     | <span dir="rtl">16.4</span>     |
| <span dir="rtl">Cohort Baseline</span>         | <span dir="rtl">20٪</span> | <span dir="rtl">30</span>     | <span dir="rtl">6.0</span>      |
| <span dir="rtl">Trigger Evidence</span>        | <span dir="rtl">15٪</span> | <span dir="rtl">60</span>     | <span dir="rtl">9.0</span>      |
| <span dir="rtl">Measurement Design</span>      | <span dir="rtl">15٪</span> | <span dir="rtl">78</span>     | <span dir="rtl">11.7</span>     |
| <span dir="rtl">Incremental Causality</span>   | <span dir="rtl">10٪</span> | <span dir="rtl">20</span>     | <span dir="rtl">2.0</span>      |

| <span dir="rtl">Confidence نهایی: 66/100 — کلاس B :: Job تکرارشونده و چند mechanism معقول داریم، اما هنوز رابطه علّی بین Feature و retention و baseline cohort روشن نیست.</span> |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">اصل وجود فرصت retention در چرخه مصرف beauty نسبتاً پایدار است؛ ادعای اینکه Guided Assistant واقعاً retention را بالا می‌برد هنوز شکننده و نیازمند آزمون است.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: برای 2–3 category با چرخه تکرار روشن، cohort repurchase baseline و median reorder interval استخراج شود؛ سپس reminder pilot با holdout اجرا شود.</span> |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
