**سؤال 19 — User Storyها و اولویت‌بندی**

**تبدیل Epicها به رفتارهای قابل ساخت و تست**

نسخه مستقل و قابل ارائه \| مبتنی بر Evidence Base پروژه خانومی

**نمره دفاع‌پذیری فعلی: 95 از ۱۰۰**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>صورت سؤال دقیق بوتکمپ<br />
</strong>«فیچر پیشنهادی را به اپیک (Epic) و داستان‌های کاربر (User Stories) خرد و اولویت‌بندی کنید.»</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

منبع: پروژه پایانی بوتکمپ مدیریت محصول آکادمی همراه، گام هفتم.

**توضیح هاند**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>توضیح برای سگ شکاری<br />
</strong>Epic می‌گه «بخش سؤال‌ها». User Story می‌گه «منِ کاربر می‌خوام جواب قبلیم رو عوض کنم تا recommendation اشتباه نشه». یعنی هر تکه بزرگ رو تبدیل می‌کنیم به کار مشخص.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**استوری‌لاین**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Story Format<br />
</strong>به‌عنوان [کاربر] می‌خواهم [کار] تا بتوانم [ارزش] — سپس Acceptance Criteria.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

| **ID** | **User Story**                                                                                                 | **Priority** |
|--------|----------------------------------------------------------------------------------------------------------------|--------------|
| US1    | به‌عنوان کاربر مردد می‌خواهم از Search/Category وارد راهنمای انتخاب شوم تا مجبور نباشم بین همه محصولات بگردم.    | P0           |
| US2    | می‌خواهم Need اصلی‌ام را انتخاب کنم تا سؤال‌های نامرتبط نبینم.                                                    | P0           |
| US3    | می‌خواهم فقط چند سؤال کوتاه پاسخ دهم تا سریع به نتیجه برسم.                                                     | P0           |
| US4    | می‌خواهم جواب قبلی را ویرایش کنم تا نتیجه بر اساس اطلاعات درست باشد.                                            | P1           |
| US5    | می‌خواهم حداکثر سه پیشنهاد ببینم تا overload نشوم.                                                              | P0           |
| US6    | می‌خواهم بدانم چرا هر محصول پیشنهاد شده تا بتوانم به نتیجه اعتماد کنم.                                          | P0           |
| US7    | می‌خواهم قیمت/موجودی پیشنهاد را ببینم تا گزینه غیرقابل خرید نگیرم.                                              | P0           |
| US8    | می‌خواهم جایگزین ببینم تا اگر گزینه اول مناسب نبود تصمیمم متوقف نشود.                                           | P0           |
| US9    | می‌خواهم مستقیماً وارد PDP شوم تا خرید را ادامه دهم.                                                             | P0           |
| US10   | می‌خواهم بگویم پیشنهاد مفید نبود تا سیستم از feedback یاد بگیرد.                                                | P1           |
| US11   | می‌خواهم بدون استفاده از Advisor به مسیر عادی برگردم تا کنترل دست خودم بماند.                                   | P0           |
| US12   | به‌عنوان تیم محصول می‌خواهم exposure/start/completion/click/cart/purchase را track کنم تا اثر Feature را بسنجیم. | P0           |
| US13   | به‌عنوان تیم محصول می‌خواهم recommendationهای unsafe/medical claim مسدود شوند تا ریسک کاربر کم شود.              | P0           |
| US14   | می‌خواهم preferenceهایم در آینده ذخیره شود تا دفعه بعد سریع‌تر انتخاب کنم.                                       | P2           |

**نمونه Acceptance Criteria**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>US5 — Shortlist<br />
</strong>Given کاربر flow را کامل کرده است، When نتیجه تولید می‌شود، Then حداکثر ۳ SKU موجود نمایش داده شود؛ هر SKU عنوان، قیمت، دلیل پیشنهاد و CTA PDP داشته باشد.</th>
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
<th><strong>US12 — Tracking<br />
</strong>برای هر eligible exposure، start، answer step، completion، recommendation impression، click، add-to-cart و purchase event ثبت شود و session/user attribution در حد privacy policy موجود حفظ شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**اولویت‌بندی**

P0 = ضروری برای hypothesis/safety/measurement؛ P1 = learning/usability؛ P2 = retention/scale.

**نریتیو ارائه**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Talk Track<br />
</strong>«User Storyها را بر اساس value و testability اولویت دادیم. P0ها فقط چیزهایی هستند که بدون آنها core hypothesis، measurement یا safety ناقص می‌شود. Memory و personalization دائمی را عمداً P2 گذاشتیم تا MVP بزرگ نشود.»</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Audit و نمره**

**نمره فعلی: ۹۵ از ۱۰۰**

• Storyها behavior-based و testable هستند.

• کمبود: technical acceptance criteria دقیق پس از شناخت API/catalog schema نهایی می‌شود.

**رفرنس‌ها**

• پروژه پایانی بوتکمپ مدیریت محصول آکادمی همراه — صورت سؤال رسمی.

• Survey خریداران ۱۲ ماه اخیر خانومی — n=46.

• Survey Never/Lapsed — n=28.

• khanoumi-comments-cleaned.csv — 39,737 کامنت Cleaned.

• مصاحبه‌های عمیق کاربران پروژه خانومی.

• گزارش مدیر محصول — Product Data Gap، recommendation usage، friction خرید و KPIهای داخلی.

• گزارش مدیرعامل — جهت‌گیری profitability/efficiency/resilience و context بیزینس.

• UX Review پروژه خانومی — Landing، Chatbot و Purchase Flow.

• گزارش رسمی خانومی ۱۴۰۴ — metrics رشد، بازگشت، NPS، OTD، Return Rate و BNPL.

• Benchmark پروژه — Sephora، Ulta، Nykaa و نمونه‌های داخلی؛ برای mechanism/context.

نسخه: شهریور ۱۴۰۵
