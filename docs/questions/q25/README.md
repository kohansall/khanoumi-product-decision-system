<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q25 | برنامه Acquisition</span></p>
<p><span dir="rtl">آیا برنامه جذب برای تست و سپس رشد Feature به داده و اقتصاد کانال متصل است؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">در این پروژه، Acquisition در فاز اول به معنی خرید ترافیک جدید نیست. هدف اولیه رساندن کاربران Eligible موجود به Fake Door و سنجش تقاضاست. بنابراین Owned Traffic داخل سایت و CRM منطقی‌تر از هزینه‌کرد سنگین Paid است؛ اما مقیاس‌دادن Acquisition بدون CAC/CTR/CVR واقعی قابل دفاع نیست.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• فاز Validation: placement داخل Home/PDP/Search، CRM و owned surfaces.</span>
>
> <span dir="rtl">• پیام اصلی Fake Door: «در ۲ دقیقه محصول مناسبم را پیدا کن».</span>
>
> <span dir="rtl">• Segment اولیه: کاربرانی با Need مشخص ولی SKU نامشخص یا uncertainty بالا.</span>
>
> <span dir="rtl">• Paid acquisition فقط بعد از اثبات downstream value و داشتن channel economics.</span>
>
> <span dir="rtl">• Attribution باید source/placement → funnel → purchase را وصل کند.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>             | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>      | <span dir="rtl">نقش در تصمیم</span>           |
|-----------------------------------------------|----------------------------|-----------------------------------|-----------------------------------------------|
| <span dir="rtl">Target segment</span>         | <span dir="rtl">15٪</span> | <span dir="rtl">داریم</span>      | <span dir="rtl">تمرکز پیام و placement</span> |
| <span dir="rtl">Owned traffic baseline</span> | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>     | <span dir="rtl">حجم تست</span>                |
| <span dir="rtl">Channel CTR</span>            | <span dir="rtl">10٪</span> | <span dir="rtl">نداریم</span>     | <span dir="rtl">تقاضا</span>                  |
| <span dir="rtl">CVR downstream</span>         | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>     | <span dir="rtl">ارزش اقتصادی</span>           |
| <span dir="rtl">CAC / incremental cost</span> | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>     | <span dir="rtl">مقیاس‌پذیری</span>             |
| <span dir="rtl">Message proposition</span>    | <span dir="rtl">10٪</span> | <span dir="rtl">داریم</span>      | <span dir="rtl">testable demand</span>        |
| <span dir="rtl">Attribution</span>            | <span dir="rtl">10٪</span> | <span dir="rtl">قابل طراحی</span> | <span dir="rtl">اثر کانال</span>              |
| <span dir="rtl">Channel fit</span>            | <span dir="rtl">10٪</span> | <span dir="rtl">نسبی</span>       | <span dir="rtl">انتخاب سطح تست</span>         |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>           | <span dir="rtl">وضعیت</span>   | <span dir="rtl">طبقه Missing</span>           | <span dir="rtl">اثر</span>                   |
|---------------------------------------------|--------------------------------|-----------------------------------------------|----------------------------------------------|
| <span dir="rtl">Segment hypothesis</span>   | <span dir="rtl">موجود</span>   | <span dir="rtl">—</span>                      | <span dir="rtl">متوسط/قوی</span>             |
| <span dir="rtl">Owned traffic volume</span> | <span dir="rtl">ناموجود</span> | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">برای sample/timing</span>    |
| <span dir="rtl">Paid CAC</span>             | <span dir="rtl">ناموجود</span> | <span dir="rtl">Ignorable در Fake Door</span> | <span dir="rtl">برای scale بعداً مهم</span>   |
| <span dir="rtl">Message</span>              | <span dir="rtl">موجود</span>   | <span dir="rtl">—</span>                      | <span dir="rtl">قابل تست</span>              |
| <span dir="rtl">Attribution</span>          | <span dir="rtl">نسبی</span>    | <span dir="rtl">Estimable</span>              | <span dir="rtl">با UTM/event property</span> |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• Need/uncertainty از Q2–Q4 برای segment و message.</span>
>
> <span dir="rtl">• Current mobile-heavy ecommerce context برای placementهای داخل سایت.</span>
>
> <span dir="rtl">• MVP Fake Door از Q15 برای acquisition validation low-cost.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• بدون traffic baseline، forecast حجم acquisition قطعی ممنوع.</span>
>
> <span dir="rtl">• بدون CAC و downstream CVR، Paid scale business case حداکثر Confidence = 59.</span>
>
> <span dir="rtl">• Channel recommendation که فقط از benchmark خارجی آمده باشد باید Hypothesis بماند.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>          | <span dir="rtl">Sensitivity</span>         | <span dir="rtl">VOI</span>    | <span dir="rtl">دلیل</span>              |
|---------------------------------------|--------------------------------------------|-------------------------------|------------------------------------------|
| <span dir="rtl">Owned traffic</span>  | <span dir="rtl">High</span>                | <span dir="rtl">High</span>   | <span dir="rtl">سرعت و sample تست</span> |
| <span dir="rtl">CTA CTR</span>        | <span dir="rtl">High</span>                | <span dir="rtl">High</span>   | <span dir="rtl">سیگنال demand</span>     |
| <span dir="rtl">Downstream CVR</span> | <span dir="rtl">High</span>                | <span dir="rtl">High</span>   | <span dir="rtl">ارزش واقعی کانال</span>  |
| <span dir="rtl">Paid CAC</span>       | <span dir="rtl">Low فعلاً/High scale</span> | <span dir="rtl">Medium</span> | <span dir="rtl">در فاز بعد حیاتی</span>  |

