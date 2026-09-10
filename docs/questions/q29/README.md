<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q29 | ROI و Payback</span></p>
<p><span dir="rtl">ROI فقط وقتی معنا دارد که هزینه و Contribution هر دو با عدم‌قطعیت خودشان وارد مدل شوند.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">Q29 خروجی ترکیبی Q27 و Q28 است. چون Cost و Incremental Contribution هنوز driverهای بحرانی نامشخص دارند، دادن ROI یا Payback تک‌عددی علمی نیست. خروجی فعلی باید Break-even Analysis و فرمول‌های Scenario باشد و Confidence آن نمی‌تواند از ضعیف‌ترین ورودی‌های upstream بالاتر برود.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• ROI = (Cumulative Incremental Contribution − Total Incremental Cost) ÷ Total Incremental Cost.</span>
>
> <span dir="rtl">• Payback = اولین دوره‌ای که Contribution تجمعی هزینه Incremental را پوشش می‌دهد.</span>
>
> <span dir="rtl">• Break-even Orders = Total Cost ÷ Contribution per Incremental Order.</span>
>
> <span dir="rtl">• Break-even Spend مهم است: حداکثر هزینه قابل قبول برای یک سطح Benefit مشخص.</span>
>
> <span dir="rtl">• اگر ورودی‌ها Range باشند، خروجی هم باید Range/Distribution باشد.</span>
>
> <span dir="rtl">• مدل قبلی ROI +63٪ و Payback 7.3 ماه به‌دلیل Cost/Revenue فرضی superseded است.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>                  | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>      | <span dir="rtl">نقش در تصمیم</span>             |
|----------------------------------------------------|----------------------------|-----------------------------------|-------------------------------------------------|
| <span dir="rtl">Total incremental cost</span>      | <span dir="rtl">25٪</span> | <span dir="rtl">ناقص</span>       | <span dir="rtl">از Q27</span>                   |
| <span dir="rtl">Incremental contribution</span>    | <span dir="rtl">30٪</span> | <span dir="rtl">ناقص</span>       | <span dir="rtl">از Q28</span>                   |
| <span dir="rtl">Timing/cash flow</span>            | <span dir="rtl">10٪</span> | <span dir="rtl">نداریم</span>     | <span dir="rtl">payback</span>                  |
| <span dir="rtl">Uncertainty ranges</span>          | <span dir="rtl">10٪</span> | <span dir="rtl">روش داریم</span>  | <span dir="rtl">انتقال عدم قطعیت</span>         |
| <span dir="rtl">Break-even logic</span>            | <span dir="rtl">10٪</span> | <span dir="rtl">داریم</span>      | <span dir="rtl">تصمیم بدون forecast کامل</span> |
| <span dir="rtl">Decision horizon</span>            | <span dir="rtl">5٪</span>  | <span dir="rtl">قابل تعریف</span> | <span dir="rtl">window</span>                   |
| <span dir="rtl">Risk/discounting</span>            | <span dir="rtl">5٪</span>  | <span dir="rtl">بعداً</span>       | <span dir="rtl">برای horizon بلند</span>        |
| <span dir="rtl">Scenario/Monte Carlo inputs</span> | <span dir="rtl">5٪</span>  | <span dir="rtl">ناقص</span>       | <span dir="rtl">پس از calibration</span>        |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>          | <span dir="rtl">وضعیت</span>   | <span dir="rtl">طبقه Missing</span>         | <span dir="rtl">اثر</span>                      |
|--------------------------------------------|--------------------------------|---------------------------------------------|-------------------------------------------------|
| <span dir="rtl">Cost</span>                | <span dir="rtl">ناقص</span>    | <span dir="rtl">Critical Unknown</span>     | <span dir="rtl">Q27=58</span>                   |
| <span dir="rtl">Contribution</span>        | <span dir="rtl">ناقص</span>    | <span dir="rtl">Critical Unknown</span>     | <span dir="rtl">Q28=49</span>                   |
| <span dir="rtl">Timing</span>              | <span dir="rtl">ناموجود</span> | <span dir="rtl">Estimable</span>            | <span dir="rtl">بعد roadmap/pilot</span>        |
| <span dir="rtl">Break-even formula</span>  | <span dir="rtl">موجود</span>   | <span dir="rtl">—</span>                    | <span dir="rtl">قوی</span>                      |
| <span dir="rtl">Input distributions</span> | <span dir="rtl">ناموجود</span> | <span dir="rtl">Estimable after data</span> | <span dir="rtl">Monte Carlo فعلاً زود است</span> |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• Upstream Q27 cost evidence.</span>
>
> <span dir="rtl">• Upstream Q28 revenue/contribution evidence.</span>
>
> <span dir="rtl">• Hubbard/AIE برای ranges، VOI و uncertainty propagation به‌عنوان روش، نه source عدد خانومی.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• Confidence Q29 از کیفیت Q27 و Q28 بالاتر نمی‌رود.</span>
>
> <span dir="rtl">• ROI تک‌عددی با input range ممنوع.</span>
>
> <span dir="rtl">• Monte Carlo با distributionهای دلخواه precision مصنوعی است.</span>
>
> <span dir="rtl">• اگر Contribution Margin در دسترس نباشد، GMV-based ROI معتبر نیست.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>                    | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>       | <span dir="rtl">دلیل</span>               |
|-------------------------------------------------|------------------------------------|----------------------------------|-------------------------------------------|
| <span dir="rtl">Incremental contribution</span> | <span dir="rtl">Very High</span>   | <span dir="rtl">Very High</span> | <span dir="rtl">صورت ROI و payback</span> |
| <span dir="rtl">Total cost</span>               | <span dir="rtl">Very High</span>   | <span dir="rtl">Very High</span> | <span dir="rtl">مخرج و break-even</span>  |
| <span dir="rtl">Timing</span>                   | <span dir="rtl">High</span>        | <span dir="rtl">Medium</span>    | <span dir="rtl">payback/cash flow</span>  |
| <span dir="rtl">Distribution choice</span>      | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span>    | <span dir="rtl">Monte Carlo shape</span>  |

