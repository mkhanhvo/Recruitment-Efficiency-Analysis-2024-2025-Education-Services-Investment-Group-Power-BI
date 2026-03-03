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

In 2024, recruitment pipeline operated with relatively strong efficiency. Out of 11,931 screened candidates & 274 were successfully onboarded, resulting in a **Hiring Success Rate of 2.3%**. **Offer Acceptance reached 92.3%** indicating strong offer competitiveness and stable late stage conversion


<img width="1040" height="313" alt="image" src="https://github.com/user-attachments/assets/87f939c0-688b-437b-8a55-6f9ac8212ac5" />


In 2025, although screening volume increased significantly to 14,876 candidates (+25%), **total onboarded hires declined sharply** to 126. As a result, **Hiring Success Rate dropped to 0.8% (–63% YoY).** This indicates that the issue in 2025 is not pipeline volume but conversion effectiveness. 2025 reflects a pattern of increased effort but reduced output


<img width="1037" height="311" alt="image" src="https://github.com/user-attachments/assets/f819d4de-b2a2-4a19-89eb-28c02d4a0743" />

### 📌 Analysis 2. Pipeline Productivity Deterioration

Productivity indicators further confirm this shift. In 2024, 7 CVs were required to generate 1 interview, 6 interviews were required to secure 1 offer

#### *2024 Hiring Efficiency & Conversion*

<img width="1036" height="175" alt="image" src="https://github.com/user-attachments/assets/bd24ad5f-205e-4e3b-a667-9240ac545904" />

In 2025, screening efficiency declined significantly: **CVs per interview increased by 42.9%** and **interviews per offer surged by 66.7%** versus 2024. Recruiter effort has increased substantially while yield per stage has decreased. Although offer per hire remains at 1, **overall offer issuance has dropped** due to weakened upstream conversion. The recruitment engine is working harder but producing fewer outcomes. TopCV, CareerViet and LinkedIn remained key sources but offer conversion rates declined. Zalo and Employee Referral maintained high offer rates (>25%). Low conversion from Facebook, VNW and other boards suggests stricter source screening is needed

#### *2025 Hiring Efficiency & Conversion*

<img width="1040" height="169" alt="image" src="https://github.com/user-attachments/assets/bcb9bfc5-b18e-4cc1-9e8a-ac15351be7b5" />

### 📌 Analysis 3. Funnel Quality Deterioration
In 2024, the pipeline showed** healthy progression and conversion remained stable** across stages: 14.6% of screened candidates progressed to interview, 17.1% of interviews converted to offers & 92.3% of offers were accepted

#### *2024 Hiring Funnel & Performance Overview*

<img width="833" height="242" alt="image" src="https://github.com/user-attachments/assets/91d184d0-4148-4a14-8981-6707899cb0a4" />

In 2025, all major transitions weakened simultaneously: **screening → interview declined** to **10.4%, interview → offer declined** to **10.0%** & **offer acceptance dropped** to **81.3%.** This suggests a systemic decline rather than an isolated bottleneck. Candidate qualification at screening appears weaker, interview selectivity less precise & offer competitiveness lower than the prior year. Pipeline leakage increased at every stage

#### *2025 Hiring Funnel & Performance Overview*

<img width="836" height="242" alt="image" src="https://github.com/user-attachments/assets/a680d54f-6362-44b0-b7cc-f31b8f6ca5db" />

### 📌 Analysis 4. Business Unit Performance Shift
During 2024, **offer acceptance rates were consistently strong across Business Units.** Acceptance stability suggested competitive positioning and effective candidate engagement. By 2025, performance divergence emerged: Property Management fell to 75%, Adult English declined to 78.8%, Group HQ dropped to 70.3%, Kids English & STEM remained comparatively stable around 93–94%

Scatter analysis indicates that some units maintain moderate Interview → Offer rates but suffer from declining acceptance. This may point to compensation competitiveness, candidate experience inconsistency, or delayed decision cycles in certain units. Performance dispersion across BUs has widened

#### *2024 Offer Conversion Alignment by Business Unit in*

<img width="527" height="224" alt="image" src="https://github.com/user-attachments/assets/f9b3bb0d-d399-4116-935d-69b85ab48447" />

