# 📊 Recruitment Performance & Efficiency Analysis 2024–2025

### Author: Vo Tran Mai Khanh
### Date: 01/2026
### Tools Used: Power Query, PBI

## 📌 Background & Overview  

### 📖 Objective:
This project evaluates recruitment performance to identify inefficiencies, optimize hiring investment and support data driven workforce decisions.
- Recruitment Channel Effectiveness: assess sourcing performance using hiring rate, CV efficiency and role level contribution to optimize channel investment
- Business Unit & Position Efficiency: analyze conversion patterns across business units and job families to identify structural bottlenecks and refine hiring strategies by role complexity
- Recruiter (PIC) Performance & Workload: evaluate recruiter effectiveness through stage conversion rates, CV effort per hire and workload distribution to improve governance and balance performance
- Year over Year Diagnosis (2024–2025): compare trends to distinguish structural hiring issues from short-term fluctuations

### 👤 Who is this project for?  
- HR Management – to monitor recruitment performance, identify structural inefficiencies and make strategic workforce planning decisions
- HR Team (Talent Acquisition) – to optimize sourcing channels, improve stage level conversion and allocate recruiter workload more effectively
- Business Unit Leaders – to understand hiring efficiency within their teams and adjust role-specific hiring strategies
- Board of Directors (BOD) – to gain visibility into hiring effectiveness, investment efficiency and talent scalability to support expansion decisions

### 👤 Client Background

The A Holdings is a UK based investor that entered the Vietnam market 13 years ago with its first franchise in English education, following strong expansion in other countries. The investor has since diversified into pre-school English, STEM and non-education management services, resulting in significant human resource demands for smooth operations and further expansion

## 📂 Dataset Description & Data Structure

### 📊 Data Source  
- Source: internal data from company’s website and other third party hiring channels (TOPCV, VNW, CareerViet, etc.)
- Size: ~27,000+ records across 01 fact table and 04 supporting dimensions
- Format: .xlsx

#### 1️⃣ Tables Used:
- Recruitment Tracking
- Dimension Position
- Dimension Business Unit
- Dimension Hiring Sources
- Dimension Date

#### 2️⃣ Table Schema & Data Snapshot: 
**Table 1: Recruitment tracking**
<details>
<summary>Recruitment tracking Schema</summary>
<img width="740" height="94" alt="image" src="https://github.com/user-attachments/assets/f1a28c75-9e15-4e48-875d-5db2024641a4" />
<img width="959" height="95" alt="image" src="https://github.com/user-attachments/assets/05cbffd2-3fdc-47c4-9411-16c49d8215ee" />
</details>

**Table 2: Dimension Position**
<details>
<summary>Dimension Position Schema</summary>
<img width="551" height="95" alt="image" src="https://github.com/user-attachments/assets/53478283-3bcb-443f-97d4-03b1acaf0d11" />
<img width="572" height="94" alt="image" src="https://github.com/user-attachments/assets/7659c113-2710-43c7-be97-d4b1d1964ffd" />
<img width="574" height="95" alt="image" src="https://github.com/user-attachments/assets/25d33f09-ad65-4e29-a658-8ac45002fd6f" />
<img width="571" height="94" alt="image" src="https://github.com/user-attachments/assets/2f9f0f2c-7d04-43b8-a5a0-f5ad47b3ad2f" />
<img width="628" height="93" alt="image" src="https://github.com/user-attachments/assets/d4e27e5a-f664-47ca-906b-18645871e678" />
</details>

**Table 3: Dimension Business Unit**
<details>
<summary>Dimension Business Unit</summary>
<img width="133" height="96" alt="image" src="https://github.com/user-attachments/assets/972ca654-fe68-46b5-80b0-19589d1e93a3" />
</details>

**Table 4: Dimension Hiring Sources**
<details>
<summary>Dimension Hiring Sources</summary>
<img width="77" height="279" alt="image" src="https://github.com/user-attachments/assets/00f9599d-4e52-435b-966b-26c693432af2" />
</details>

**Table 5: Dimension Time**
<details>
<summary>Dimension Time</summary>
<img width="387" height="263" alt="image" src="https://github.com/user-attachments/assets/3cd02e5c-353b-4b61-8084-4cc1c36c8bef" />
</details>

