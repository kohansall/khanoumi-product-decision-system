<span dir="rtl">سؤال ۱</span>

<span dir="rtl">بازسازی جریان‌های فعلی کاربر در خانومی</span>

<span dir="rtl">Current-State User Flows & Journey Reconstruction</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">خلاصه یک‌خطی</span></p>
<p><span dir="rtl">در سؤال اول هنوز قرار نیست راه‌حل انتخاب کنیم. هدف این است که از روی شواهد موجود، مسیر واقعی و قابل دفاع کاربر را از «نیاز» تا «خرید، تجربه محصول و خرید مجدد» بازسازی کنیم و دقیقاً مشخص کنیم کجا مشاهده مستقیم داریم و کجا صرفاً استنتاج تحلیلی داریم.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

| <span dir="rtl">وضعیت پاسخ</span>                   | <span dir="rtl">کلاس</span> | <span dir="rtl">Confidence</span> | <span dir="rtl">روش</span>                       |
|-----------------------------------------------------|-----------------------------|-----------------------------------|--------------------------------------------------|
| <span dir="rtl">قابل استفاده برای تصمیم بعدی</span> | <span dir="rtl">A</span>    | <span dir="rtl">84 / 100</span>   | <span dir="rtl">DECAF Quantification v1.0</span> |

<span dir="rtl">این ۸۴٪ «نرخ تکمیل پروژه» یا «احتمال درستی Flow» نیست؛ نمره Confidence تصمیمی است که بر اساس کیفیت شواهد، پوشش داده‌های لازم، مثلث‌سازی، میزان وابستگی به فرض و حساسیت به داده‌های گمشده ساخته شده است.</span>

<span dir="rtl">۱. روایت فصل — در این مرحله چه اتفاقی افتاد؟</span>

<span dir="rtl">برای پاسخ به سؤال ۱، Journey را از روی یک Funnel عمومی فروشگاه اینترنتی حدس نزدیم. ابتدا رفتار گزارش‌شده خریداران اخیر را خواندیم، بعد مسیر خروج و جایگزین‌های Never/Lapsed را اضافه کردیم، سپس تم‌های Voice of Customer و مشاهده UX لندینگ، چت‌بات و مسیر خرید را برای Cross-check به کار بردیم. نتیجه یک Current-State Journey است که Transaction را از Evaluation جدا می‌کند و نشان می‌دهد بیشترین سیگنال فعلی اصطکاک، قبل از تکمیل تصمیم خرید دیده می‌شود؛ نه اینکه از همین حالا یک Feature خاص را اثبات کند.</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">اصل پژوهشی فصل</span></p>
<p><span dir="rtl">Flow قابل مشاهده، Flow گزارش‌شده و Flow استنتاجی سه چیز متفاوت‌اند. در این سند این سه سطح با هم مخلوط نمی‌شوند.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl">۲. سؤال تصمیمی</span>

<span dir="rtl">آیا با داده‌های فعلی می‌توانیم مسیرهای اصلی کاربر خانومی را به اندازه کافی دقیق بازسازی کنیم که در مراحل بعدی، Problem Discovery و Prioritization روی یک نقشه معتبر از تجربه فعلی بنا شوند؟</span>

<span dir="rtl">۳. مرز پاسخ</span>

<span dir="rtl">• این فصل Current State را توضیح می‌دهد؛ Solution انتخاب نمی‌کند.</span>

<span dir="rtl">• این فصل می‌تواند وجود مراحل و مسیرهای اصلی را بازسازی کند؛ اما بدون Product Analytics درباره نرخ Drop-off، Frequency یا سهم هر مسیر در کل کاربران ادعای قطعی نمی‌کند.</span>

<span dir="rtl">• Surveyها نمونه Convenience هستند؛ درصدهای آن‌ها فقط توصیف همان نمونه‌اند، نه برآورد جمعیت کاربران خانومی.</span>

<span dir="rtl">• UX Review مشاهده کارشناسی است؛ جای Usability Test مشاهده‌ای با کاربر واقعی را نمی‌گیرد.</span>

<span dir="rtl">۴. Evidence Base و نقش هر منبع</span>