> <span dir="rtl">• ابتدا exposure و CTR روی owned surfaces اندازه‌گیری شود؛ این ارزان‌ترین Evidence با VOI بالا است.</span>
>
> <span dir="rtl">• بعد از اثبات engagement، attribution تا purchase و سپس CAC scale بررسی شود.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                 | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|----------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Segment Evidence</span>      | <span dir="rtl">20٪</span> | <span dir="rtl">78</span>     | <span dir="rtl">15.6</span>     |
| <span dir="rtl">Channel Fit Logic</span>     | <span dir="rtl">20٪</span> | <span dir="rtl">82</span>     | <span dir="rtl">16.4</span>     |
| <span dir="rtl">Traffic Baseline</span>      | <span dir="rtl">15٪</span> | <span dir="rtl">25</span>     | <span dir="rtl">3.8</span>      |
| <span dir="rtl">Economics Evidence</span>    | <span dir="rtl">15٪</span> | <span dir="rtl">20</span>     | <span dir="rtl">3.0</span>      |
| <span dir="rtl">Message Testability</span>   | <span dir="rtl">15٪</span> | <span dir="rtl">90</span>     | <span dir="rtl">13.5</span>     |
| <span dir="rtl">Attribution Readiness</span> | <span dir="rtl">15٪</span> | <span dir="rtl">72</span>     | <span dir="rtl">10.8</span>     |

| <span dir="rtl">Confidence نهایی: 68/100 — کلاس B :: استراتژی فاز Validation منطقی و کم‌ریسک است، ولی بدون baseline ترافیک و اقتصاد کانال نمی‌توان forecast Acquisition یا scale plan عددی داد.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">اولویت دادن به Owned Traffic برای Demand Validation حتی با تغییر اکثر فرض‌ها منطقی می‌ماند؛ چیزی که شکننده است اندازه، زمان و هزینه Scale است.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: برای 3 placement داخلی، Exposure baseline و CTR فعلی استخراج شود؛ Fake Door با source property اجرا و downstream funnel به‌صورت cohort ردیابی شود.</span> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