#### *2025 Offer Conversion Alignment by Business Unit*

<img width="522" height="224" alt="image" src="https://github.com/user-attachments/assets/5fb92357-562f-4408-a664-2c8f65e18330" />

### 🎯 Recommendations
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

During 2024, hiring output was relatively balanced across major sourcing channels. **TopCV & CareerViet generated the largest screening volumes while Employee Referral delivered strong hiring efficiency despite lower volume.** Although high volume platforms required greater screening effort, conversion performance remained within an acceptable range, indicating manageable quality dispersion across channels

<img width="1036" height="212" alt="image" src="https://github.com/user-attachments/assets/8c2496bc-4f93-4e84-8198-7801b435bff0" />

Looking at 2025, sourcing dynamics became more polarized. Screening volume increased across major job boards, yet **hiring contribution became increasingly concentrated in fewer channels.** High volume sources such as CareerViet & TopCV absorbed a disproportionate share of screening activity but delivered weaker hiring success rates. Meanwhile, **Employee Referral continued to demonstrate superior efficiency,** requiring fewer CVs and interviews per hire

The volume versus conversion comparison highlights a structural imbalance:** incremental screening effort did not produce proportional hiring gains**. Instead, effort intensity increased as reflected in higher CVs per Interview and Interviews per Offer ratios for several large channels. This suggests declining top of funnel quality and reduced mid stage selectivity rather than insufficient pipeline size

<img width="1038" height="217" alt="image" src="https://github.com/user-attachments/assets/be035d70-4825-43a8-8a17-6bf05de75ae4" />

### 📌 Analysis 2. Channel Performance Variance by Critical roles (Sales & Teacher)

For Sales roles, hiring efficiency deteriorated markedly from 2024 to 2025. While **TopCV remained the dominant source (48.3% in 2024 and 44.4% in 2025),** screening effort increased sharply: CVs per interview nearly tripled for TopCV (from 9 to 24) and more than doubled for CareerViet (from 16 to 37), indicating significant quality dilution in high volume channels. Hiring success rates declined in 2025 despite increased sourcing volume, reflecting rising input but lower yield. In contrast, **Employee Referral consistently delivered stronger conversion performance across both years,** with lower CV effort and higher success rates. Funnel data suggests that the primary **bottleneck lies in early stage qualification (Screen → Interview),** rather than offer stage acceptance

Overall, Sales hiring in 2025 became more volume driven but less efficient, reinforcing the need to rebalance sourcing strategy toward higher-quality, role aligned channels rather than relying heavily on broad job boards

### *Sales Source Effectiveness (2024)*

<img width="1037" height="211" alt="image" src="https://github.com/user-attachments/assets/615a8da5-8671-47a8-8ed2-abdcb7a5fa17" />

### *Sales Source Effectiveness (2025)*

<img width="1034" height="213" alt="image" src="https://github.com/user-attachments/assets/83e73452-059e-4630-871f-c092516f2747" />

This pattern is also evident in the Teacher position where channel contribution shifted significantly year over year. While **VTJ dominated hiring share in 2024, its sharp decline in 2025** highlights how source performance can fluctuate depending on role dynamics & sourcing strategy adjustments. In contrast, **TopCV strengthened its position as the primary hiring driver & Employee Referral emerged as a meaningful contributor,** suggesting improved alignment between channel quality & role requirements. Together, these findings emphasize that sourcing strategy should be calibrated at the job family level with ongoing performance monitoring to optimize conversion efficiency and hiring outcomes

Overall, the data suggests that sourcing inefficiency in 2025 is driven primarily by channel mix quality rather than absolute screening volume. Without recalibrating allocation toward consistently high-yield channels, additional sourcing effort is likely to amplify recruiter workload rather than improve hiring output

#### *Teacher Source Effectiveness (2024)*

<img width="1035" height="211" alt="image" src="https://github.com/user-attachments/assets/f52b4cba-f65b-4174-aa93-c3df91b82191" />

#### *Teacher Source Effectiveness (2025)*

<img width="1037" height="215" alt="image" src="https://github.com/user-attachments/assets/dbb6493e-3873-48e4-9b71-64e290db5a27" />

