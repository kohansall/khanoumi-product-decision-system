<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q17 | Roadmap از MVP تا Launch</span></p>
<p><span dir="rtl">آیا توالی مراحل، Gateها و وابستگی‌ها برای حرکت از Validation تا Scale قابل دفاع‌اند؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">در این فصل، Roadmap به‌جای تقویم Featureها به یک زنجیره تصمیم تبدیل می‌شود. مسیر پیشنهادی خانومی از Demand Validation شروع می‌شود، سپس Concierge/Wizard-of-Oz، Rule-based MVP، Limited Pilot، Launch Readiness و در نهایت Scale Decision. هر فاز فقط وقتی به فاز بعدی می‌رود که معیار خروج آن پاس شود.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• Phase 1 — Demand Validation: Fake Door و سنجش تقاضای واقعی.</span>
>
> <span dir="rtl">• Phase 2 — Concierge / Wizard-of-Oz: ارائه پیشنهاد با عملیات دستی برای یادگیری سریع.</span>
>
> <span dir="rtl">• Phase 3 — Rule-based MVP: خودکارسازی حداقلی منطق پیشنهاد.</span>
>
> <span dir="rtl">• Phase 4 — Limited Pilot: اتصال محدود به مسیر خرید و پایش Guardrailها.</span>
>
> <span dir="rtl">• Phase 5 — Launch Readiness: رفع ریسک‌های داده، Safety، Analytics و Operations.</span>
>
> <span dir="rtl">• Phase 6 — Scale Decision: تصمیم Build/Scale بر اساس Outcome، نه صرفاً تحویل Feature.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>          | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>  | <span dir="rtl">نقش در تصمیم</span>              |
|--------------------------------------------|----------------------------|-------------------------------|--------------------------------------------------|
| <span dir="rtl">Phases & gates</span>      | <span dir="rtl">20٪</span> | <span dir="rtl">داریم</span>  | <span dir="rtl">توالی یادگیری و شرط عبور</span>  |
| <span dir="rtl">Dependencies</span>        | <span dir="rtl">15٪</span> | <span dir="rtl">داریم</span>  | <span dir="rtl">جلوگیری از Build زودهنگام</span> |
| <span dir="rtl">Exit criteria</span>       | <span dir="rtl">20٪</span> | <span dir="rtl">نسبی</span>   | <span dir="rtl">تعریف تصمیم پایان هر فاز</span>  |
| <span dir="rtl">Validation signals</span>  | <span dir="rtl">15٪</span> | <span dir="rtl">داریم</span>  | <span dir="rtl">اتصال Roadmap به Evidence</span> |
| <span dir="rtl">Team capacity</span>       | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span> | <span dir="rtl">واقعی‌کردن تاریخ و حجم</span>     |
| <span dir="rtl">Technical estimates</span> | <span dir="rtl">10٪</span> | <span dir="rtl">نداریم</span> | <span dir="rtl">زمان‌بندی Delivery</span>         |
| <span dir="rtl">Risk register</span>       | <span dir="rtl">5٪</span>  | <span dir="rtl">داریم</span>  | <span dir="rtl">کنترل ریسک</span>                |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>         | <span dir="rtl">وضعیت</span>   | <span dir="rtl">طبقه Missing</span>             | <span dir="rtl">اثر</span>                  |
|-------------------------------------------|--------------------------------|-------------------------------------------------|---------------------------------------------|
| <span dir="rtl">توالی فازها</span>        | <span dir="rtl">موجود</span>   | <span dir="rtl">—</span>                        | <span dir="rtl">قوی</span>                  |
| <span dir="rtl">ظرفیت واقعی تیم</span>    | <span dir="rtl">ناموجود</span> | <span dir="rtl">Critical Unknown</span>         | <span dir="rtl">روی تاریخ اثر مستقیم</span> |
| <span dir="rtl">Velocity تاریخی</span>    | <span dir="rtl">ناموجود</span> | <span dir="rtl">Estimable after sprint 1</span> | <span dir="rtl">برای forecast دقیق</span>   |
| <span dir="rtl">Gateهای Validation</span> | <span dir="rtl">موجود</span>   | <span dir="rtl">—</span>                        | <span dir="rtl">قوی</span>                  |
| <span dir="rtl">تاریخ قطعی Launch</span>  | <span dir="rtl">ناموجود</span> | <span dir="rtl">Ignorable فعلاً</span>           | <span dir="rtl">نباید جعل شود</span>        |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• Evidence پژوهش کاربر و Q1–Q14 برای اینکه Roadmap از مسئله شروع شود.</span>
>
> <span dir="rtl">• MVP و Scope از Q15–Q16 برای تعریف مراحل ساخت.</span>
>
> <span dir="rtl">• منطق Stage-gate با اصول Discovery و جلوگیری از Build Trap هم‌راستاست.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• بدون ظرفیت واقعی تیم، تاریخ دقیق یا velocity قطعی ممنوع است.</span>
>
> <span dir="rtl">• Roadmap بدون Exit Criteria حداکثر Confidence = 69.</span>
>
> <span dir="rtl">• اگر فاز Scale قبل از Validation Outcome تعریف شود، حداقل 15 امتیاز Penalty.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>              | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>    | <span dir="rtl">دلیل</span>                                |
|-------------------------------------------|------------------------------------|-------------------------------|------------------------------------------------------------|
| <span dir="rtl">Team capacity</span>      | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">تاریخ و حجم Sprintها را تغییر می‌دهد</span> |
| <span dir="rtl">Validation gates</span>   | <span dir="rtl">High</span>        | <span dir="rtl">Medium</span> | <span dir="rtl">می‌تواند توقف/ادامه را عوض کند</span>       |
| <span dir="rtl">Technical estimate</span> | <span dir="rtl">Medium</span>      | <span dir="rtl">High</span>   | <span dir="rtl">روی sequencing و duration اثر دارد</span>  |
| <span dir="rtl">Exact launch date</span>  | <span dir="rtl">Low فعلاً</span>    | <span dir="rtl">Low</span>    | <span dir="rtl">برای Discovery تصمیم حیاتی نیست</span>     |