| <span dir="rtl">منبع</span>                  | <span dir="rtl">حجم / پوشش</span>                         | <span dir="rtl">نقش در Q1</span>                                                         | <span dir="rtl">محدودیت</span>                               |
|----------------------------------------------|-----------------------------------------------------------|------------------------------------------------------------------------------------------|--------------------------------------------------------------|
| <span dir="rtl">Survey خریداران اخیر</span>  | <span dir="rtl">n=46</span>                               | <span dir="rtl">Trigger، Evaluation، Decision، Checkout، Fulfillment، Repurchase</span>  | <span dir="rtl">Self-report و نمونه غیرتصادفی</span>         |
| <span dir="rtl">Survey Never/Lapsed</span>   | <span dir="rtl">n=28؛ 17 Never + 11 Lapsed</span>         | <span dir="rtl">مسیر خروج، جایگزین‌ها و مانع ورود/بازگشت</span>                           | <span dir="rtl">نمونه کوچک و Convenience</span>              |
| <span dir="rtl">VOC تمیزشده</span>           | <span dir="rtl">39,737 کامنت؛ 4,023 Problem-tagged</span> | <span dir="rtl">Cross-check تم‌های تجربه و مسئله</span>                                   | <span dir="rtl">کامنت‌نویسان نماینده کل مشتریان نیستند</span> |
| <span dir="rtl">VOC خام</span>               | <span dir="rtl">76,837 کامنت</span>                       | <span dir="rtl">Data lineage و کنترل نسخه تحلیل</span>                                   | <span dir="rtl">مبنای مستقیم Theme Frequency نیست</span>     |
| <span dir="rtl">UX Review</span>             | <span dir="rtl">Landing + Chatbot + Purchase Flow</span>  | <span dir="rtl">معماری مشاهده‌پذیر Flow و نقاط تعامل</span>                               | <span dir="rtl">Expert observation، نه usability test</span> |
| <span dir="rtl">گزارش‌های مدیریتی/رسمی</span> | <span dir="rtl">context عملیاتی</span>                    | <span dir="rtl">کنترل اینکه Transaction/Fulfillment را بی‌دلیل Root Problem ننامیم</span> | <span dir="rtl">برای Frequency رفتاری کافی نیست</span>       |

<span dir="rtl">۵. Current-State Journey نهایی</span>

| <span dir="rtl">مرحله</span>                     | <span dir="rtl">سؤال کاربر</span>                 | <span dir="rtl">رفتار فعلی قابل بازسازی</span>                            | <span dir="rtl">خروجی محتمل</span>                |
|--------------------------------------------------|---------------------------------------------------|---------------------------------------------------------------------------|---------------------------------------------------|
| <span dir="rtl">۱. Trigger</span>                | <span dir="rtl">الان چه نیازی دارم؟</span>        | <span dir="rtl">نیاز محصول، تمام‌شدن محصول، تخفیف، تحقیق/مقایسه</span>     | <span dir="rtl">ورود به Discovery یا تعویق</span> |
| <span dir="rtl">۲. Discovery</span>              | <span dir="rtl">چه گزینه‌هایی وجود دارد؟</span>    | <span dir="rtl">Home / Search / Category / Campaign / Product List</span> | <span dir="rtl">فهرست گزینه‌ها</span>              |
| <span dir="rtl">۳. Evaluation</span>             | <span dir="rtl">کدام گزینه مناسب‌تر است؟</span>    | <span dir="rtl">قیمت، تخفیف، Fit، اطلاعات، نظرها، اصالت، موجودی</span>    | <span dir="rtl">Confidence یا Doubt</span>        |
| <span dir="rtl">۴. Confidence Check</span>       | <span dir="rtl">چطور مطمئن شوم؟</span>            | <span dir="rtl">Review، مقایسه بیرونی، سؤال از دیگران، تعویق</span>       | <span dir="rtl">Buy / Delay / Exit</span>         |
| <span dir="rtl">۵. PDP / Decision</span>         | <span dir="rtl">آیا این SKU را انتخاب کنم؟</span> | <span dir="rtl">مرور جزئیات و تصمیم نهایی</span>                          | <span dir="rtl">Add to Cart یا خروج</span>        |
| <span dir="rtl">۶. Transaction</span>            | <span dir="rtl">چطور خرید را تمام کنم؟</span>     | <span dir="rtl">Cart → Login/OTP → Address → Shipping → Payment</span>    | <span dir="rtl">Order</span>                      |
| <span dir="rtl">۷. Fulfillment</span>            | <span dir="rtl">آیا درست و سالم می‌رسد؟</span>     | <span dir="rtl">Delivery / Packaging / Match</span>                       | <span dir="rtl">Receive یا Issue</span>           |
| <span dir="rtl">۸. Product Experience</span>     | <span dir="rtl">واقعاً مناسب بود؟</span>           | <span dir="rtl">استفاده و ارزیابی Fit/Effect/Texture</span>               | <span dir="rtl">Satisfaction یا Mismatch</span>   |
| <span dir="rtl">۹. Repurchase / Switching</span> | <span dir="rtl">دوباره از کجا بخرم؟</span>        | <span dir="rtl">یادآوری، بازگشت، تغییر برند/کانال</span>                  | <span dir="rtl">Repurchase یا Switch</span>       |