### 🎯 Recommendations
#### 1️⃣ Rebalance Channel Allocation Toward High-Yield Sources
- Gradually reduce reliance on high volume, low conversion job boards (e.g., TopCV, CareerViet for Sales)
- Expand Employee Referral incentives for Sales & Teacher roles, given its consistently superior conversion efficiency
- Set minimum conversion benchmarks (e.g., Screen → Interview rate threshold) for continued budget allocation per source

#### 2️⃣ Strengthen Early-Stage Qualification Controls (Screen → Interview)
- Introduce stricter screening alignment sessions for Sales roles before mass sourcing
- Define target CV → interview efficiency bands per job family (e.g., flag when CVs per Interview exceed historical range)
- Monitor top of funnel quality weekly during high growth periods

#### 3️⃣ Implement Role-Specific Sourcing Strategy
- Develop separate sourcing mix targets for Sales vs. Teacher roles
- Review annual channel performance at the job family level rather than overall averages
- Reallocate sourcing investment dynamically based on role level conversion yield

#### 4️⃣ Introduce Volume to Yield Monitoring Framework
- Track incremental hires per additional 100 screened CVs by source
- Flag sources where screening effort rises without proportional hiring gain
- Incorporate yield efficiency KPIs into recruiter and BU performance dashboards
- Rationale: 2025 shows rising input but declining output, indicating structural inefficiency rather than pipeline shortage

#### 5️⃣ Protect Recruiter Capacity During Expansion Phases
- Pre-define sourcing caps for channels exceeding CV per Interview thresholds
- Shift recruiter effort toward higher probability pipelines instead of scaling screening volume

### 3️⃣ Business Unit & Position Efficiency Analysis

Across 2024 & 2025, high CVs per hire consistently concentrate in strategic, technical and Head Quarter based roles with selected commercial positions in Adult English also requiring significant hiring effort. Funnel diagnostics indicate that neither screening intensity nor offer rejection rate fully explains this inefficiency. While mid funnel conversion (interview → offer) contributes in certain roles, the pattern suggests more structural challenges, such as talent scarcity, expectation misalignment & market competitiveness rather than isolated process issues

#### *2024 Business & Position - Level Recruitment Performance*

<img width="1036" height="380" alt="image" src="https://github.com/user-attachments/assets/50337680-453b-48f2-ab3c-ce60c0849c16" />

#### *2025 Business & Position - Level Recruitment Performance*

<img width="1035" height="382" alt="image" src="https://github.com/user-attachments/assets/6b0ed427-fa58-4782-a785-00b0e3f820aa" />

### 📌 Analysis 1. High CVs per Hire – Cross Year Pattern
In 2024, high CVs volume intensive roles were primarily concentrated in:
- Senior HQ functions (Marketing Head, Finance Head, HRBP, Investment Analyst)
- Specialized roles (Software Support, Corporate Investment)
- Selected Adult English commercial roles

In 2025, the pattern remains similar, with concentration in:
- Group HQ strategic/technical roles (Digital Marketing Specialist, Data Engineer, Strategy, Commercial Solution)
- Adult English commercial and education related roles (Branch Sales Manager, Sales Consultant, Teacher, Student Services)

Cross year consistency shows that hiring inefficiency is role structure driven rather than year specific fluctuation

### 📌 Analysis 2. Is Offer Rejection the Key Reason?
Across both years, only a minority of high CV per hire roles overlap with high rejection positions. Several roles show high rejection rates but do not require excessive CV volume. Offer rejection contributes in selected cases but does not systematically drive CV inefficiency

#### *Top 10 Positions – Highest CVs per Hire vs Highest Offer Rejection Rate (2024)*

<img width="725" height="257" alt="image" src="https://github.com/user-attachments/assets/1d061443-36fc-4700-a57f-1d43ab0b9f2c" />

#### *Top 10 Positions – Highest CVs per Hire vs Highest Offer Rejection Rate (2025)*

<img width="725" height="260" alt="image" src="https://github.com/user-attachments/assets/8c7d3037-fda8-4c94-945c-12c83a07b5eb" />

### 📌 Analysis 3. Is Screening Volume the Main Driver?
In both years, roles requiring high CV volume to generate interviews do not significantly overlap with those requiring high CVs per hire. This indicates front end screening inefficiency is not the primary root cause. High CV requirement is not simply due to poor CV quality inflow

