## Preetam Roy

**Data and process analytics — financial services back-office operations.**

I work where analytics meets operations: taking the messy reality of a case-management
process — SLA clocks, rework loops, backlogs, work that changes hands five times — and
turning it into something a business can actually act on.

Currently Business Process Lead (Data Analytics) at **Tata Consultancy Services**, working
on the NEST Pensions account. Previously at **Diligenta**, a TCS subsidiary, in
Peterborough, UK. MSc Computer Science, Queen Mary University of London.

### What I actually do

- **Operational analysis at scale** — SQL and Python over 50K+ monthly case records, finding
  where the time and the failures really are rather than where people assume they are.
- **Power BI that survives contact with users** — dimensional models, DAX that performs,
  and dashboards leadership uses to make decisions instead of admiring.
- **Process improvement with evidence** — Lean Six Sigma applied properly: measure the
  process, establish whether a change is signal or noise, then fix the right thing.
- **Report automation** — removing the recurring manual work that quietly consumes an
  analyst's week.

### Featured project

**[opslab](https://github.com/pr1317/opslab)** — an operations analytics toolkit for
back-office processes, in pure standard-library Python.

**[Score a case →](https://pr1317.github.io/opslab/)**  The fitted survival model,
running in your browser over a simulated pensions back office. Set a case's
complexity, backlog pressure and channel, pick an SLA target, and watch its
probability of breaching move — a typical case sits at 27%, and the same case
waiting on a third party at 83%. The map filter, the control charts and the DAX
findings are live too. Nothing is fitted client side: the coefficients and the
baseline hazard come from the Python, and a parity test holds the two to 1e-9.

The [full static report](https://pr1317.github.io/opslab/report.html) is the same
analysis as a document, with every chart drawn by the package itself. To run it on
your own machine, `pip install git+https://github.com/pr1317/opslab` then
`opslab try`.

Four modules, each built because the obvious tool gets the wrong answer:

| | |
|---|---|
| **Process mining** | Discovers the real process map from event logs — rework loops, bottlenecks, handovers, and a four-eyes segregation-of-duties check run against the log rather than the policy document |
| **Statistical process control** | Control charts with all eight Nelson run rules, process capability, and Gage R&R — so "the numbers moved" gets tested instead of assumed |
| **SLA survival analysis** | Kaplan-Meier and Cox proportional hazards on right-censored case data, because the cases still open are the slow ones and dropping them flatters every report that does it |
| **Power BI linter** | 20 static-analysis rules over tabular models and DAX, reading TMSL and TMDL, exit-coded for CI |

Case durations in its test data come from a model whose true coefficients are published in
the source, so the analysis is *verifiable* — a test asserts the fitted estimates land
within three standard errors of the values that generated the data.

### Other projects

- **[customer-churn-analytics](https://github.com/pr1317/customer-churn-analytics)** — churn
  prediction on the 7,043-customer IBM Telco dataset in Python, Pandas and scikit-learn.
  **0.846 ROC-AUC**, 75% recall at a threshold tuned to 0.56. Accuracy is the least
  interesting number here — 73.5% of these customers stay, so "nobody leaves" scores 73.5%
  and is worth nothing; the campaign returns **8.2×**, and stays profitable down to a 10%
  offer-acceptance rate.
- **[handwritten-digit-recognition](https://github.com/pr1317/handwritten-digit-recognition)** —
  **98.48%** on the standard 10,000-image MNIST test set: 152 digits wrong, from a 784-256-10
  network trained in 51 seconds on two CPU cores. Preprocessing beat model choice — removing
  handwriting slant with an affine shear is worth **+3.34 points**, more than the gap between
  the worst and best model in the whole comparison.
- **[smart-traffic-management](https://github.com/pr1317/smart-traffic-management)** — YOLOv4-tiny
  and a centroid tracker turning a highway camera into telemetry: **26 unique vehicles counted
  at 8.2 fps** on two CPU cores. Near-field recall is **0.33**, stated rather than hidden — the
  clip ships without labels, so an overall "detection accuracy" would be a number with nothing
  behind it.
- **[Portfolio](https://github.com/pr1317/Portfolio)** — the source of my personal site at
  **[pr1317.github.io](https://pr1317.github.io)**, where all four projects run live: score a
  case against the SLA model, draw a digit, score a customer, watch the traffic counter run.
  Static files, no framework and no bundler.

### Toolbox

`SQL` · `Python` · `Power BI` · `DAX` · `Power Query` · `Advanced Excel` ·
`MySQL` · `PostgreSQL` · `Oracle` · `MongoDB` · `Java` · `C++` · `JavaScript`

Process mapping · Root cause analysis · Requirements gathering · SLA and KPI management ·
UAT support · Statistical process control · Survival analysis · Computer vision (OpenCV, YOLO)

### Certifications

- **Microsoft Certified: Power BI Data Analyst Associate (PL-300)**
- **Lean Six Sigma Green Belt** — Tata Consultancy Services

### Elsewhere

[LinkedIn](https://linkedin.com/in/preetam-roy)