#### 3️⃣ Data Relationships:
- Recruitment Tracking -> Dim Time: many to one
- Recruitment Tracking -> Dim Position: many to one
- Recruitment Tracking -> Dim Business Unit: many to one
- Recruitment Tracking -> Dim Hiring Sources: many to one

<img width="698" height="470" alt="image" src="https://github.com/user-attachments/assets/0c327361-57a4-48d7-bd0c-2baceb77c3ac" />

## 🧠 Design Thinking Process  
### 1️⃣ Empathize 

<img width="756" height="489" alt="image" src="https://github.com/user-attachments/assets/16212c75-a7d2-4a5e-a58f-bff542c785af" />

### 2️⃣ Define point of view 

<img width="1035" height="303" alt="image" src="https://github.com/user-attachments/assets/7197ff05-d301-4284-8e37-491208c11b49" />

### 3️⃣ Ideate  

<img width="1087" height="227" alt="image" src="https://github.com/user-attachments/assets/c58fb124-b4ae-4199-b97f-d811feb23832" />

## 📊 Key Insights & Visualizations  

### 1️⃣ Recruitment Performance Overview

### 📌 Analysis 1. Overall Hiring Performance: 2024 vs 2025

In 2024, recruitment pipeline operated with relatively strong efficiency. Out of 11,931 screened candidates & 274 were successfully onboarded, resulting in a Hiring Success Rate of 2.3%. Offer Acceptance reached 92.3%, indicating strong offer competitiveness and stable late-stage conversion

<img width="1040" height="313" alt="image" src="https://github.com/user-attachments/assets/87f939c0-688b-437b-8a55-6f9ac8212ac5" />

In 2025, although screening volume increased significantly to 14,876 candidates (+25%), total onboarded hires declined sharply to 126. As a result, Hiring Success Rate dropped to 0.8% (–63% YoY). This indicates that the issue in 2025 is not pipeline volume but conversion effectiveness. 2025 reflects a pattern of increased effort but reduced output

<img width="1037" height="311" alt="image" src="https://github.com/user-attachments/assets/f819d4de-b2a2-4a19-89eb-28c02d4a0743" />

### 📌 Analysis 2. Pipeline Productivity Deterioration

Productivity indicators further confirm this shift. In 2024, 7 CVs were required to generate 1 interview, 6 interviews were required to secure 1 offer

#### *2024 Hiring Efficiency & Conversion*

<img width="1036" height="175" alt="image" src="https://github.com/user-attachments/assets/bd24ad5f-205e-4e3b-a667-9240ac545904" />

In 2025, screening efficiency declined significantly: CVs per interview increased by 42.9% and interviews per offer surged by 66.7% versus 2024. Recruiter effort has increased substantially while yield per stage has decreased. Although offer per hire remains at 1, overall offer issuance has dropped due to weakened upstream conversion. The recruitment engine is working harder but producing fewer outcomes.
TopCV, CareerViet and LinkedIn remained key sources but offer conversion rates declined. Zalo and Employee Referral maintained high offer rates (>25%). Low conversion from Facebook, VNW and other boards suggests stricter source screening is needed

#### *2025 Hiring Efficiency & Conversion*

<img width="1040" height="169" alt="image" src="https://github.com/user-attachments/assets/bcb9bfc5-b18e-4cc1-9e8a-ac15351be7b5" />

### 📌 Analysis 3. Funnel Quality Deterioration
In 2024, the pipeline showed healthy progression and conversion remained stable across stages: 14.6% of screened candidates progressed to interview, 17.1% of interviews converted to offers & 92.3% of offers were accepted

#### *2024 Hiring Funnel & Performance Overview*

<img width="833" height="242" alt="image" src="https://github.com/user-attachments/assets/91d184d0-4148-4a14-8981-6707899cb0a4" />

In 2025, all major transitions weakened simultaneously: screening → interview declined to 10.4%, interview → offer declined to 10.0% & offer acceptance dropped to 81.3%. This suggests a systemic decline rather than an isolated bottleneck. Candidate qualification at screening appears weaker, interview selectivity less precise & offer competitiveness lower than the prior year. Pipeline leakage increased at every stage

#### *2025 Hiring Funnel & Performance Overview*

<img width="836" height="242" alt="image" src="https://github.com/user-attachments/assets/a680d54f-6362-44b0-b7cc-f31b8f6ca5db" />