#### *Top 10 Positions with the Highest CVs per Interview (2024)*

<img width="365" height="261" alt="image" src="https://github.com/user-attachments/assets/02297e90-f16e-4476-a81a-8131a8280b39" />

### *Top 10 Positions with the Highest CVs per Interview (2025)*

<img width="362" height="261" alt="image" src="https://github.com/user-attachments/assets/b42e4668-d7ed-4736-b4af-ed1255b63c81" />

### 📌 Analysis 4. Mid Funnel Conversion Impact
In 2025 especially, several high CV intensive roles also show high Interview per Offer ratios (e.g., Strategy, Commercial Solution, Teacher, Student Services). This suggests mid funnel inefficiency partially explains hiring effort, particularly for strategic and education related roles. However, since overlap remains limited, this still does not fully account for the pattern

#### *Top 10 Positions with the Highest Interviews per Offer (2024)*

<img width="364" height="258" alt="image" src="https://github.com/user-attachments/assets/1822747d-77ac-469c-b75f-a927c1f45541" />

#### *Top 10 Positions with the Highest Interviews per Offer (2025)*

<img width="363" height="257" alt="image" src="https://github.com/user-attachments/assets/0ed95f37-b989-4722-bd7d-f1bcabb49f98" />

Across 2024–2025, roles with consistently high CV per hire ratios were primarily concentrated in complex, strategic and HQ-based functions. These positions appear structurally constrained by talent scarcity (notably in Data, Strategy, and Digital domains), heightened hiring standards and market supply demand imbalance. Conversion friction in the mid funnel further amplified screening effort without proportional hiring gains. Overall, the pattern suggests that inefficiency is driven less by pipeline volume and more by structural factors such as compensation competitiveness + expectation misalignment between hiring managers and market realities

### 🎯 Recommendations
- Conduct quarterly expectation calibration workshops with hiring managers for strategic/HQ roles to align requirements with market supply realities
- Reduce job board allocation for high complexity roles and reallocate budget to precision sourcing (headhunting, niche platforms, referral campaigns)
- Set efficiency guardrails (e.g., max CVs per interview threshold) to trigger sourcing strategy review when exceeded
- Implement structured mid-funnel checkpoints (post-screen review + post-interview alignment within 48h) to minimize unnecessary CV recycling
- Introduce role complexity-based hiring playbooks, differentiating sourcing and evaluation strategy by job family rather than applying a uniform recruitment model

### 4️⃣ PIC Performance Analysis

Across 2024-2025, PIC performance shows increasing dispersion between high efficiency & low efficiency recruiters. While certain PICs consistently demonstrate strong screen to join success rates & balanced funnel conversion, performance gaps widen in BU specific hiring particularly in Sales and HQ roles. Bubble size comparison (CVs per Hire) further indicates that high success rate does not always equate to sourcing efficiency, highlighting the need for workload balancing & role based performance calibration

#### *Recruiter Performance & Workload Distribution (2024)*

<img width="1034" height="361" alt="image" src="https://github.com/user-attachments/assets/d55e6788-87d0-4e8c-869e-9eb416589c71" />

#### *Recruiter Performance & Workload Distribution (2025)*

<img width="1031" height="360" alt="image" src="https://github.com/user-attachments/assets/c5055eb7-c806-42de-b5e5-d34c601c1530" />

### 📌 Analysis 1. Overall PIC Performance
- 2025 shows greater variance in success rates across PICs compared to 2024
- Some PICs improved conversion efficiency but handled fewer positions
- Others handled high volume but with lower screen → interview or interview → offer rates

Bubble analysis indicates that higher CVs per Hire is often associated with: strategic/Head Quarter (HQ) roles & complex commercial positions. Efficiency and workload are not evenly distributed. High-performing PICs are not necessarily those handling the most complex or volume heavy roles. Performance evaluation should consider both funnel efficiency & role complexity

#### *Overall PIC Performance (2024)*

<img width="745" height="199" alt="image" src="https://github.com/user-attachments/assets/dac8e29c-f39a-4bd5-9820-0c90f4a64e24" />