<span dir="rtl">۶. چهار مسیر اصلی که از شواهد استخراج می‌شوند</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Flow A — کاربر با محصول مشخص</span></p>
<p><span dir="rtl">Need / Trigger → Search → Product List → PDP → Review / Price / Product Info → Add to Cart → Login / OTP → Address → Shipping → Payment → Order</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Flow B — کاربر با نیاز، بدون SKU مشخص</span></p>
<p><span dir="rtl">Need → Home / Category / Search → Browse → Compare → Reviews / Product Info → Confidence Check → PDP → Cart → Checkout</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Flow C — ورود کمپینی / تخفیفی</span></p>
<p><span dir="rtl">Campaign / Promotion → Landing → Product List → PDP → Price / Discount Evaluation → Cart → Checkout</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Flow D — کمک و پشتیبانی</span></p>
<p><span dir="rtl">Question / Problem → Chatbot → FAQ / Routing → Answer یا Human Handoff → بازگشت به Shopping / Support</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">Flow E — حلقه پس از خرید</span></p>
<p><span dir="rtl">Purchase → Delivery → Product Experience → Satisfaction / Dissatisfaction → Repurchase / Alternative / Switching</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl">۷. سیگنال‌های رفتاری کلیدی که شکل Journey را توضیح می‌دهند</span>

| <span dir="rtl">سیگنال</span>               | <span dir="rtl">داده موجود</span>                                                     | <span dir="rtl">برداشت مجاز</span>                                                         |
|---------------------------------------------|---------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|
| <span dir="rtl">سخت‌ترین بخش مراجعه</span>   | <span dir="rtl">16/46 اعتماد به اطلاعات/نظرها؛ 11/46 Fit؛ 1/46 سبد و پرداخت</span>    | <span dir="rtl">در این نمونه، friction گزارش‌شده بیشتر در Evaluation است تا Checkout</span> |
| <span dir="rtl">وقتی کاربر مردد است</span>  | <span dir="rtl">23/46 Review؛ 15/46 مقایسه سایت دیگر؛ 12/46 تعویق</span>              | <span dir="rtl">Confidence Check بخشی واقعی از Journey گزارش‌شده است</span>                 |
| <span dir="rtl">نتیجه آخرین مراجعه</span>   | <span dir="rtl">27 خرید کامل؛ 19 بدون خرید کامل</span>                                | <span dir="rtl">فقط outcome نمونه؛ Conversion Rate سایت نیست</span>                        |
| <span dir="rtl">تطابق سفارش</span>          | <span dir="rtl">38/46 درست؛ 7 packaging dissatisfaction؛ 1 wrong/incomplete</span>    | <span dir="rtl">Fulfillment در نمونه سیگنال بحران غالب ندارد</span>                        |
| <span dir="rtl">Never/Lapsed جایگزین</span> | <span dir="rtl">فروشگاه فیزیکی، داروخانه، سایر Onlineها، influencer/competitor</span> | <span dir="rtl">Switching باید در Journey دیده شود، نه فقط Checkout</span>                 |
| <span dir="rtl">VOC</span>                  | <span dir="rtl">Availability، price، sensory، quality، effectiveness و...</span>      | <span dir="rtl">تجربه تصمیم/مصرف چندعاملی است؛ Count کامنت = prevalence کاربر نیست</span>  |

