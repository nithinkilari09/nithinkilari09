<div align="center">

# Hi, I'm Nithin Kilari 👋

### Data Engineer & Data Analyst · M.S. Data Science (4.0 GPA), Oklahoma City University

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Building+automated%2C+end-to-end+data+pipelines;GCP+%2B+Snowflake+%C2%B7+AWS+%2B+Databricks+%C2%B7+BigQuery+%C2%B7+Athena;Real+live+data%2C+not+toy+datasets)](https://git.io/typing-svg)

[![Email](https://img.shields.io/badge/Email-nithinkilari09%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:nithinkilari09@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kilari_Nithin-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kilari-nithin-619481272/)
[![Profile Views](https://komarev.com/ghpvc/?username=nithinkilari09&style=flat-square&color=58A6FF&label=Profile+Views)](https://github.com/nithinkilari09)

</div>

---

### 👀 What I actually do

Four portfolio projects, each built end to end on **real, live, public data** — no
sample datasets, no mocked pipelines. Two data-engineering builds (scheduled ingestion →
cloud warehouse → live dashboard, zero manual steps) and two data-analytics builds
(locked business questions, confounder-aware findings, real numbers only). Every repo
ships a build log documenting what broke and how it was actually fixed.

---

## 🧱 Data Engineering

<table>
<tr>
<td width="50%" valign="top">

### 🌐 [tech-skill-demand-pipeline](https://github.com/nithinkilari09/tech-skill-demand-pipeline)

Live pipeline over real tech job postings — which skills/tools recruiters actually ask
for, by CS domain, updated daily with zero manual steps.

**🟢 [Live dashboard →](https://nithinkilari09.github.io/tech-skill-demand-pipeline/)**

- RemoteOK + Arbeitnow → **S3** → **Databricks** medallion (Bronze/Silver/Gold, PySpark
  + Delta Lake + Unity Catalog) → static **GitHub Pages** dashboard
- 1,002 postings deduped, classified into a CS-domain taxonomy + 11 non-tech categories,
  skills matched against a 61-entry curated dictionary
- Fully scheduled, no human trigger: ingest 03:00 UTC → ETL 04:00 UTC → dashboard
  rebuild 06:00 UTC — every stage verified with a real triggered run

`AWS S3` `Databricks` `PySpark` `Delta Lake` `Unity Catalog` `GitHub Actions` `Plotly`

</td>
<td width="50%" valign="top">

### 🌍 [geopolitical-pulse](https://github.com/nithinkilari09/geopolitical-pulse)

Near-real-time analytics over the GDELT 2.0 global event database — where is
geopolitical tension escalating *right now*.

**🟢 Ingestion live** — 15-minute GitHub Actions cron, unattended

- GCS landing → **Snowflake** storage integration → Streams + Tasks (incremental
  loads) → **Snowpark** silver transforms → 5 SQL marts → **Streamlit-in-Snowflake**
  dashboard
- Marts answer tension-by-region, event-type spikes vs. a 24h baseline, tone trend, and
  top-coverage countries — not a raw-field dump
- Deliberately Snowflake-centric on GCP, complementing the AWS/Databricks stack next
  door so tooling doesn't overlap across the portfolio

`GCP · GCS` `Snowflake` `Snowpark` `Streams & Tasks` `Streamlit` `GitHub Actions`

</td>
</tr>
</table>

## 📊 Data Analytics

<table>
<tr>
<td width="50%" valign="top">

### 🛒 [instacart-basket-analysis](https://github.com/nithinkilari09/instacart-basket-analysis)

Behavior analysis of **~3M real Instacart orders** built to answer five specific
business questions — churn, loyalty, timing, product strategy — not a generic
"explore the dataset" notebook.

**🟢 [Live Tableau dashboard →](https://public.tableau.com/app/profile/nithin.kilari/viz/instakart-basket-analysis/Dashboard1)**

- **BigQuery** (load + SQL) → **pandas** (confounder-aware analysis) → **Tableau**
  (5-panel published dashboard)
- Real headline finding: reorder rate holds 55–68% up to 29 days since last order,
  then cliffs to 45.8% at 30+ days
- 229 "anchor" products identified by reorder frequency + basket presence, not price —
  this dataset has no revenue field, and no chart here pretends otherwise

`BigQuery` `SQL` `pandas` `Tableau`

</td>
<td width="50%" valign="top">

### 💊 [physician-payments-prescribing](https://github.com/nithinkilari09/physician-payments-prescribing)

Do industry payments to physicians correlate with brand-name prescribing? Same genre
of question as ProPublica's *Dollars for Docs*, framed strictly as association, not
causation, with specialty controlled for throughout.

**Streamlit dashboard** (Sankey, treemap, icicle decomposition) over **CMS Open
Payments (14.3M rows) + Medicare Part D (1.38M rows)**, joined on NPI

- **S3 → Athena** (serverless SQL, no cluster) **→ pandas → Streamlit/Plotly**
- Real finding: a modest but statistically robust payment↔brand-prescribing
  association survives two independent confounder methods (ΔR² ≈ 0.0023–0.0025)
- Payments are highly concentrated: top 1% of paid physicians take 66% of all
  physician-directed dollars (Gini = 0.93)

`AWS S3` `Athena` `Glue` `pandas` `Streamlit` `Plotly`

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 📈 GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=nithinkilari09&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=nithinkilari09&layout=compact&theme=tokyonight&hide_border=true" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=nithinkilari09&theme=tokyonight&hide_border=true" />

</div>

---

<div align="center">

**📫 Reach out:** [Email](mailto:nithinkilari09@gmail.com) · [LinkedIn](https://www.linkedin.com/in/kilari-nithin-619481272/)

</div>
