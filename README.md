# سیستم تصمیم‌گیری محصول خانومی

پروژه نهایی بوتکمپ مدیریت محصول، بازطراحی‌شده به‌عنوان یک Case Study قابل ممیزی و Portfolio-ready.

> وضعیت تصمیم :: **Guided Beauty Decision Assistant — Selected for Validation**  
> این Feature هنوز Validation‌شده نیست. شواهد فعلی Opportunity را پشتیبانی می‌کنند، نه موفقیت قطعی راه‌حل را.

## مسئله و فرصت

شواهد چندمنبعی نشان می‌دهند Delivery در داده فعلی Root Problem اصلی نیست. سیگنال قوی‌تر به دشواری ارزیابی Fit محصول، پراکندگی اطلاعات و پایین‌بودن Decision Confidence مربوط است. Opportunity منتخب، کاهش effort و عدم‌قطعیت انتخاب محصول با یک مسیر هدایت‌شده، کوتاه، توضیح‌پذیر و متصل به موجودی واقعی است.

## Feature و مسیر MVP

**Fake Door → Concierge / Wizard-of-Oz → Rule-based MVP → Controlled Pilot**

هر مرحله Gate دارد. AI خود Feature نیست و فقط پس از اثبات ارزش Feature می‌تواند به‌عنوان روش پیاده‌سازی بررسی شود.

## دسترسی سریع

- [Prototype تعاملی](design/prototype/index.html)
- [VOC dashboard](discovery/voc/interactive-dashboard/)
- [VOC cleaned canonical dataset](discovery/voc/cleaned/)
- [فهرست Q01 تا Q30](docs/questions/)
- [Final report](docs/final-report/)
- [Final presentation](presentation/final-deck/khanoumi-final-presentation-fa.pptx)
- [Jira project KAN](https://kohansal.atlassian.net/jira/software/projects/KAN)
- [Confluence START HERE](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8028163)
- [Figma V2](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl)
- [FigJam — نقشه تصمیم](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3)

## معماری Evidence

`raw → cleaned → analysis → synthesis → decision → delivery → measurement`

یک Dataset فقط یک مالک canonical دارد. بخش‌های دیگر با لینک داخلی به آن ارجاع می‌دهند. هر Claim تحلیلی باید یکی از این چهار برچسب را داشته باشد :: **Fact · Evidence · Logical Inference · Hypothesis**.

## DECAF

DECAF در این پروژه یک روش اختصاصی برای Decision Confidence است، نه یک استاندارد جهانی و نه احتمال آماری موفقیت.

| کلاس | معنای استفاده |
|---|---|
| A | قابل پذیرش و دفاع؛ شواهد چندمنبعی و Caveat کنترل‌شده |
| B | قابل استفاده با Caveat؛ تصمیم ممکن است اما Missing Data مهم است |
| C | جهت‌نما؛ فقط Scenario یا Hypothesis، نه ادعای قطعی |
| D | ناکافی برای تصمیم |

Cap Rule و کنترل Double Counting مانع بالا رفتن مصنوعی Confidence می‌شوند. برای Q18، Q19، Q20، Q23 و Q24 Confidence پژوهشی ساخته نشده، چون Artifact اجرایی یا طراحی‌اند.

## نقش ابزارها

| سیستم | Source of Truth |
|---|---|
| Confluence | Evidence، تحلیل، تصمیم و Caveat |
| GitHub | Artifactها، داده‌های نهایی، خروجی خواندنی و Versioning |
| Jira | Delivery برای Q17 تا Q20 |
| Figma | Design، Journey، Low-fi و Prototype design |

## نقشه ۳۰ سؤال

| سؤال | موضوع | DECAF Confidence |
|---|---|---|
| [Q01](docs/questions/q01/) | جریان فعلی کاربر | 84/100 — A |
| [Q02](docs/questions/q02/) | کشف مسئله | 92/100 — A |
| [Q03](docs/questions/q03/) | اعتبارسنجی و اولویت‌بندی مسئله | 89/100 — A |
| [Q04](docs/questions/q04/) | نیازهای مشترک کاربران | 89/100 — A |
| [Q05](docs/questions/q05/) | مجموعه رقبا | 93/100 — A |
| [Q06](docs/questions/q06/) | مقایسه قابلیت رقبا | 89/100 — A |
| [Q07](docs/questions/q07/) | الگوهای رهبران جهانی | 92/100 — A |
| [Q08](docs/questions/q08/) | روندهای بازار | 88/100 — A |
| [Q09](docs/questions/q09/) | سنتز فرصت‌ها | 91/100 — A |
| [Q10](docs/questions/q10/) | انتخاب Feature | 72/100 — B |
| [Q11](docs/questions/q11/) | Pain و نیاز بازار | 88/100 — A |
| [Q12](docs/questions/q12/) | منطق Evidence تا Decision | 87/100 — A |
| [Q13](docs/questions/q13/) | اثر مورد انتظار | 78/100 — B |
| [Q14](docs/questions/q14/) | چرایی ارزش آزمون | 78/100 — B |
| [Q15](docs/questions/q15/) | تعریف MVP | 94/100 — A |
| [Q16](docs/questions/q16/) | قابلیت‌های اصلی MVP | 93/100 — A |
| [Q17](docs/questions/q17/) | Roadmap | 78/100 — B |
| [Q18](docs/questions/q18/) | Epics | — اجرایی/طراحی |
| [Q19](docs/questions/q19/) | User Stories | — اجرایی/طراحی |
| [Q20](docs/questions/q20/) | برنامه اسپرینت دوهفته‌ای | — اجرایی/طراحی |
| [Q21](docs/questions/q21/) | KPIها | 86/100 — A |
| [Q22](docs/questions/q22/) | Success Metrics و Guardrails | 74/100 — B |
| [Q23](docs/questions/q23/) | سفر جدید کاربر | — اجرایی/طراحی |
| [Q24](docs/questions/q24/) | Low-Fidelity Wireframes | — اجرایی/طراحی |
| [Q25](docs/questions/q25/) | Acquisition | 68/100 — B |
| [Q26](docs/questions/q26/) | Retention | 66/100 — B |
| [Q27](docs/questions/q27/) | مدل هزینه | 58/100 — C |
| [Q28](docs/questions/q28/) | پیش‌بینی درآمد | 49/100 — C |
| [Q29](docs/questions/q29/) | ROI و Payback | 45/100 — C |
| [Q30](docs/questions/q30/) | یکپارچه‌سازی و ارائه نهایی | 79/100 — B |

## محدودیت مهم

این Repo شامل Validation ساختگی، Sprint history ساختگی یا Forecast تک‌عددی بدون baseline نیست. Gapها در [Final audit](docs/final-report/audit-report.md) ثبت شده‌اند.