### 📌 Analysis 4. Business Unit Performance Shift
During 2024, offer acceptance rates were consistently strong across Business Units. Acceptance stability suggested competitive positioning and effective candidate engagement. By 2025, performance divergence emerged: Property Management fell to 75%, Adult English declined to 78.8%, Group HQ dropped to 70.3%, Kids English & STEM remained comparatively stable around 93–94%

Scatter analysis indicates that some units maintain moderate Interview → Offer rates but suffer from declining acceptance. This may point to compensation competitiveness, candidate experience inconsistency, or delayed decision cycles in certain units. Performance dispersion across BUs has widened

#### *2024 Offer Conversion Alignment by Business Unit in*

<img width="527" height="224" alt="image" src="https://github.com/user-attachments/assets/f9b3bb0d-d399-4116-935d-69b85ab48447" />

#### *2025 Offer Conversion Alignment by Business Unit*

<img width="522" height="224" alt="image" src="https://github.com/user-attachments/assets/5fb92357-562f-4408-a664-2c8f65e18330" />

### 📌 Analysis 5. Monthly Trend Pattern

While 2024 reflected temporary fluctuations followed by recovery, 2025 demonstrates sustained efficiency pressure throughout the year. The additional screening volume failed to drive equivalent hiring outcomes, indicating a structural shift rather than cyclical seasonality

The highlighted months indicate periods where screening volume exceeded the annual average while conversion performance fell below benchmark. This signals that increased sourcing intensity did not generate proportional hiring outcomes. In several high-volume periods, efficiency declined further rather than improving. The pattern points to structural inefficiency under pressure — potentially driven by diluted screening criteria, heavier recruiter workload, slower hiring decisions or reduced offer competitiveness. Notably in 2025, the clustering of such months suggests that scaling effort without reinforcing conversion discipline amplified pipeline leakage instead of strengthening hiring success

### Recommendations
#### 1️⃣ Strengthen Early Funnel Qualification
- Align must have criteria before major hiring waves
- Standardize screening checklist to improve CV quality
- Reduce dependency on high volume, low conversion channels
  
#### 2️⃣ Enforce Interview & Decision Discipline
- Implement structured interview scorecards
- Limit excessive interview rounds and monitor roles with high interview-per offer ratios
- Establish strict feedback turnaround timelines

#### 3️⃣ Protect Offer Yield & Drive Accountability
- Conduct systematic analysis of declined offers
- Improve decision speed to reduce candidate drop off
- Track BU level conversion KPIs and link to performance reviews

### 2️⃣ Source Performance & Conversion Effectiveness

<img width="1033" height="358" alt="image" src="https://github.com/user-attachments/assets/5e93ed02-0e60-4672-be1c-b0c30b822684" />

### 📌 Analysis 1. Sourcing Effectiveness Shift

During 2024, hiring output was relatively balanced across major sourcing channels. TopCV & CareerViet generated the largest screening volumes while Employee Referral delivered strong hiring efficiency despite lower volume. Although high volume platforms required greater screening effort, conversion performance remained within an acceptable range, indicating manageable quality dispersion across channels

<img width="1036" height="212" alt="image" src="https://github.com/user-attachments/assets/8c2496bc-4f93-4e84-8198-7801b435bff0" />

Looking at 2025, sourcing dynamics became more polarized. Screening volume increased across major job boards, yet hiring contribution became increasingly concentrated in fewer channels. High volume sources such as CareerViet & TopCV absorbed a disproportionate share of screening activity but delivered weaker hiring success rates. Meanwhile, Employee Referral continued to demonstrate superior efficiency, requiring fewer CVs and interviews per hire

<img width="1038" height="217" alt="image" src="https://github.com/user-attachments/assets/be035d70-4825-43a8-8a17-6bf05de75ae4" />

The volume versus conversion comparison highlights a structural imbalance: incremental screening effort did not produce proportional hiring gains. Instead, effort intensity increased, as reflected in higher CVs per Interview and Interviews per Offer ratios for several large channels. This suggests declining top of funnel quality and reduced mid stage selectivity rather than insufficient pipeline size



Role specific analysis (e.g., Sales) further indicates that channel effectiveness varies by job family. Certain platforms perform adequately at an overall level but underdeliver in function specific hiring, reinforcing the need for role channel alignment rather than uniform source allocation

