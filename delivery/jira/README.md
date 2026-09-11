# Jira Audit — KAN

آخرین کنترل :: ۱۱ سپتامبر ۲۰۲۶  
دامنه :: Q17 Roadmap، Q18 Epics، Q19 User Stories، Q20 Two-Week Sprint Plan

## نتیجه کنترل

Jira از نظر ساختار Portfolio و داوری قابل دفاع است. پروژه شامل ۵۷ Issue است:

- ۱ Feature مرجع :: KAN-1
- ۱۲ Epic :: KAN-2 تا KAN-13
- ۴۴ Story و Task :: KAN-14 تا KAN-57
- همه Issueها در وضعیت Idea
- بدون ادعای Sprint History یا Delivery انجام‌شده

## کنترل‌های انجام‌شده

| کنترل | نتیجه |
|---|---|
| Parent برای Story و Task | ۴۴ از ۴۴ دارای Parent |
| Priority | ۵۷ از ۵۷ دارای Priority |
| Label | ۵۷ از ۵۷ دارای Label |
| Acceptance Criteria | ۴۴ از ۴۴ Story و Task |
| Definition of Done | در Issueهای اجرایی ثبت شده |
| Epic به Feature | با Issue Link نوع Relates و Reference به KAN-1 |
| Sprint Mapping | در Description Issueها ثبت شده |
| Research داخل Jira | منتقل نشده؛ Confluence Source of Truth مانده |
| Figma و Confluence | در Issueهای مرتبط لینک شده |
| وضعیت اجرا | همگی Idea؛ هیچ نتیجه یا اجرای ساختگی ثبت نشده |

## Q17 — Roadmap

- [KAN-1 — Feature و Roadmap](https://kohansal.atlassian.net/browse/KAN-1)
- [Q17 canonical document](../../docs/questions/q17/)

Roadmap به‌صورت Gate-based تعریف شده است:

**Demand Validation → Concierge / Wizard-of-Oz → Rule-based MVP → Controlled Pilot → Scale / Iterate / Stop**

تاریخ و Capacity ساختگی وارد نشده است.

## Q18 — Epics

| بازه | اولویت | Epicها |
|---|---|---|
| MVP Core | P0 | KAN-2 تا KAN-7 |
| Pilot و Improvement | P1 | KAN-8 تا KAN-10 |
| Post-validation | P2 | KAN-11 تا KAN-13 |

- [Q18 canonical document](../../docs/questions/q18/)
- [KAN-2](https://kohansal.atlassian.net/browse/KAN-2) تا [KAN-13](https://kohansal.atlassian.net/browse/KAN-13)

به‌علت Hierarchy پروژه Team-managed، Epicها Parent مستقیم Feature نیستند و با Issue Link نوع Relates به KAN-1 متصل‌اند.

## Q19 — User Stories و Tasks

- [Q19 canonical document](../../docs/questions/q19/)
- [KAN-14](https://kohansal.atlassian.net/browse/KAN-14) تا [KAN-57](https://kohansal.atlassian.net/browse/KAN-57)

هر Issue اجرایی شامل این اجزاست:

- User Value یا Technical Goal
- Acceptance Criteria
- Dependency
- Sprint Mapping یا Backlog
- لینک‌های مرجع
- Definition of Done
- Priority، Label و Parent

## Q20 — Two-Week Sprint Plan

| Sprint | Goal |
|---|---|
| Sprint 1 | Demand Validation و Measurement Foundation |
| Sprint 2 | Question Flow و Concierge MVP |
| Sprint 3 | Rule-based Recommendation، Explainability و Alternative |
| Sprint 4 | PDP و Cart Handoff، Attribution و Controlled Pilot |
| Sprint 5 | Evaluation، Guardrail Review و Scale Decision |

- [Q20 canonical document](../../docs/questions/q20/)

Board فعلی Kanban است؛ بنابراین Sprintها به‌عنوان **برنامه دوهفته‌ای پیشنهادی** در Description ثبت شده‌اند، نه Sprint Object یا تاریخچه واقعی.

## Story Point و Capacity

Story Point روی Issueهای فعلی فعال یا ثبت نشده است و Capacity تیم واقعی نیز در داده پروژه وجود ندارد. برای جلوگیری از Precision ساختگی:

- Priority و Sprint Mapping ثبت شده‌اند
- Estimate عددی جعل نشده است
- Story Point باید در Refinement با تیم اجرا تعیین شود
- Sprint Commitment فقط پس از مشخص‌شدن Capacity معتبر است

این Caveat ضعف ساختار نیست؛ مرز بین Planning و Execution واقعی را حفظ می‌کند.

## اتصال به Design و GitHub

- [Prototype تعاملی](../../design/prototype/index.html)
- [مستند Prototype](../../design/prototype/)
- [Figma V2](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl)
- [FigJam](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3)
- [Repository](https://github.com/kohansall/khanoumi-product-decision-system)
- [Confluence START HERE](https://kohansal.atlassian.net/wiki/spaces/PM/pages/8028163)

## نتیجه نهایی

ساختار Jira برای پاسخ Q17 تا Q20 کامل است. اقدام بعدی Jira تنها زمانی لازم می‌شود که تیم واقعی وارد Delivery شود و Sprint، Assignee، Capacity، Story Point و تاریخ اجرا مشخص شوند.
