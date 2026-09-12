# سیستم تصمیم‌گیری محصول خانومی

پروژه نهایی بوتکمپ مدیریت محصول، بازطراحی‌شده به‌عنوان یک Case Study قابل ممیزی و Portfolio-ready.

> وضعیت تصمیم :: **Guided Beauty Decision Assistant — Selected for Validation**  
> این Feature هنوز Validation‌شده نیست. شواهد فعلی Opportunity را پشتیبانی می‌کنند، نه موفقیت قطعی راه‌حل را.
>
> مقیاس VOC :: **۷۶٬۸۳۷ کامنت خام Crawl‌شده → ۳۹٬۷۳۷ رکورد Cleaned و Canonical**  
> این اعداد تعداد کامنت‌اند، نه تعداد کاربر. کاهش تعداد نتیجه کنترل Lineage، پاک‌سازی و Deduplication است.

## فهرست اصلی

- [مسئله و فرصت](#مسئله-و-فرصت)
- [Feature و مسیر MVP](#feature-و-مسیر-mvp)
- [دسترسی سریع](#دسترسی-سریع)
- [فهرست مرکزی لینک‌ها](#فهرست-مرکزی-لینکها)
- [معماری Evidence](#معماری-evidence)
- [DECAF](#decaf)
- [نقش ابزارها](#نقش-ابزارها)
- [نقشه ۳۰ سؤال](#نقشه-۳۰-سؤال)
- [محدودیت مهم](#محدودیت-مهم)

## مسئله و فرصت

شواهد چندمنبعی نشان می‌دهند Delivery در داده فعلی Root Problem اصلی نیست. سیگنال قوی‌تر به دشواری ارزیابی Fit محصول، پراکندگی اطلاعات و پایین‌بودن Decision Confidence مربوط است. Opportunity منتخب، کاهش effort و عدم‌قطعیت انتخاب محصول با یک مسیر هدایت‌شده، کوتاه، توضیح‌پذیر و متصل به موجودی واقعی است.

## Feature و مسیر MVP

**Fake Door → Concierge / Wizard-of-Oz → Rule-based MVP → Controlled Pilot**

هر مرحله Gate دارد. AI خود Feature نیست و فقط پس از اثبات ارزش Feature می‌تواند به‌عنوان روش پیاده‌سازی بررسی شود.

## دسترسی سریع

- [Easy Access :: فهرست کامل لینک‌های پروژه](EASY-ACCESS.md)
- [Prototype تعاملی](design/prototype/index.html)
- [VOC dashboard](discovery/voc/interactive-dashboard/)
- [VOC cleaned canonical dataset](discovery/voc/cleaned/)
- [فهرست Q01 تا Q30](docs/questions/)
- [Final report](docs/final-report/)
- [Final presentation :: HTML canonical](presentation/final-deck/index.html)
- [Jira project KAN](https://kohansal.atlassian.net/jira/software/projects/KAN)
- [Confluence START HERE](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8028163)
- [Figma V2](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl)
- [FigJam — نقشه تصمیم](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3)

## فهرست مرکزی لینک‌ها

این فهرست مسیر مستقیم تمام بخش‌های پروژه را براساس ترتیب Q01 تا Q30 ارائه می‌کند.

### لینک‌های اصلی پروژه

| مقصد | لینک |
|---|---|
| GitHub Repository | [مشاهده پروژه](https://github.com/kohansall/khanoumi-product-decision-system) |
| Confluence Main Page | [مشاهده صفحه اصلی](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8028163) |
| Confluence Submission Hub | [مشاهده Submission Hub](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8749057) |
| Confluence 30-Question Index | [مشاهده فهرست سؤالات](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8814593) |
| Confluence Jira Mapping | [مشاهده Jira Mapping](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8781825) |
| Jira Project KAN | [مشاهده پروژه Jira](https://kohansal.atlassian.net/jira/software/projects/KAN/issues) |
| Figma Design | [مشاهده طراحی](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl) |
| FigJam Board | [مشاهده FigJam](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3) |
| Interactive Prototype | [مشاهده Prototype](design/prototype/index.html) |
| VOC Dashboard | [مشاهده داشبورد VOC](discovery/voc/interactive-dashboard/index.html) |
| Survey Results | [مشاهده خروجی تعاملی دو Survey](discovery/user-research/surveys/survey-results-interactive.html) |
| Final Presentation | [مشاهده ارائه تعاملی نهایی](presentation/final-deck/index.html) |
| Final Audit Report | [مشاهده گزارش Audit](docs/final-report/audit-report.md) |

### Discovery و Problem Definition

| سؤال | موضوع | پاسخ اصلی | Artifact موضوعی |
|---|---|---|---|
| Q01 | جریان فعلی کاربر | [مشاهده Q01](docs/questions/q01/) | [Discovery Overview](discovery/overview/) |
| Q02 | کشف مسئله | [مشاهده Q02](docs/questions/q02/) | [Problem Synthesis](discovery/problem-synthesis/) |
| Q03 | اعتبارسنجی و اولویت‌بندی مسئله | [مشاهده Q03](docs/questions/q03/) | [Problem Synthesis](discovery/problem-synthesis/) |
| Q04 | نیازهای مشترک کاربران | [مشاهده Q04](docs/questions/q04/) | [User Research Synthesis](discovery/user-research/synthesis/) |

### Competitor و Market Research

| سؤال | موضوع | پاسخ اصلی | Artifact موضوعی |
|---|---|---|---|
| Q05 | مجموعه رقبا | [مشاهده Q05](docs/questions/q05/) | [Competitor Analysis](discovery/competitors/) |
| Q06 | مقایسه قابلیت رقبا | [مشاهده Q06](docs/questions/q06/) | [Competitor Analysis](discovery/competitors/) |
| Q07 | الگوهای رهبران جهانی | [مشاهده Q07](docs/questions/q07/) | [Market Research](discovery/market/) |
| Q08 | روندهای بازار | [مشاهده Q08](docs/questions/q08/) | [Market Research](discovery/market/) |
| Q09 | سنتز فرصت‌ها | [مشاهده Q09](docs/questions/q09/) | [Opportunity](discovery/opportunity/) |

### Solution و MVP

| سؤال | موضوع | پاسخ اصلی | Artifact موضوعی |
|---|---|---|---|
| Q10 | انتخاب Feature | [مشاهده Q10](docs/questions/q10/) | [Feature Selection](solution/feature-selection/) |
| Q11 | Pain و نیاز بازار | [مشاهده Q11](docs/questions/q11/) | [Feature Selection](solution/feature-selection/) |
| Q12 | منطق Evidence تا Decision | [مشاهده Q12](docs/questions/q12/) | [Feature Selection](solution/feature-selection/) |
| Q13 | اثر مورد انتظار | [مشاهده Q13](docs/questions/q13/) | [Solution](solution/) |
| Q14 | چرایی ارزش آزمون | [مشاهده Q14](docs/questions/q14/) | [Validation](solution/validation/) |
| Q15 | تعریف MVP | [مشاهده Q15](docs/questions/q15/) | [MVP](solution/mvp/) |
| Q16 | قابلیت‌های اصلی MVP | [مشاهده Q16](docs/questions/q16/) | [MVP](solution/mvp/) |

### Delivery و Jira

| سؤال | موضوع | پاسخ اصلی | GitHub Artifact | Jira |
|---|---|---|---|---|
| Q17 | Roadmap | [مشاهده Q17](docs/questions/q17/) | [Roadmap](delivery/roadmap/) | [KAN-1](https://kohansal.atlassian.net/browse/KAN-1) |
| Q18 | Epics | [مشاهده Q18](docs/questions/q18/) | [Epic Mapping](delivery/epics/) | [KAN-2 تا KAN-13](delivery/jira/) |
| Q19 | User Stories | [مشاهده Q19](docs/questions/q19/) | [User Stories](delivery/user-stories/) | [KAN-14 تا KAN-57](delivery/jira/) |
| Q20 | برنامه اسپرینت دوهفته‌ای | [مشاهده Q20](docs/questions/q20/) | [Sprint Plan](delivery/sprint-plan/) | [Jira Mapping](delivery/jira/) |

> Q18، Q19 و Q20 Artifact اجرایی هستند؛ بنابراین برای آن‌ها Confidence پژوهشی DECAF تولید نشده است. Sprint Plan نیز برنامه پیشنهادی است، نه Sprint History واقعی.

### Measurement

| سؤال | موضوع | پاسخ اصلی | Artifact موضوعی |
|---|---|---|---|
| Q21 | KPIها | [مشاهده Q21](docs/questions/q21/) | [KPIs](measurement/kpis/) و [Success Metrics](measurement/success-metrics/) |
| Q22 | Success Metrics و Guardrails | [مشاهده Q22](docs/questions/q22/) | [Guardrails](measurement/guardrails/) |

### Design و Prototype

| سؤال | موضوع | پاسخ اصلی | Design Artifact |
|---|---|---|---|
| Q23 | سفر جدید کاربر | [مشاهده Q23](docs/questions/q23/) | [User Journey](design/user-journey/) |
| Q24 | Low-Fidelity Wireframes | [مشاهده Q24](docs/questions/q24/) | [Low-Fi](design/low-fi/)، [Prototype](design/prototype/index.html)، [Figma](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl) و [FigJam](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3) |

> Q23 و Q24 Artifact طراحی هستند؛ بنابراین برای آن‌ها Confidence پژوهشی DECAF تولید نشده است.

### Business Impact

| سؤال | موضوع | پاسخ اصلی | Artifact موضوعی |
|---|---|---|---|
| Q25 | Acquisition | [مشاهده Q25](docs/questions/q25/) | [Acquisition](business/acquisition/) |
| Q26 | Retention | [مشاهده Q26](docs/questions/q26/) | [Retention](business/retention/) |
| Q27 | مدل هزینه | [مشاهده Q27](docs/questions/q27/) | [Cost Model](business/cost-model/) |
| Q28 | پیش‌بینی درآمد | [مشاهده Q28](docs/questions/q28/) | [Revenue Forecast](business/revenue-forecast/) |
| Q29 | ROI و Payback | [مشاهده Q29](docs/questions/q29/) | [ROI and Payback](business/roi-payback/) |

### Final Submission

| سؤال | موضوع | پاسخ اصلی | خروجی نهایی |
|---|---|---|---|
| Q30 | یکپارچه‌سازی و ارائه نهایی | [مشاهده Q30](docs/questions/q30/) | [Final Report](docs/final-report/) و [Final Presentation](presentation/final-deck/index.html) |

### داده‌ها و Evidence

| بخش | لینک |
|---|---|
| VOC Overview | [مشاهده VOC](discovery/voc/) |
| Raw Anonymized VOC | [مشاهده داده خام](discovery/voc/raw/) |
| Cleaned VOC | [مشاهده داده پاک‌سازی‌شده](discovery/voc/cleaned/) |
| VOC Analysis | [مشاهده تحلیل VOC](discovery/voc/analysis/) |
| VOC Interactive Dashboard | [مشاهده Dashboard](discovery/voc/interactive-dashboard/index.html) |
| User Interviews | [مشاهده مصاحبه‌ها](discovery/user-research/interviews/) |
| Surveys | [مشاهده نظرسنجی‌ها](discovery/user-research/surveys/) |
| Personas | [مشاهده پرسوناها](discovery/user-research/personas/) |
| UX Review | [مشاهده UX Review](discovery/ux-review/) |
| Competitor Benchmark | [مشاهده Benchmark](discovery/competitors/) |
| Market Research | [مشاهده تحقیقات بازار](discovery/market/) |
| Visual Maps | [مشاهده نقشه‌ها](design/visual-maps/) |
| Source Register | [مشاهده فهرست منابع](sources/source-register/) |
| Official Reports Register | [مشاهده منابع رسمی](sources/official-reports/) |
| External Research Register | [مشاهده تحقیقات بیرونی](sources/external-research/) |

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
