# Prototype تعاملی V3

وضعیت طراحی :: **کامل‌شده**  
وضعیت Feature :: **Selected for Validation — نه Validation‌شده**

- [اجرای نسخه Canonical V3](index.html)
- [نسخه ثابت V3](v3.html)
- [Figma V2](https://www.figma.com/design/y7r2zCBHGz1gVHsZ2MArWl)
- [FigJam — نقشه تصمیم](https://www.figma.com/board/tbsGkzv48y5wmnChZqpTB3)
- [Q23 — User Journey](../../docs/questions/q23/)
- [Q24 — Low-Fidelity و Prototype](../../docs/questions/q24/)
- [MVP Definition](../../solution/mvp/)
- [Jira Delivery Map](../../delivery/jira/)

## تغییرهای V3

- Quiz شش‌مرحله‌ای شامل دسته، نوع پوست، دغدغه، هدف، بودجه و منشأ برند
- خلاصه قابل ویرایش پاسخ‌ها پیش از Recommendation
- نمایش پنج Recommendation در Prototype
- درصد تطابق نمایشی برای توضیح منطق رتبه‌بندی
- توضیح «چرا این محصول؟» برای هر گزینه
- PDP شخصی‌سازی‌شده و افزودن به سبد
- ثبت بازخورد مثبت یا منفی و دلیل بازخورد
- نمایش User Flow، Rule-based Logic و اصول UX در تب‌های مستقل

## مسیر تجربه پیاده‌شده

**Entry → Introduction → Six-step Quiz → Profile Summary → Loading → Five Recommendations → Why this product → PDP → Cart → Feedback**

Alternative مستقل در V3 به‌عنوان P1 و Future مشخص شده است و نباید به‌عنوان قابلیت پیاده‌شده فعلی معرفی شود.

## محدوده V3

| بخش | وضعیت |
|---|---|
| Entry و معرفی ارزش | پیاده‌شده |
| Quiz شش‌مرحله‌ای | پیاده‌شده |
| Back و Edit | پیاده‌شده |
| پنج Recommendation نمونه | پیاده‌شده |
| Why this product | پیاده‌شده |
| PDP و افزودن به سبد | پیاده‌شده |
| Feedback و دلیل بازخورد منفی | پیاده‌شده |
| Alternative مستقل | P1 و Future |
| اتصال به Inventory واقعی | نیازمند Delivery |
| No-match واقعی | نیازمند Delivery |
| Recommendation Engine واقعی | نیازمند Validation و Product Data |

## منطق پیشنهادی MVP

موتور اجرایی باید Rule-based یا Concierge باشد و این ورودی‌ها را در نظر بگیرد:

1. Category
2. Skin Type
3. Main Concern
4. Purchase Goal
5. Budget
6. Brand Origin Preference
7. Product Availability و Product Data معتبر

## مرز عددهای Prototype

درصدهای Match، قیمت‌ها، Ratingها، Product Claims و زمان «کمتر از دو دقیقه» در V3 داده واقعی آزمایش نیستند. آن‌ها محتوای نمایشی برای تست Flow هستند و پیش از Pilot باید با Catalog، Inventory، Analytics و Compliance واقعی خانومی جایگزین یا تأیید شوند.

## Guardrailهای لازم برای Delivery

- جلوگیری از Medical Claim
- حذف SKU ناموجود یا فاقد داده کافی
- جلوگیری از Match Percentage بدون فرمول کالیبره
- Grounding دلیل پیشنهاد به پاسخ کاربر و Product Data
- حفظ مسیر Browse و Cart
- رضایت برای ذخیره ترجیحات
- No-match صادقانه
- Versioning و Rollback Rule Set

## رویدادهای Validation

| مرحله | Event پیشنهادی |
|---|---|
| مشاهده Entry | guide_exposed |
| شروع راهنما | guide_started |
| پاسخ به سؤال | question_answered |
| ویرایش پاسخ | answer_edited |
| تکمیل Quiz | guide_completed |
| مشاهده Recommendation | recommendation_viewed |
| بازکردن دلیل | recommendation_reason_opened |
| ورود به PDP | recommendation_pdp_clicked |
| افزودن به سبد | recommended_item_added |
| ثبت Feedback | recommendation_feedback_submitted |
| خروج | guide_exited |

## سناریوهای تست

- Happy Path از Entry تا Cart
- Edit Path از Summary به سؤال قبلی
- Why Path برای فهم دلیل Recommendation
- Feedback Path با دلیل منفی
- Safety Path برای درخواست پزشکی یا خارج از Scope
- No-match Path پس از اتصال Engine واقعی
- Availability Path با تغییر موجودی

## Definition of Done این Artifact

- V3 روی مسیر Canonical GitHub قرار دارد
- نسخه ثابت v3.html برای Traceability نگهداری می‌شود
- Flow و Scope واقعی V3 مستند شده‌اند
- تفاوت Prototype Data و داده معتبر صریح است
- لینک‌های Q24، Figma، Jira و Presentation به نسخه Canonical متصل‌اند