> <span dir="rtl">• بالاترین VOI همان داده‌های Q27/Q28 است؛ اندازه‌گیری جداگانه جدیدی قبل از آن ارزش کمتری دارد.</span>
>
> <span dir="rtl">• Break-even analysis می‌تواند حتی قبل از Forecast کامل به Finance بگوید چه سطح uplift یا contribution برای توجیه هزینه لازم است.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                 | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|----------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Formula/Logic</span>         | <span dir="rtl">20٪</span> | <span dir="rtl">95</span>     | <span dir="rtl">19.0</span>     |
| <span dir="rtl">Cost Evidence</span>         | <span dir="rtl">25٪</span> | <span dir="rtl">58</span>     | <span dir="rtl">14.5</span>     |
| <span dir="rtl">Contribution Evidence</span> | <span dir="rtl">30٪</span> | <span dir="rtl">49</span>     | <span dir="rtl">14.7</span>     |
| <span dir="rtl">Timing Evidence</span>       | <span dir="rtl">10٪</span> | <span dir="rtl">25</span>     | <span dir="rtl">2.5</span>      |
| <span dir="rtl">Uncertainty Treatment</span> | <span dir="rtl">10٪</span> | <span dir="rtl">90</span>     | <span dir="rtl">9.0</span>      |
| <span dir="rtl">Break-even Usefulness</span> | <span dir="rtl">5٪</span>  | <span dir="rtl">95</span>     | <span dir="rtl">4.8</span>      |

| <span dir="rtl">Confidence نهایی: 45/100 — کلاس C :: منطق مالی درست شده، اما ورودی‌های اقتصادی upstream هنوز ضعیف‌اند. بنابراین فعلاً فقط Break-even و Scenario Model قابل دفاع است، نه ROI/Payback قطعی.</span> |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">این نتیجه که «ROI فعلاً نباید تک‌عددی گزارش شود» بسیار Robust است. خود مقدار ROI و Payback فعلاً Robust نیست و با کوچک‌ترین تغییر در uplift/margin/cost می‌تواند عوض شود.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: پس از تکمیل Q27 و Q28، Low/Base/High و سپس در صورت داشتن distributions معتبر Monte Carlo اجرا شود؛ قبل از آن فقط break-even table ارائه شود.</span> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