### *Sales hiring rate by source in 2024*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/fbbd28796079e4b0ff06992bad9a01452ab03607/Source%20-%20Hiring%20rate%20by%20source%20(2024).png)

### *Sales hiring rate by source in 2025*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/40ae679f306329436a2211147fe8073a665a743f/Source%20-%20Sales%20consultant%20hire%20by%20source%20(2025).png)

This pattern is also evident in the Teacher position where channel contribution shifted significantly year over year. While VTJ dominated hiring share in 2024, its sharp decline in 2025 highlights how source performance can fluctuate depending on role dynamics & sourcing strategy adjustments. In contrast, TopCV strengthened its position as the primary hiring driver & Employee Referral emerged as a meaningful contributor, suggesting improved alignment between channel quality & role requirements. Together, these findings emphasize that sourcing strategy should be calibrated at the job-family level, with ongoing performance monitoring to optimize conversion efficiency and hiring outcomes

### *Teacher hiring rate by source in 2024*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/ae7faf39d985fe8052ab37c740a189442de1fc06/Source%20-%20Teacher%20hire%20by%20source%20(2024).png)

### *Teacher hiring rate by source in 2025*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/80cc9e8f8f0f237e2a465a26b511e4ea64396e5d/Source%20-%20Teacher%20hire%20by%20source%20(2025).png)

Overall, the data suggests that sourcing inefficiency in 2025 is driven primarily by channel mix quality rather than absolute screening volume. Without recalibrating allocation toward consistently high-yield channels, additional sourcing effort is likely to amplify recruiter workload rather than improve hiring output

# II. Business Unit & Position Efficiency Analysis – 2024 & 2025
  
Across 2024 & 2025, high CVs per hire consistently concentrate in strategic, technical and Head Quarter based roles with selected commercial positions in Adult English also requiring significant hiring effort. Funnel diagnostics indicate that neither screening intensity nor offer rejection rate fully explains this inefficiency. While mid funnel conversion (interview → offer) contributes in certain roles, the pattern suggests more structural challenges, such as talent scarcity, expectation misalignment & market competitiveness rather than isolated process issues

### 1. High CVs per Hire – Cross Year Pattern
In 2024, high CVs volume intensive roles were primarily concentrated in:
- Senior HQ functions (Marketing Head, Finance Head, HRBP, Investment Analyst)
- Specialized roles (Software Support, Corporate Investment)
- Selected Adult English commercial roles

In 2025, the pattern remains similar, with concentration in:
- Group HQ strategic/technical roles (Digital Marketing Specialist, Data Engineer, Strategy, Commercial Solution)
- Adult English commercial and education related roles (Branch Sales Manager, Sales Consultant, Teacher, Student Services)

Cross year consistency shows that hiring inefficiency is role structure driven rather than year specific fluctuation

### 2. Is Offer Rejection the Key Reason?
Across both years, only a minority of high CV per hire roles overlap with high rejection positions. Several roles show high rejection rates but do not require excessive CV volume. Offer rejection contributes in selected cases but does not systematically drive CV inefficiency

### *Top 10 Positions – Highest CVs per Hire vs Highest Offer Rejection Rate (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/1b6d5479662b2f1bce0dd133bfd2bbb6c1a4b340/BU%20-%20Top%2010%20positions%20with%20most%20CVs%20per%20Hire%20%26%20Rejection%20rate%20(2024)%20-%2055%25%20image.png)

### *Top 10 Positions – Highest CVs per Hire vs Highest Offer Rejection Rate (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/27550888d29e9ef7a7b9312f3ba6df51e6b765c4/BU%20-%20Top%2010%20positions%20with%20most%20CVs%20per%20Hire%20%26%20Rejection%20rate%20(2025)%20-%2055%25%20image.png)

### 3. Is Screening Volume the Main Driver?
In both years, roles requiring high CV volume to generate interviews do not significantly overlap with those requiring high CVs per hire. This indicates front end screening inefficiency is not the primary root cause. High CV requirement is not simply due to poor CV quality inflow

### *Top 10 Positions with the Highest CVs per Interview (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/f14d595e1396c1a778a3041513683d45c41c2570/BU%20-%20Top%2010%20positions%20with%20most%20CVs%20per%20Interview%20(2024).png)