> <span dir="rtl">• بیشترین VOI: ظرفیت واقعی Design/Engineering/Data و تخمین فنی Rule-based MVP.</span>
>
> <span dir="rtl">• بعد از Sprint اول، velocity واقعی می‌تواند forecast را جایگزین planning proposal کند.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                       | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|----------------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Phase/Gate Logic</span>            | <span dir="rtl">25٪</span> | <span dir="rtl">92</span>     | <span dir="rtl">23.0</span>     |
| <span dir="rtl">Dependency Coverage</span>         | <span dir="rtl">20٪</span> | <span dir="rtl">88</span>     | <span dir="rtl">17.6</span>     |
| <span dir="rtl">Exit Criteria Quality</span>       | <span dir="rtl">20٪</span> | <span dir="rtl">82</span>     | <span dir="rtl">16.4</span>     |
| <span dir="rtl">Capacity Evidence</span>           | <span dir="rtl">15٪</span> | <span dir="rtl">35</span>     | <span dir="rtl">5.2</span>      |
| <span dir="rtl">Technical Estimate Evidence</span> | <span dir="rtl">10٪</span> | <span dir="rtl">30</span>     | <span dir="rtl">3.0</span>      |
| <span dir="rtl">Risk & Validation Alignment</span> | <span dir="rtl">10٪</span> | <span dir="rtl">90</span>     | <span dir="rtl">9.0</span>      |

| <span dir="rtl">Confidence نهایی: 78/100 — کلاس B :: منطق توالی و Gateها قابل دفاع است، اما بدون ظرفیت و تخمین فنی واقعی، بخش زمان‌بندی هنوز Proposal است نه Forecast.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">ترتیب کلی Validation → Concierge → Rule-based MVP → Pilot → Scale در برابر تغییر اکثر فرض‌ها پایدار است؛ چیزی که شکننده است تاریخ و ظرفیت اجرای هر فاز است، نه منطق Stage-gate.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: یک Capacity Check کوتاه با PM/Engineering/Design انجام شود و برای هر فاز Person-day یا T-shirt estimate ثبت شود؛ سپس تاریخ‌ها به Roadmap اضافه شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
