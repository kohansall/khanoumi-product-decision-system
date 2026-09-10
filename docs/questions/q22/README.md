<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Q22 | Success Metrics و Guardrails</span></p>
<p><span dir="rtl">آیا قبل از آزمایش، تعریف موفقیت و خط قرمزهای آسیب روشن‌اند؟</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# <span dir="rtl">خلاصه فصل</span>

<span dir="rtl">در این فصل، «موفقیت» از یک حس کلی به Decision Rule تبدیل می‌شود. Feature فقط وقتی ارزش ادامه دارد که Outcome اصلی بهتر شود و هم‌زمان Guardrailهایی مثل توصیه نامناسب، شکایت، مرجوعی یا آسیب اعتماد بدتر نشوند.</span>

## <span dir="rtl">نتیجه فعلی پروژه خانومی</span>

> <span dir="rtl">• Primary outcome باید Incremental باشد، نه فقط engagement.</span>
>
> <span dir="rtl">• Guardrails: inappropriate recommendation، return/cancel، complaint/contact rate، safety incidents، hidden-ad perception.</span>
>
> <span dir="rtl">• Decision rule باید قبل از experiment نوشته شود.</span>
>
> <span dir="rtl">• Threshold عددی فعلاً برای بخش‌هایی که baseline ندارند، TBD یا Directional است.</span>
>
> <span dir="rtl">• Sample size باید بعد از baseline و MDE محاسبه شود، نه حدس زده شود.</span>

# <span dir="rtl">چارچوب کوانتیفیکیشن DECAF</span>

<span dir="rtl">این امتیاز «احتمال آماری موفقیت» نیست. هدف آن سنجش کیفیت شواهد و میزان اتکاپذیری تصمیم فعلی است. معیارها برای همین سؤال انتخاب شده‌اند و با سؤال‌های دیگر لزوماً یکسان نیستند.</span>

## <span dir="rtl">Required Data و وزن اهمیت</span>

| <span dir="rtl">ورودی لازم</span>      | <span dir="rtl">وزن</span> | <span dir="rtl">وضعیت</span>       | <span dir="rtl">نقش در تصمیم</span>        |
|----------------------------------------|----------------------------|------------------------------------|--------------------------------------------|
| <span dir="rtl">Primary outcome</span> | <span dir="rtl">18٪</span> | <span dir="rtl">داریم</span>       | <span dir="rtl">محور تصمیم</span>          |
| <span dir="rtl">Guardrails</span>      | <span dir="rtl">18٪</span> | <span dir="rtl">داریم</span>       | <span dir="rtl">کنترل آسیب</span>          |
| <span dir="rtl">Baselines</span>       | <span dir="rtl">15٪</span> | <span dir="rtl">بخشی نداریم</span> | <span dir="rtl">تعریف threshold</span>     |
| <span dir="rtl">Thresholds/MDE</span>  | <span dir="rtl">15٪</span> | <span dir="rtl">نداریم</span>      | <span dir="rtl">Go/No-Go عددی</span>       |
| <span dir="rtl">Sample size</span>     | <span dir="rtl">12٪</span> | <span dir="rtl">نداریم</span>      | <span dir="rtl">قدرت آزمون</span>          |
| <span dir="rtl">Decision rules</span>  | <span dir="rtl">12٪</span> | <span dir="rtl">قابل تعریف</span>  | <span dir="rtl">پیش‌ثبت تصمیم</span>        |
| <span dir="rtl">Segment safety</span>  | <span dir="rtl">10٪</span> | <span dir="rtl">داریم</span>       | <span dir="rtl">ریسک beauty/medical</span> |

## <span dir="rtl">Have / Missing Classification</span>

| <span dir="rtl">داده/ورودی</span>              | <span dir="rtl">وضعیت</span>      | <span dir="rtl">طبقه Missing</span>           | <span dir="rtl">اثر</span>                            |
|------------------------------------------------|-----------------------------------|-----------------------------------------------|-------------------------------------------------------|
| <span dir="rtl">Guardrail list</span>          | <span dir="rtl">موجود</span>      | <span dir="rtl">—</span>                      | <span dir="rtl">قوی</span>                            |
| <span dir="rtl">Return/support baseline</span> | <span dir="rtl">بخشی موجود</span> | <span dir="rtl">Estimable</span>              | <span dir="rtl">نیاز به feature-level baseline</span> |
| <span dir="rtl">MDE</span>                     | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">برای sample size</span>               |
| <span dir="rtl">Sample size</span>             | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Estimable بعد baseline</span> | <span dir="rtl">نباید جعلی باشد</span>                |
| <span dir="rtl">Go/No-Go thresholds</span>     | <span dir="rtl">ناموجود</span>    | <span dir="rtl">Critical Unknown</span>       | <span dir="rtl">بعد baseline/strategy</span>          |