<span dir="rtl">۸. نقشه داده‌های لازم برای Q1</span>

<span dir="rtl">وزن‌ها نشان می‌دهند نبود هر داده چقدر می‌تواند بازسازی Journey را ناقص کند. مجموع وزن‌ها ۱۰۰ است؛ این وزن‌ها مخصوص سؤال ۱ هستند و در سؤال‌های دیگر تغییر می‌کنند.</span>

| <span dir="rtl">داده لازم</span>                       | <span dir="rtl">وزن اهمیت</span> | <span dir="rtl">وضعیت فعلی</span>      | <span dir="rtl">نوع برخورد</span>                               |
|--------------------------------------------------------|----------------------------------|----------------------------------------|-----------------------------------------------------------------|
| <span dir="rtl">Landing / Home</span>                  | <span dir="rtl">12٪</span>       | <span dir="rtl">داریم</span>           | <span dir="rtl">Observed / UX evidence</span>                   |
| <span dir="rtl">Search / Category / Browse</span>      | <span dir="rtl">13٪</span>       | <span dir="rtl">تا حد خوب داریم</span> | <span dir="rtl">Observed + survey-supported</span>              |
| <span dir="rtl">PDP / Evaluation</span>                | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم</span>           | <span dir="rtl">Survey + VOC + UX</span>                        |
| <span dir="rtl">Chatbot / Support</span>               | <span dir="rtl">8٪</span>        | <span dir="rtl">داریم</span>           | <span dir="rtl">Observed UX</span>                              |
| <span dir="rtl">Cart / Checkout</span>                 | <span dir="rtl">15٪</span>       | <span dir="rtl">داریم</span>           | <span dir="rtl">Observed + survey signal</span>                 |
| <span dir="rtl">Login / OTP / Address / Payment</span> | <span dir="rtl">7٪</span>        | <span dir="rtl">بخشی داریم</span>      | <span dir="rtl">Observed architecture؛ telemetry نداریم</span>  |
| <span dir="rtl">Delivery / Post-purchase</span>        | <span dir="rtl">7٪</span>        | <span dir="rtl">داریم</span>           | <span dir="rtl">Survey + official context</span>                |
| <span dir="rtl">Repurchase / Switching</span>          | <span dir="rtl">7٪</span>        | <span dir="rtl">داریم</span>           | <span dir="rtl">Survey + Never/Lapsed</span>                    |
| <span dir="rtl">Behavioral Analytics</span>            | <span dir="rtl">10٪</span>       | <span dir="rtl">نداریم</span>          | <span dir="rtl">Critical unknown برای frequency/drop-off</span> |
| <span dir="rtl">Edge / Failure States</span>           | <span dir="rtl">6٪</span>        | <span dir="rtl">محدود</span>           | <span dir="rtl">Estimable only as hypotheses</span>             |

<span dir="rtl">۹. طبقه‌بندی Missing Data</span>

| <span dir="rtl">کلاس</span>               | <span dir="rtl">برای Q1 چه چیزهایی داخل آن است؟</span>                                                  | <span dir="rtl">اثر بر تصمیم</span>                                                               |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| <span dir="rtl">قابل برآورد</span>        | <span dir="rtl">بخشی از Post-purchase sequence، switching logic، برخی failure paths</span>              | <span dir="rtl">برای ترسیم ساختار Journey قابل استفاده است، اما باید Inference label بخورد</span> |
| <span dir="rtl">قابل اغماض برای Q1</span> | <span dir="rtl">سهم دقیق روش‌های پرداخت، تعداد کلیک Navigation، نرخ استفاده Chatbot، Time-on-page</span> | <span dir="rtl">برای «وجود Flow» ضروری نیست؛ در KPI/analytics بعداً مهم می‌شود</span>               |
| <span dir="rtl">Critical Unknown</span>   | <span dir="rtl">Session-level telemetry، واقعی‌ترین drop-offها، observed usability behavior</span>       | <span dir="rtl">ممکن است محل و شدت friction را جابه‌جا کند؛ سقف برخی ادعاها را محدود می‌کند</span>  |

