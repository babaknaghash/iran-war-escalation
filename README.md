# Iran War Escalation

**OSINT and market-based escalation risk assessment skill for Iran–Israel–United States tensions, with structured Persian-language reports.**

اسکیل **Iran War Escalation** برای پایش و تحلیل خطر تشدید تنش یا درگیری مرتبط با ایران، اسرائیل و ایالات متحده طراحی شده است. خروجی آن یک **ارزیابی ریسک مبتنی بر شواهد** است، نه پیش‌بینی قطعی وقوع جنگ.

## قابلیت‌ها

- ترکیب منابع مستقل در حوزه دیپلماسی، حریم هوایی و NOTAM، دریانوردی و تنگه هرمز، تحرکات نظامی تأییدشده و منابع OSINT.
- بررسی شاخص‌های بازار مانند نفت Brent و WTI، طلا، VIX، نرخ ارز، اوراق قرضه، سهام، رمزارز و بازارهای پیش‌بینی.
- پایش اختلال‌های GNSS، AIS، اینترنت و داده‌های عمومی ماهواره‌ای در صورت دسترسی.
- ارائه امتیاز ریسک **۰ تا ۱۰۰** و برچسب‌های Green / Yellow / Orange / Red / Black با روش امتیازدهی مستند.
- تهیه گزارش فارسی با بخش‌های ثابت، سناریوهای ۲۴ ساعت آینده، سطح اطمینان، محدودیت منابع و تغییرات نسبت به گزارش قبلی.
- تفکیک واقعیت تأییدشده، گزارش معتبر، ادعای تأییدنشده و سیگنال غیرمستقیم بازار.

## ساختار مخزن

```text
iran-war-escalation/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── icon.svg
└── references/
    ├── indicator-taxonomy.md
    ├── market-watchlist.md
    ├── report-template.md
    ├── scoring-rubric.md
    └── source-checklist.md
```

## استفاده

این مخزن یک اسکیل مبتنی بر دستورالعمل‌های Markdown است و به‌تنهایی داده زنده دریافت نمی‌کند. برای اجرا، پوشه مخزن را در محیطی که از اسکیل‌های دارای `SKILL.md` پشتیبانی می‌کند قرار دهید و قابلیت دسترسی به وب/داده‌های عمومی را برای عامل اجراکننده فراهم کنید.

**نمونه درخواست:**

> با استفاده از اسکیل Iran War Escalation، خطر تشدید درگیری میان ایران، اسرائیل و آمریکا را برای ۲۴ ساعت آینده بررسی کن. شاخص‌های عددی، منابع، شواهد متناقض و محدودیت داده‌ها را صریح گزارش بده.

**Example prompt (English):**

> Use the Iran War Escalation skill to assess escalation risk involving Iran, Israel, and the United States over the next 24 hours. Produce the structured report in Persian, cite sources, and state unavailable data explicitly.

## روش و محدودیت‌ها

۱. گردآوری داده‌ها مطابق `references/source-checklist.md` و دسته‌بندی سیگنال‌ها مطابق `references/indicator-taxonomy.md`.
۲. سنجش هم‌راستایی شواهد مستقل و امتیازدهی مطابق `references/scoring-rubric.md`.
۳. تدوین خروجی مطابق قالب `references/report-template.md`.

**نکته:** نمره ریسک و احتمال سناریوها برآورد تحلیلی هستند، نه احتمالات آماری کالیبره‌شده. کیفیت گزارش وابسته به تازگی، اعتبار و دسترس‌پذیری منابع است. داده‌های مسدود، تأخیردار یا ناموجود باید در گزارش مشخص شوند. این اسکیل توصیه نظامی عملیاتی یا سرمایه‌گذاری ارائه نمی‌کند.

## Scope (English)

The skill evaluates geopolitical escalation involving Iran, Israel, and the United States by corroborating public diplomatic, aviation, maritime, military-logistics, cyber/GNSS, energy, financial-market, and prediction-market signals. It produces a Persian risk report with a 0–100 heuristic score, confidence level, scenario assessment, source citations, and explicit data-access limitations. It does **not** predict military outcomes or supply tactical advice.

## نام و تغییرات

شناسه و نام نمایشی اسکیل **Iran War Escalation** (`iran-war-escalation`) است. دامنه منابع، فرایند تحلیل و قالب گزارش اصلی حفظ شده‌اند.
