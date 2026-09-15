# HR SaaS Unit Economics and Funnel Model

A spreadsheet model and one-page memo on a single question: for an Indian SMB payroll/HR SaaS priced per employee per month, which lever moves LTV:CAC most — churn, funnel conversion, pricing or seat expansion?
Base-case answer: demo-to-paid conversion and price tie (+20% each for a 20% improvement), ahead of churn (+16%).
All inputs are labelled assumptions or cited public benchmarks. No company data is used.

*Independent project, not affiliated with any company named.*

## Why this exists

HR and payroll software for Indian SMBs is sold per employee at low prices, so small changes in conversion, churn or price decide whether a customer is worth acquiring. I built this to practise the numbers behind that decision: a funnel, unit economics and a clear ranking of levers, with every assumption visible and changeable.

## What's inside

- `hr_saas_unit_economics.xlsx` — live-formula model: Inputs, Scenarios (bear/base/bull), 24-month Funnel, Unit Economics, Sensitivity.
- `memo.md` — one-page decision memo with base-case numbers, limits and three questions for the real team.
- `README.md` — this file.

## Key findings

Base case, from the workbook:

- LTV:CAC is 1.73 (LTV ₹106,858; CAC ₹61,919). CAC payback is 20.2 months.
- Improving each lever by 20%: price +20.0%, demo held-to-paid +20.0%, churn +16.2%, visitor-to-sign-up +12.2%, seat expansion +4.8%.
- A 20% price rise gains nothing if it cuts demo-to-paid conversion by 16.7%, so conversion is the safer first lever.
- When churn is high (bear case, 5% a month), cutting churn ranks first (+21.1%).
- At one blended CAC, 10–25 employee accounts return 0.73x and 101–500 employee accounts 6.3x.

## How to use

1. Open the workbook in Excel or Google Sheets. Formulas recalculate on open.
2. Choose Bear, Base or Bull in `Scenarios!C3`.
3. Change any blue cell in `Inputs` or `Scenarios`. Black cells are formulas.
4. Read results in `Unit Economics` and the lever ranking in `Sensitivity`.

The memo quotes the base case. It does not update when inputs change.

## Sources

All accessed 16 September 2026. Benchmarks are third-party figures, not data from any HR SaaS company.

| Source | Used for |
|---|---|
| [Asanify pricing (India)](https://asanify.com/pricing) | ₹99 and ₹199 per employee per month; up to 60% off select plans; 2 months free on annual plans |
| [Keka pricing](https://www.keka.com/pricing) and [HROne on Keka pricing](https://hrone.cloud/blog/keka-pricing-india/) | ₹90–150 per extra employee. Hidden in Keka's page source, not shown on the live page; HROne, a competitor, reports the same. Unverified. |
| [greytHR pricing](https://www.greythr.com/pricing/) | ₹2,495–4,495 per month for 50 employees; ₹45–85 per extra employee |
| [RazorpayX Payroll pricing](https://razorpay.com/payroll/pricing/) | ₹3,499 per month for up to 20 employees; ₹150 per extra employee; plus GST |
| [Zoho Payroll pricing (India)](https://www.zoho.com/in/payroll/pricing/) | ₹1,000–4,000 per month (annual billing) with 25–50 employees; ₹40–80 per extra employee |
| [First Page Sage: B2B SaaS funnel benchmarks](https://firstpagesage.com/seo-blog/b2b-saas-funnel-conversion-benchmarks-fc/) (updated 11 June 2025) | Visitor-to-lead 2.3%, lead-to-MQL 37%, MQL-to-SQL 32%, SQL-to-opportunity 40%, opportunity-to-close 46% (small-company buyers) |
| [First Page Sage: free trial benchmarks](https://firstpagesage.com/seo-blog/saas-free-trial-conversion-rate-benchmarks/) (updated 5 September 2025) | HR-industry trial-to-paid 22.7% (bear case) |
| [GrowthSpree: demo show rates](https://www.growthspreeofficial.com/blogs/b2b-saas-demo-show-rate-benchmarks-2026-by-source-day-of-week-time-to-demo-acv-vertical) | Median show rate 55–65%. Vendor blog; no method disclosed. |
| [Kalungi: SaaS churn benchmarks](https://www.kalungi.com/blog/saas-churn-rate-benchmarks) (May 2025) | SMB SaaS monthly churn 3–7%. No underlying study cited. |
| [SaaS Capital: 2026 spending benchmarks](https://www.saas-capital.com/blog-posts/spending-benchmarks-for-private-b2b-saas-companies/) | Cost-of-revenue lines used to set gross margin |
| [KeyBanc and Sapphire Ventures survey](https://sapphireventures.com/press/keybanc-capital-markets-and-sapphire-ventures-private-saas-company-survey/) | ~23-month median CAC payback (2022), as a sanity check |

Not verified and therefore labelled as assumptions: segment mix, average headcount per segment, list prices by segment, marketing cost per visitor, sales cost per demo, seat expansion, visitor volume.

## CV bullet

Built a 24-month funnel and unit-economics model (Excel, live bear/base/bull scenarios) for an Indian SMB payroll SaaS using public pricing from 5 vendors and cited benchmarks; ranked five growth levers and showed a 20% gain in demo-to-paid conversion lifts LTV:CAC as much as a 20% price rise (1.73 to 2.07); wrote a one-page decision memo.