<span dir="rtl">۱۰. DECAF Quantification v1.0 — معیارهای Q1</span>

<span dir="rtl">Confidence سؤال ۱ با پنج معیار ثابت DECAF محاسبه می‌شود، اما ورودی و حساسیت هر معیار مخصوص همین سؤال است.</span>

| <span dir="rtl">معیار</span>                           | <span dir="rtl">وزن</span> | <span dir="rtl">تعریف در Q1</span>                                                      | <span dir="rtl">نمره Q1</span> |
|--------------------------------------------------------|----------------------------|-----------------------------------------------------------------------------------------|--------------------------------|
| <span dir="rtl">Direct Evidence Quality</span>         | <span dir="rtl">30٪</span> | <span dir="rtl">کیفیت مشاهده/داده مستقیم درباره Flow و Journey</span>                   | <span dir="rtl">90</span>      |
| <span dir="rtl">Required Data Coverage</span>          | <span dir="rtl">25٪</span> | <span dir="rtl">چه سهمی از داده‌های لازم با شواهد قابل استفاده پوشش داده شده</span>      | <span dir="rtl">85</span>      |
| <span dir="rtl">Evidence Triangulation</span>          | <span dir="rtl">20٪</span> | <span dir="rtl">هم‌گرایی خانواده‌های مستقل Survey، VOC، UX و context رسمی</span>          | <span dir="rtl">88</span>      |
| <span dir="rtl">Low Dependency on Assumptions</span>   | <span dir="rtl">15٪</span> | <span dir="rtl">تا چه حد نقشه Journey بدون فرض‌های سنگین پابرجاست</span>                 | <span dir="rtl">85</span>      |
| <span dir="rtl">Low Sensitivity to Missing Data</span> | <span dir="rtl">10٪</span> | <span dir="rtl">اگر داده‌های گمشده اضافه شوند، آیا ساختار اصلی Journey عوض می‌شود؟</span> | <span dir="rtl">55</span>      |

<span dir="rtl">۱۱. Rubric امتیازدهی ثابت</span>

| <span dir="rtl">بازه</span>   | <span dir="rtl">معنای Evidence Score</span>                                        |
|-------------------------------|------------------------------------------------------------------------------------|
| <span dir="rtl">90–100</span> | <span dir="rtl">داده مستقیم/مشاهده معتبر، منبع رسمی تازه یا telemetry مناسب</span> |
| <span dir="rtl">75–89</span>  | <span dir="rtl">شواهد ساختاریافته و قابل دفاع با محدودیت روشن</span>               |
| <span dir="rtl">50–74</span>  | <span dir="rtl">Proxy معتبر، نمونه Convenience یا evidence غیرمستقیم</span>        |
| <span dir="rtl">30–49</span>  | <span dir="rtl">Expert inference با شواهد محدود</span>                             |
| <span dir="rtl">0–29</span>   | <span dir="rtl">فرض بدون پشتوانه، داده superseded یا ادعای غیرقابل ردیابی</span>   |

<span dir="rtl">۱۲. محاسبه Confidence</span>

| <span dir="rtl">محاسبه</span>   | <span dir="rtl">امتیاز وزنی</span> |
|---------------------------------|------------------------------------|
| <span dir="rtl">90 × 30٪</span> | <span dir="rtl">27.00</span>       |
| <span dir="rtl">85 × 25٪</span> | <span dir="rtl">21.25</span>       |
| <span dir="rtl">88 × 20٪</span> | <span dir="rtl">17.60</span>       |
| <span dir="rtl">85 × 15٪</span> | <span dir="rtl">12.75</span>       |
| <span dir="rtl">55 × 10٪</span> | <span dir="rtl">5.50</span>        |
| <span dir="rtl">جمع</span>      | <span dir="rtl">84.10 ≈ 84</span>  |

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">نتیجه DECAF</span></p>
<p><span dir="rtl">Confidence Q1 = 84 / 100 → Class A. یعنی ساختار اصلی Current Journey برای ادامه Discovery قابل دفاع است، ولی این نمره اجازه نمی‌دهد درباره نرخ افت، Frequency مسیرها یا causal bottleneck ادعای قطعی کنیم.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl">۱۳. Cap Rules و کنترل عددسازی</span>

