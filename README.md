# سیستم تصمیم‌گیری محصول خانومی

پروژه نهایی بوتکمپ مدیریت محصول آکادمی همراه — کیس «خانومی».

## تز اصلی

**مسئله اصلی:** عدم اطمینان در تصمیم پیش از خرید  
**فرصت منتخب:** کاهش Decision Uncertainty  
**Feature Candidate:** Guided Beauty Decision Assistant  
**وضعیت:** Selected for Validation — نه Validated Solution  
**مسیر MVP:** Fake Door → Concierge / Wizard-of-Oz → Rule-based MVP → Pilot → Scale Decision

## معماری مخزن

```text
.
├── docs/questions/        # Q01 تا Q30
├── research/              # شواهد و قواعد تحقیق
├── methodology/           # DECAF و Quantification
├── design/                # Figma و FigJam
├── delivery/              # Jira و Traceability
├── financial/             # Q27 تا Q29
└── presentation/          # روایت ارائه نهایی
```

## ۳۰ سؤال

- [Q01 — جریان‌های فعلی کاربر](docs/questions/Q01.md) — 84/A
- [Q02 — کشف مشکلات](docs/questions/Q02.md) — 92/A
- [Q03 — اعتبارسنجی و اولویت‌بندی](docs/questions/Q03.md) — 89/A
- [Q04 — نیازهای مشترک](docs/questions/Q04.md) — 89/A
- [Q05 — رقبا](docs/questions/Q05.md) — 93/A
- [Q06 — مقایسه قابلیت رقبا](docs/questions/Q06.md) — 89/A
- [Q07 — رهبران جهانی](docs/questions/Q07.md) — 92/A
- [Q08 — روندهای جهانی](docs/questions/Q08.md) — 88/A
- [Q09 — فضای فرصت](docs/questions/Q09.md) — 91/A
- [Q10 — انتخاب Feature](docs/questions/Q10.md) — 72/B
- [Q11 — درد و نیاز بازار](docs/questions/Q11.md) — 88/A
- [Q12 — منطق شواهد تا تصمیم](docs/questions/Q12.md) — 87/A
- [Q13 — اثر مورد انتظار](docs/questions/Q13.md) — 78/B
- [Q14 — چرا ارزش تست دارد](docs/questions/Q14.md) — 78/B
- [Q15 — دامنه MVP](docs/questions/Q15.md) — 94/A
- [Q16 — قابلیت‌های MVP](docs/questions/Q16.md) — 93/A
- [Q17 — Roadmap](docs/questions/Q17.md) — 78/B
- [Q18 — Epics](docs/questions/Q18.md) — Artifact
- [Q19 — User Stories](docs/questions/Q19.md) — Artifact
- [Q20 — Sprint Plan](docs/questions/Q20.md) — Artifact
- [Q21 — KPIها](docs/questions/Q21.md) — 86/A
- [Q22 — Success Metrics & Guardrails](docs/questions/Q22.md) — 74/B
- [Q23 — User Journey](docs/questions/Q23.md) — Artifact
- [Q24 — Low-Fidelity](docs/questions/Q24.md) — Artifact
- [Q25 — Acquisition](docs/questions/Q25.md) — 68/B
- [Q26 — Retention](docs/questions/Q26.md) — 66/B
- [Q27 — Cost Model](docs/questions/Q27.md) — 58/C
- [Q28 — Revenue Forecast](docs/questions/Q28.md) — 49/C
- [Q29 — ROI / Payback](docs/questions/Q29.md) — 45/C
- [Q30 — Final Integration](docs/questions/Q30.md) — 79/B

## سیستم‌های اصلی

- Confluence: https://kohansal.atlassian.net/wiki/spaces/PM/pages/8028163
- Jira KAN: https://kohansal.atlassian.net/jira/software/projects/KAN
- Figma V1: https://www.figma.com/design/BKS86q9M6nJPNLlegK7Zwz
- Figma V2: https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl
- FigJam: https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3

## قواعد Evidence Integrity

- Fact، Evidence، Logical Inference و Hypothesis از هم جدا نگه داشته می‌شوند.
- چند خروجی از یک Dataset، چند Evidence مستقل محسوب نمی‌شوند.
- Benchmark اثبات Demand محلی نیست.
- Convenience Sample به Population تعمیم داده نمی‌شود.
- Q18/Q19/Q20/Q23/Q24 عمداً Confidence پژوهشی ندارند.
- مدل مالی تا ورود داده معتبر Stage-Gated و Break-even based باقی می‌ماند.

## حریم خصوصی و حق نشر

داده خام دارای PII و منابع دارای حق نشر در مخزن عمومی بازنشر نمی‌شوند. فقط خروجی تحلیلی، لینک منابع و Artifactهای مناسب Portfolio نگهداری می‌شوند.