#### *Overall PIC Performance (2025)*

<img width="746" height="199" alt="image" src="https://github.com/user-attachments/assets/1bb37f5d-d41a-4825-9a5a-3c5ad967a929" />

### 📌 Analysis 2. Sales Hiring – Adult English Business Unit
In 2024, recruiter performance remained relatively clustered, with no extreme outliers in conversion patterns or effort levels

By 2025, however, clear divergence emerged: one PIC demonstrated a notably high Interview → Offer rate despite a low HR Screen → Interview rate, suggesting stronger late stage selectivity but weaker early qualification. The increase in bubble size for certain PICs indicates heavier sourcing effort per hire, particularly within Adult English Sales where hiring outcomes became more polarized. These patterns point to potential inconsistencies in screening standards, misalignment between early stage qualification, hiring manager expectations and differing sourcing strategies where some recruiters rely on narrower pipelines yet achieve stronger late stage conversion efficiency

#### *Sales Hiring – Adult English Business Unit (2024)*

<img width="745" height="200" alt="image" src="https://github.com/user-attachments/assets/30da8f84-04cb-47ac-ade1-eff8f9bd9d54" />

#### *Sales Hiring – Adult English Business Unit (2025)*

<img width="748" height="202" alt="image" src="https://github.com/user-attachments/assets/f7f9adbf-44c2-4231-8f9f-ee7c5bc2076c" />

### 📌 Analysis 3. Sales Hiring – Kids English Business Unit
In 2024, recruiter performance and workload were relatively balanced, with no major inefficiencies

By 2025, divergence became more visible: one PIC handled significantly more positions than average and conversion rates varied more widely across the team. This suggests emerging workload concentration risk and potential over reliance on specific recruiters, while improved efficiency among some PICs may reflect experience gains or better hiring calibration

#### *Sales Hiring – Kids English Business Unit (2024)*

<img width="746" height="205" alt="image" src="https://github.com/user-attachments/assets/ebcd6e01-4a6e-4d22-a702-6a1605272d82" />

#### *Sales Hiring – Kids English Business Unit (2025)*

<img width="750" height="202" alt="image" src="https://github.com/user-attachments/assets/6fafb67a-3e42-4358-a1c1-6f779492e489" />

### 🎯 Recommendations
Rebalance workload distribution to reduce concentration risk and avoid over reliance on specific recruiters handling disproportionately high volumes
- Standardize early stage screening criteria to minimize conversion variance across PICs, particularly at the Screen → Interview stage
- Evaluate recruiter performance using weighted metrics that account for role complexity, hiring volume and funnel efficiency rather than raw success rate alone
- Implement periodic funnel calibration reviews to detect misalignment between screening quality and hiring manager expectations
- Capture and share best practices from recruiters with strong late stage conversion to improve overall team consistency

## 🔎 Final Conclusion & Recommendations 

Across 2024–2025, hiring inefficiencies are structurally concentrated in high complexity, driven more by talent scarcity, expectation misalignment and decision stage friction than by sourcing volume alone.Commercial roles like Sales show relatively stable funnels, while strategic and specialized positions require higher CV effort, display greater conversion volatility. PIC performance differences reflect role complexity and workload distribution rather than pure individual capability. Efficiency gains will come from smarter channel-role alignment, earlier hiring manager calibration and differentiated KPIs by job complexity—not from increasing CV volume

Based on these conclusions, the following recommendations are proposed for the HR team:

### 1️⃣ Differentiate PIC KPIs by Role Complexity
- Do not evaluate HQ & Sales PICs using identical efficiency benchmarks
- Introduce role weighted performance index

### 2️⃣ Balance Workload Distribution
- Avoid concentration of high-complexity roles on few PICs
- Monitor average positions handled per PIC to reduce burnout risk

### 3️⃣ Strengthen Early Funnel Calibration (Sales BUs)
- Standardize screening criteria
- Align screening benchmarks with hiring managers
- Reduce unnecessary CV volume for interview generation.

### 4️⃣ Improve Mid-Funnel Governance (HQ)
- Implement structured evaluation scorecards
- Shorten decision turnaround time
- Pre-align compensation & expectation to reduce late stage friction
