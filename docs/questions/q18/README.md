**سؤال 18 — Epicهای Feature**

**شکستن Guided Decision Assistant به بلوک‌های قابل تحویل**

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
</strong>Feature بزرگه. برای اینکه تیم بتونه بسازتش، خردش می‌کنیم به چند تکه بزرگ: شروع، سؤال‌ها، recommendation، نتیجه، tracking و safety.</th>
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
<th><strong>Decomposition<br />
</strong>Feature → Epics → Stories → Acceptance Criteria → Sprint</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

| **Epic**                         | **هدف**                                                                       | **اولویت** |
|----------------------------------|-------------------------------------------------------------------------------|------------|
| E1 — Entry & Eligibility         | نمایش CTA در context مناسب و تعیین اینکه کدام user/session eligible است.      | P0         |
| E2 — Need Capture                | گرفتن Need/Concern و constraints اصلی کاربر.                                  | P0         |
| E3 — Question Flow               | سؤال‌های کوتاه و progressive با امکان back/edit.                               | P0         |
| E4 — Recommendation Logic        | تبدیل input به shortlist محدود از SKUهای موجود.                               | P0         |
| E5 — Recommendation Result       | نمایش ۳ پیشنهاد، explanation و alternative.                                   | P0         |
| E6 — Commerce Bridge             | اتصال نتیجه به PDP/Cart و reuse مسیر خرید فعلی.                               | P0         |
| E7 — Analytics & Experimentation | event taxonomy، funnel، control/test و dashboard.                             | P0         |
| E8 — Feedback & Learning         | ثبت usefulness / mismatch برای iteration.                                     | P1         |
| E9 — Safety & Governance         | guardrail برای claims، ingredient contraindicationهای شناخته‌شده و escalation. | P0         |
| E10 — Personalization Memory     | ذخیره preference و reuse در جلسات بعدی.                                       | P2         |

**منطق اولویت‌بندی**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>P0<br />
</strong>بدون آن core hypothesis یا safety/measurement قابل تست نیست.</th>
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
<th><strong>P1<br />
</strong>برای learning و usability مهم است، اما Fake Door/Concierge بدون آن هم قابل اجراست.</th>
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
<th><strong>P2<br />
</strong>ارزش Scale/Retention دارد ولی برای MVP ضروری نیست.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Definition of Done سطح Epic**

• Outcome مشخص

• Event tracking مشخص

• Acceptance criteria قابل تست

• Owner و dependency مشخص

• Guardrail مرتبط مشخص

**نریتیو ارائه**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Talk Track<br />
</strong>«Feature را به ۱۰ Epic شکستیم. هفت Epic هسته تجربه و measurement را می‌سازند، Safety هم P0 است، Feedback P1 و Memory P2. این یعنی roadmap از همان ابتدا analytics و safety را کنار UI می‌سازد، نه بعد از launch.»</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Audit و نمره**

**نمره فعلی: ۹۵ از ۱۰۰**

• Epics outcome-oriented و قابل نگاشت به MVP هستند.

• کمبود: dependencyهای backend واقعی خانومی هنوز باید با تیم فنی confirm شوند.

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