### *Top 10 Positions with the Highest CVs per Interview (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/f14d595e1396c1a778a3041513683d45c41c2570/BU%20-%20Top%2010%20positions%20with%20most%20CVs%20per%20Interview%20(2025).png)

### 4. Mid Funnel Conversion Impact
In 2025 especially, several high CV intensive roles also show high Interview per Offer ratios (e.g., Strategy, Commercial Solution, Teacher, Student Services). This suggests mid funnel inefficiency partially explains hiring effort, particularly for strategic and education related roles. However, since overlap remains limited, this still does not fully account for the pattern

### *Top 10 Positions with the Highest Interviews per Offer (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/f14d595e1396c1a778a3041513683d45c41c2570/BU%20-%20Top%2010%20positions%20with%20most%20Interview%20per%20Offer%20(2024).png)

### *Top 10 Positions with the Highest Interviews per Offer (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/f14d595e1396c1a778a3041513683d45c41c2570/BU%20-%20Top%2010%20positions%20with%20most%20Interview%20per%20Offer%20(2025).png)

## Core Cross Year Insight
High CV per hire roles across 2024 2025 are:
- Concentrated in high complexity and strategic functions
- Frequently HQ-based
- Sensitive to market supply demand imbalance
- Partially affected by mid funnel conversion challenges

The data suggests structural factors such as:
- Talent scarcity (Data, Strategy, Digital roles)
- Compensation competitiveness
- Elevated hiring standards
- Expectation misalignment between hiring managers and market reality

## Recommendations
The consistent concentration of high CVs per hire in strategic and Head Quarter roles across two consecutive years signals a structural hiring challenge, not a temporary funnel fluctuation. Continuing to apply volume based recruitment strategies to high complexity roles will likely increase sourcing effort without materially improving hiring outcomes

Leadership intervention is required in three areas:
- Recalibrate role expectations vs. market reality for strategic and technical positions
- Shift from volume sourcing to precision sourcing (targeted channels, headhunting, niche pools)
- Strengthen hiring manager alignment and decision discipline to reduce mid-funnel inefficiencies.

Without differentiated strategy by job complexity, recruitment effort will continue to scale disproportionately with limited return. The data indicates that efficiency gains will not come from “more CVs,” but from smarter targeting and tighter decision alignment

## III. PIC Performance Analysis - 2024 & 2025

Across 2024 - 2025, PIC performance shows increasing dispersion between high efficiency & low efficiency recruiters. While certain PICs consistently demonstrate strong screen to join success rates & balanced funnel conversion, performance gaps widen in BU specific hiring particularly in Sales and HQ roles. Bubble size comparison (CVs per Hire) further indicates that high success rate does not always equate to sourcing efficiency, highlighting the need for workload balancing & role based performance calibration

### 1. Overall PIC Performance (2024 vs 2025)
- 2025 shows greater variance in success rates across PICs compared to 2024
- Some PICs improved conversion efficiency but handled fewer positions
- Others handled high volume but with lower screen → interview or interview → offer rates

### *Overall PIC Performance (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Performance%202024.png)

### *Overall PIC Performance (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/615ecf8eb3095fae88e9bc48026092b57a0756db/PIC%20-%20HQ%20Performance%20in%202025.png)

Bubble analysis indicates that higher CVs per Hire is often associated with: strategic/Head Quarter (HQ) roles & complex commercial positions. Efficiency and workload are not evenly distributed. High-performing PICs are not necessarily those handling the most complex or volume heavy roles. Performance evaluation should consider both funnel efficiency & role complexity

### 2. Sales Hiring – Adult English Business Unit (2024 vs 2025)
- 2024: Performance relatively clustered, no extreme outliers
- 2025: Clear divergence one PIC shows very high interview → offer rate but low HR screen → interview rate
- Increased bubble size for certain PICs suggests heavier sourcing effort per hire. Sales hiring in Adult English became more polarized in 2025

### *Sales Hiring – Adult English Business Unit (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Sales%20hiring%20performance%20for%20Adult%20English%20(2024).png)

### *Sales Hiring – Adult English Business Unit (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Sales%20hiring%20performance%20for%20Adult%20English%20(2025).png)

### Insights
- Possible inconsistency in candidate screening standards
- Potential misalignment between early screening & hiring manager expectations
- Some PICs may rely on narrower pipelines but achieve stronger late stage conversion