## <span dir="rtl">Evidence Triangulation</span>

> <span dir="rtl">• VOC و Survey برای ریسک انتخاب نامناسب.</span>
>
> <span dir="rtl">• گزارش‌های رسمی برای سلامت فعلی fulfillment/support به‌عنوان context.</span>
>
> <span dir="rtl">• Safety/medical boundary از طراحی Chatbot و nature محصول beauty.</span>

| <span dir="rtl">کنترل Double Counting :: مشتقات یک Dataset، چند نمودار از یک Survey، یا چند سندی که یک منبع اصلی را تکرار می‌کنند، Evidence مستقل محسوب نمی‌شوند.</span> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Cap Rules و Penaltyها</span>

> <span dir="rtl">• Threshold بدون baseline یا rationale باید TBD/Hypothesis باشد.</span>
>
> <span dir="rtl">• Sample size بدون baseline rate و MDE قابل دفاع نیست.</span>
>
> <span dir="rtl">• اگر Success Metric رشد کند ولی Guardrail بحرانی بدتر شود، Feature موفق محسوب نمی‌شود.</span>

## <span dir="rtl">Sensitivity و VOI</span>

| <span dir="rtl">ورودی</span>              | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>    | <span dir="rtl">دلیل</span>                           |
|-------------------------------------------|------------------------------------|-------------------------------|-------------------------------------------------------|
| <span dir="rtl">MDE</span>                | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">sample و decision را عوض می‌کند</span> |
| <span dir="rtl">Baseline rates</span>     | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">threshold و power را عوض می‌کند</span> |
| <span dir="rtl">Guardrail severity</span> | <span dir="rtl">High</span>        | <span dir="rtl">Medium</span> | <span dir="rtl">Go/No-Go را محدود می‌کند</span>        |
| <span dir="rtl">Experiment window</span>  | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span> | <span dir="rtl">برای purchase lag مهم است</span>      |

> <span dir="rtl">• بالاترین VOI: baseline و MDE برای outcome اصلی.</span>
>
> <span dir="rtl">• برای Guardrailهای safety، حتی رخداد کم‌تعداد ممکن است تصمیم‌ساز باشد و نباید صرفاً با میانگین پنهان شود.</span>

## <span dir="rtl">محاسبه Confidence</span>

| <span dir="rtl">معیار</span>                  | <span dir="rtl">وزن</span> | <span dir="rtl">امتیاز</span> | <span dir="rtl">سهم وزنی</span> |
|-----------------------------------------------|----------------------------|-------------------------------|---------------------------------|
| <span dir="rtl">Outcome Definition</span>     | <span dir="rtl">20٪</span> | <span dir="rtl">90</span>     | <span dir="rtl">18.0</span>     |
| <span dir="rtl">Guardrail Coverage</span>     | <span dir="rtl">20٪</span> | <span dir="rtl">92</span>     | <span dir="rtl">18.4</span>     |
| <span dir="rtl">Baseline Evidence</span>      | <span dir="rtl">15٪</span> | <span dir="rtl">50</span>     | <span dir="rtl">7.5</span>      |
| <span dir="rtl">Threshold Rationale</span>    | <span dir="rtl">15٪</span> | <span dir="rtl">42</span>     | <span dir="rtl">6.3</span>      |
| <span dir="rtl">Sample/Power Readiness</span> | <span dir="rtl">15٪</span> | <span dir="rtl">30</span>     | <span dir="rtl">4.5</span>      |
| <span dir="rtl">Decision Rule Quality</span>  | <span dir="rtl">15٪</span> | <span dir="rtl">88</span>     | <span dir="rtl">13.2</span>     |

| <span dir="rtl">Confidence نهایی: 74/100 — کلاس B :: ساختار Outcome/Guardrail قوی است، اما بدون baseline، MDE و sample calculation نمی‌توان Success Threshold عددی قطعی ساخت.</span> |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## <span dir="rtl">Decision Robustness</span>

<span dir="rtl">لیست Guardrailها و اصل تصمیم‌گیری پابرجاست؛ نمره پایین‌تر به خاطر نبود داده‌ای است که Threshold و Sample Size را عددی کند، نه ضعف مفهوم اندازه‌گیری.</span>

## <span dir="rtl">Next Evidence Action</span>

| <span dir="rtl">اقدام بعدی :: از analytics نرخ‌های پایه outcome و guardrail استخراج شود؛ سپس MDE تجاری تعیین و sample size با آزمون مناسب محاسبه شود.</span> |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
