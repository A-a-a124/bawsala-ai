# Strategic AI Readiness Simulator
### محاكي الجاهزية الاستراتيجية للذكاء الاصطناعي

> A strategic decision-support simulator that helps Saudi organizations choose an AI adoption path — balancing cost, execution speed, and digital sovereignty — and produces a board-ready decision memorandum.

> أداة محاكاة استراتيجية تساعد المؤسسات السعودية على اختيار مسار تبنّي الذكاء الاصطناعي، بموازنة التكلفة وسرعة التنفيذ والسيادة الرقمية، وتُخرج مذكرة قرار جاهزة لمجلس الإدارة.

**ABDULLAH ALADHYANI**

---

## The problem | المشكلة

Every regulated organization in Saudi Arabia faces the same strategic question: adopt global AI services (fast and inexpensive, but data leaves the Kingdom), build sovereign capability in-house (full control, but costly and slow), or run a hybrid model?

Answering it properly normally requires a consulting engagement measured in months. This simulator compresses that analysis into minutes — grounded in the regulatory reality of the Saudi market: NCA ECC, NDMO data classification, PDPL, SAMA, CST, and HCIS.

تواجه كل مؤسسة منظَّمة في المملكة السؤال نفسه: هل نعتمد على خدمات ذكاء اصطناعي عالمية جاهزة، أم نبني قدرة سيادية داخلية، أم نمضي بنموذج هجين؟ الإجابة عادةً تستغرق أشهراً من العمل الاستشاري — وهذه الأداة تختصرها إلى دقائق، مبنيةً على الواقع التنظيمي السعودي.

## What it does | ما تفعله

Four inputs — **sector, organization size, data sensitivity, technology budget** — produce a complete strategic comparison of three adoption paths:

| Path | Indicative cost | Timeline | Sovereignty risk | Execution speed |
|---|---|---|---|---|
| Full Foreign Adoption | ✔ | ✔ | ✔ | ✔ |
| Full Sovereign Build | ✔ | ✔ | ✔ | ✔ |
| Hybrid Model | ✔ | ✔ | ✔ | ✔ |

## Capabilities | المزايا

**Analysis**
- **Dual engine** — a deterministic offline engine (instant, repeatable, requires no network) plus an optional live engine that interprets a free-text scenario. The live engine falls back to the offline model transparently on any failure, and the interface always states which engine produced the result.
- **Automatic recommendation** with a written board-level justification and a stated confidence level. Decision weights shift with the inputs: higher data sensitivity and stricter regulation raise the weight of sovereignty; a smaller budget raises the weight of cost.
- **Decision-weight transparency** — the weighting the engine applied is shown to the user, not hidden behind a score.

**Financial modelling**
- **Five-year cumulative cost curve** with automatic break-even detection, exposing the real financial commitment beyond year one.
- **Cost breakdown** — CAPEX/OPEX split and spend distribution across infrastructure, licenses, talent, and integration.

**Risk & compliance**
- **Detailed risk map** — the headline sovereignty score decomposed into vendor lock-in, data exposure, geopolitical exposure, talent scarcity, and operational continuity.
- **Regulatory compliance matrix** — each path scored against the controls that actually apply to the selected sector, including a sector-specific control (SAMA for financial, CST for telecom, HCIS for energy, cloud policy for government), with a compliance percentage per path. Selecting Top Secret data automatically tightens the assessment.

**Delivery**
- **Radar comparison** across five dimensions: cost efficiency, speed, sovereignty, scalability, and talent readiness.
- **Implementation roadmap** — four phases with indicative time windows, specific to the recommended path.
- **Save & compare** — keep several analyses side by side to compare scenarios.
- **PDF board memorandum** — executive page, comparison table, compliance matrix, roadmap, final recommendation, and a sign-off block, in Arabic or English with correct Arabic typography.
- **Full Arabic/English interface** with correct RTL layout and a dark executive theme.

## Technical overview | نظرة تقنية

| Layer | Stack |
|---|---|
| Backend | Python · Flask |
| Analysis engine | Parametric deterministic model with an optional LLM-assisted layer |
| Frontend | React · Chart.js · bilingual RTL interface |
| Reporting | ReportLab with Arabic shaping and bidirectional text layout |

The application runs entirely offline by default: front-end dependencies are vendored locally and the default engine requires no network access and no API key.

## Methodology notes | ملاحظات منهجية

- Data sensitivity levels mirror the NDMO national data classification scheme (Public / Internal / Confidential / Top Secret).
- Regulatory weighting per sector reflects the intensity of that sector's supervisory regime.
- Cost figures are **indicative planning ranges in USD** produced by a parametric model. They are not quotations and do not replace a detailed feasibility study.
- The compliance matrix expresses a typical posture per path. An actual compliance determination requires review by the relevant regulator and the organization's own compliance function.

## Disclaimer | إخلاء مسؤولية

This is a decision-support simulation tool. All outputs are indicative and intended to structure a strategic discussion — not to serve as financial, legal, or regulatory advice.

أداة محاكاة لدعم القرار؛ جميع المخرجات استرشادية وتهدف إلى تنظيم النقاش الاستراتيجي، ولا تُعدّ استشارة مالية أو قانونية أو تنظيمية.

## Source code | الكود المصدري

This repository presents the project and its capabilities. The source code is kept private; access can be arranged on request for evaluation purposes.

هذا المستودع يعرض المشروع ومزاياه. الكود المصدري خاص، ويمكن ترتيب الاطلاع عليه عند الطلب لأغراض التقييم.

## License | الترخيص

Documentation and project materials in this repository © 2026 ABDULLAH ALADHYANI. See [LICENSE](LICENSE).

---

Built by **ABDULLAH ALADHYANI**