<span dir="rtl">• بدون Behavioral Analytics، درباره Drop-off Rate، Frequency یا سهم هر Flow در کل کاربران Confidence بالا مجاز نیست.</span>

<span dir="rtl">• Flowهایی که فقط از Expert Review آمده‌اند باید «فرضیه جریان» نامیده شوند، نه Fact.</span>

<span dir="rtl">• Survey Outcome 27/46 یا 19/46 نباید به Conversion Rate کل سایت تبدیل شود.</span>

<span dir="rtl">• اگر Evidence Family واحد چند خروجی تولید کرده باشد، در Triangulation فقط یک خانواده شمرده می‌شود.</span>

<span dir="rtl">• داده superseded یا نسخه قدیمی Dataset، Evidence Contribution صفر می‌گیرد.</span>

<span dir="rtl">۱۴. کنترل Triangulation و Double Counting</span>

<span dir="rtl">در Q1 مثلث‌سازی واقعی زمانی رخ می‌دهد که یک مرحله یا الگو از چند خانواده مستقل شواهد حمایت شود. Survey، VOC و UX Observation سه خانواده متفاوت‌اند. اما جدول، نمودار و Persona ساخته‌شده از همان Survey سه منبع مستقل محسوب نمی‌شوند.</span>

| <span dir="rtl">ادعا</span>                                         | <span dir="rtl">Evidence Families</span>                                      | <span dir="rtl">وضعیت Triangulation</span>                 |
|---------------------------------------------------------------------|-------------------------------------------------------------------------------|------------------------------------------------------------|
| <span dir="rtl">Evaluation مرحله پرسیگنال‌تری از Checkout است</span> | <span dir="rtl">Survey + UX + VOC</span>                                      | <span dir="rtl">قوی، با محدودیت نبود telemetry</span>      |
| <span dir="rtl">Confidence Check بخشی از Journey است</span>         | <span dir="rtl">Survey behavior + Never/Lapsed switching + VOC context</span> | <span dir="rtl">قوی</span>                                 |
| <span dir="rtl">Checkout بدون مشکل است</span>                       | <span dir="rtl">هیچ داده کافی برای این ادعا نداریم</span>                     | <span dir="rtl">رد ادعا؛ فقط signal فعلی ضعیف‌تر است</span> |
| <span dir="rtl">Guided Advisor راه‌حل درست است</span>                | <span dir="rtl">Q1 چنین چیزی را اثبات نمی‌کند</span>                           | <span dir="rtl">خارج از دامنه Q1</span>                    |

<span dir="rtl">۱۵. Sensitivity و Value of Information</span>

| <span dir="rtl">داده گمشده</span>                          | <span dir="rtl">Sensitivity</span> | <span dir="rtl">VOI</span>    | <span dir="rtl">چرا؟</span>                                                             |
|------------------------------------------------------------|------------------------------------|-------------------------------|-----------------------------------------------------------------------------------------|
| <span dir="rtl">Behavioral funnel / event analytics</span> | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">می‌تواند محل واقعی drop-off و وزن مراحل را تغییر دهد</span>              |
| <span dir="rtl">Observed usability sessions</span>         | <span dir="rtl">High</span>        | <span dir="rtl">High</span>   | <span dir="rtl">hesitation، backtracking و خروج واقعی را مشاهده می‌کنیم</span>           |
| <span dir="rtl">Chatbot usage rate</span>                  | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span> | <span dir="rtl">برای اهمیت Flow کمک می‌کند، نه وجود آن</span>                            |
| <span dir="rtl">Payment method share</span>                | <span dir="rtl">Low برای Q1</span> | <span dir="rtl">Low</span>    | <span dir="rtl">در Q1 ساختار Flow مهم است؛ سهم پرداخت در فصل‌های دیگر مهم‌تر می‌شود</span> |
| <span dir="rtl">Edge-case logs</span>                      | <span dir="rtl">Medium</span>      | <span dir="rtl">Medium</span> | <span dir="rtl">برای کامل‌کردن failure paths مفید است</span>                             |