### 3. Sales Hiring – Kids English Business Unit (2024 vs 2025)
- 2024: Moderate spread; no extreme inefficiency
- 2025: One PIC handles significantly more positions than average
- Conversion rates fluctuate more widely compared to 2024.Workload concentration risk observed in 2025

### *Sales Hiring – Kids English Business Unit (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Sales%20hiring%20performance%20for%20Kids%20English%20(2024).png)

### *Sales Hiring – Kids English Business Unit (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Sales%20hiring%20performance%20for%20Kids%20English%20(2025).png)

### Insights
- Over reliance on specific PICs may increase operational risk
- Efficiency gains may reflect experience accumulation or better hiring calibration

### 4. Sales Hiring – STEM Program (2024 vs 2025)
Performance metrics highly sensitive to small sample size
- Smaller team size → higher volatility
- Success rate spikes in 2025 but based on low position volume
- Bubble sizes suggest relatively high CV effort per hire

### *Sales Hiring – Stem Program Business Unit (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Stem%20performance%202024.png)

### *Sales Hiring – Stem Program Business Unit (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20Stem%20performance%202025.png)

## Interpretation
- KPI comparison year over year must consider base volume
- Efficiency improvements may not yet be structurally stable

### 5. Head Quarter Hiring (2024 vs 2025)
- Highest dispersion in funnel efficiency
- Some PICs demonstrate strong HR screen → interview but weak interview → offer
- CVs per Hire remains relatively high compared to Sales BUs.
- HQ hiring remains structurally more complex

### *HQ Hiring Performance (2024)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20HQ%20Performance%20in%202024.png)

### *HQ Hiring Performance (2025)*

![image alt](https://github.com/mkhanhvo/Recruitment-efficiency-analysis-report/blob/351f29f8b9150a07d99c9d61e3b820a5feb60dfc/PIC%20-%20HQ%20Performance%20in%202025.png)

### Insights
- Strategic/technical roles likely driving conversion volatility
- Decision making friction may impact interview → offer stage

## Cross Year Core Insight
- Performance dispersion increases in 2025
- Sales BUs show more stable funnel structures compared to HQ
- High CV effort per hire is frequently associated with strategic roles rather than recruiter inefficiency
- Workload distribution across PICs becomes increasingly uneven

## Recommendations
### 1. Differentiate PIC KPIs by Role Complexity
- Do not evaluate HQ & Sales PICs using identical efficiency benchmarks
- Introduce role weighted performance index

### 2. Balance Workload Distribution
- Avoid concentration of high-complexity roles on few PICs
- Monitor average positions handled per PIC to reduce burnout risk

### 3. Strengthen Early Funnel Calibration (Sales BUs)
- Standardize screening criteria
- Align screening benchmarks with hiring managers
- Reduce unnecessary CV volume for interview generation.

### 4. Improve Mid-Funnel Governance (HQ)
- Implement structured evaluation scorecards
- Shorten decision turnaround time
- Pre-align compensation & expectation to reduce late stage friction

# Overall Summary

Across 2024 & 2025, hiring performance analysis consistently indicates that inefficiencies are structurally concentrated in high complexity, strategic & HQ based roles rather than driven by sourcing volume alone. While screening intensity, offer rejection & mid-funnel conversion contribute in selected cases, none of these factors independently explains the sustained high CVs per hire pattern. Instead, the data suggests systemic challenges linked to talent market scarcity, expectation misalignment &decision-stage friction

At the BU level, commercial & operational roles particularly in Sales demonstrate relatively stable and scalable funnel structures. In contrast, HQ & specialized roles show higher volatility, greater CV effort & more pronounced conversion dispersion. PIC performance analysis further reinforces that recruiter efficiency varies by role complexity and workload distribution rather than purely by individual capability. High success rates do not always correlate with lower CV effort, underscoring the importance of role weighted performance evaluation

Overall, the findings point to a critical shift in recruitment strategy: efficiency gains will not come from increasing CV inflow, but from smarter channel role alignment, earlier hiring manager calibration, differentiated KPIs by job complexity & stronger mid funnel governance. Without structural adjustments, hiring effort will continue to scale disproportionately for strategic roles, limiting overall talent acquisition efficiency & organizational agility
