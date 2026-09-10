**سؤال 20 — اسپرینت‌های دوهفته‌ای و Jira Plan**

**تبدیل Backlog به برنامه اجرایی Delivery**

نسخه مستقل و قابل ارائه \| مبتنی بر Evidence Base پروژه خانومی

**نمره دفاع‌پذیری فعلی: 91 از ۱۰۰**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>صورت سؤال دقیق بوتکمپ<br />
</strong>«اپیک‌ها و استوری‌های خود را در قالب اسپرینت‌های دوهفته‌ای در جیرا پیاده‌سازی کنید. از نکات مطرح‌شده در بوتکمپ برای ایجاد یوزر استوری استفاده کنید.»</th>
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
</strong>حالا می‌گیم تیم در هر دو هفته دقیقاً چی بسازه. اول tracking و Fake Door، بعد سؤال‌ها، بعد recommendation، بعد نتیجه، بعد Pilot. کارهای تزئینی رو نمی‌ریزیم اول.</th>
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
<th><strong>Sprint Principle<br />
</strong>Measurement first → Core flow → Recommendation → Commerce bridge → Pilot → Hardening</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Sprint 0 — Setup / Discovery Tech**

• Event taxonomy و analytics plan

• Category/data readiness audit

• Jira epics + story mapping

• Experiment design و baseline definition

• Safety constraints

**Sprint 1 — Fake Door & Demand**

• E1 Entry CTA

• Eligible exposure tracking

• Start event

• Simple landing/form shell

• Dashboard اولیه Demand

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Sprint Goal<br />
</strong>بفهمیم آیا کاربران eligible اصلاً برای Guidance اقدام می‌کنند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Sprint 2 — Need Capture & Questions**

• E2 Need Capture

• E3 4–6 short questions

• Back/edit

• Completion tracking

• Basic accessibility/UX

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Sprint Goal<br />
</strong>کاربر flow را کوتاه و بدون friction غیرضروری کامل کند.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Sprint 3 — Recommendation Logic**

• E4 rule/manual recommendation logic

• In-stock constraint

• Data mapping

• Safety filters

• Test fixtures

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Sprint Goal<br />
</strong>برای input معتبر، shortlist قابل توضیح و قابل خرید تولید شود.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Sprint 4 — Result & Commerce**

• E5 Result Page

• Why-this-product

• Alternative

• E6 PDP bridge

• Recommendation click + add-to-cart tracking

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Sprint Goal<br />
</strong>کاربر از recommendation به تصمیم و commerce flow برسد.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Sprint 5 — Pilot & Experiment**

• Traffic ramp محدود

• Control/Test در صورت امکان

• Funnel analysis

• User feedback

• Bug/safety triage

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Sprint Goal<br />
</strong>اثر رفتاری و guardrail را قبل از scale بسنجیم.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Sprint 6 — Iterate / Launch Readiness**

• Fix highest-severity friction

• Data quality improvements

• Performance/reliability

• Operational runbook

• Launch/kill decision

**Jira Structure**

| **سطح**  | **نمونه**                                 |
|----------|-------------------------------------------|
| Epic     | E4 Recommendation Logic                   |
| Story    | US7 نمایش فقط SKU موجود                   |
| Task     | Map inventory field / rule implementation |
| Sub-task | Unit tests / analytics event / QA case    |

**Definition of Ready**

• User value روشن

• Acceptance criteria نوشته شده

• Dependency مشخص

• Analytics event مشخص

• Safety/edge case مشخص

**Definition of Done**

• Code/design complete

• QA pass

• Analytics verified

• Acceptance criteria pass

• No critical safety issue

• Release note/documentation

**نریتیو ارائه**

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Talk Track<br />
</strong>«Delivery را در شش Sprint دوهفته‌ای چیدیم. Sprint صفر data/measurement و constraints را آماده می‌کند. Sprint یک Demand را با Fake Door می‌سنجد. بعد flow، recommendation و result/commerce ساخته می‌شوند. Sprint پنج Pilot است و Sprint شش فقط اگر evidence مثبت باشد hardening و launch readiness را انجام می‌دهد.»</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Audit و نمره**

**نمره فعلی: ۹۱ از ۱۰۰**

• Sprintها به Roadmap و Epics trace می‌شوند.

• کمبود: velocity/capacity تیم و Jira واقعی خانومی در دسترس نیست؛ این برنامه planning baseline است.

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

• محتوای دوره توسعه محصول با اسکرام — اصول User Story، Sprint و Jira backlog.

نسخه: شهریور ۱۴۰۵