<span dir="rtl">۱۶. نتیجه نهایی سؤال ۱</span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><span dir="rtl">بیان قابل دفاع برای ارائه</span></p>
<p><span dir="rtl">Current Journey خانومی از Trigger و Discovery وارد Evaluation می‌شود و بخش مهمی از تصمیم در Confidence Check بسته می‌شود؛ سپس PDP، Cart و Checkout به Transaction می‌رسند و تجربه با Fulfillment، Product Experience و Repurchase/Switching ادامه پیدا می‌کند. در شواهد فعلی، سیگنال‌های friction در Evaluation و Confidence Check پررنگ‌تر از Checkout هستند. این یک «نقشه Current State» است، نه اثبات علت ریشه‌ای و نه اثبات Guided Beauty Advisor.</span></p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<span dir="rtl">۱۷. این سؤال هنوز چه چیزی را ثابت نمی‌کند؟</span>

<span dir="rtl">• ثابت نمی‌کند Guided Beauty Decision Assistant حتماً راه‌حل درست است.</span>

<span dir="rtl">• ثابت نمی‌کند ۴۱.۳٪ کل Sessionهای خانومی خرید نمی‌کنند.</span>

<span dir="rtl">• ثابت نمی‌کند Trust یا Authenticity مهم‌ترین مسئله همه کاربران است.</span>

<span dir="rtl">• ثابت نمی‌کند Checkout هیچ مسئله‌ای ندارد؛ فقط در نمونه فعلی سیگنال ضعیف‌تری دارد.</span>

<span dir="rtl">• ثابت نمی‌کند Offline همیشه بهتر از Online است؛ فقط به‌عنوان Substitute در بخشی از Never/Lapsed دیده شده است.</span>

<span dir="rtl">۱۸. اقدام بعدی برای افزایش Confidence</span>

<span dir="rtl">بیشترین بازده اطلاعاتی برای Q1 از دو مسیر می‌آید:</span>

<span dir="rtl">• ۳ تا ۵ Usability Task مشاهده‌ای روی سناریوهای Need-based و SKU-known؛ ثبت hesitation، backtracking، external comparison و task completion.</span>

<span dir="rtl">• داده Event/Funnel در سطح Session برای Search → PLP → PDP → ATC → Checkout و در صورت امکان خروج به کانال‌های خارجی.</span>

<span dir="rtl">اگر این دو منبع با Journey فعلی هم‌راستا باشند، Confidence ساختار Flow می‌تواند افزایش یابد؛ اگر خلاف آن را نشان دهند، نقشه باید اصلاح شود. هدف DECAF دفاع از مدل فعلی نیست؛ هدف این است که مشخص کند چه داده‌ای می‌تواند آن را تغییر دهد.</span>

<span dir="rtl">۱۹. رجیستری منابع استفاده‌شده</span>

<span dir="rtl">• S1 — Survey خریداران ۱۲ ماه اخیر خانومی؛ n=46.</span>

<span dir="rtl">• S2 — Survey Never/Lapsed؛ n=28، شامل 17 Never و 11 Lapsed.</span>

<span dir="rtl">• S3 — khanoumi-comments-cleaned.csv؛ 39,737 کامنت تمیزشده و 4,023 کامنت Problem-tagged.</span>

<span dir="rtl">• S4 — khanoumi-comments.csv؛ 76,837 کامنت خام؛ برای Data Lineage.</span>

<span dir="rtl">• S5 — UX Review پروژه: Landing، Chatbot و Purchase/Checkout flow؛ expert observational evidence.</span>

<span dir="rtl">• S6 — گزارش‌های رسمی و مدیریتی خانومی؛ فقط برای context و کنترل تفسیر، نه ساخت نرخ‌های رفتاری.</span>

<span dir="rtl">نسخه روش: DECAF Quantification v1.0 \| فصل: Q1 \| وضعیت: منتخب برای استفاده در پروژه نهایی</span>
