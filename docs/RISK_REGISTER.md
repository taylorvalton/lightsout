# LightsOut Risk Register

**NGen Project 14091** | **Last Updated:** Q7 (November 2025)

---

## Scoring Methodology

Risks are scored using a **Likelihood x Impact** matrix:

| Likelihood \ Impact | 2 (Low) | 4 (Med-Low) | 8 (Medium) | 16 (High) | 32 (Extreme) |
|---------------------|---------|-------------|------------|-----------|---------------|
| **5 - Probable** | 10 | 20 | 40 | 80 | 160 |
| **4 - Likely** | 8 | 16 | 32 | 64 | 128 |
| **3 - Possible** | 6 | 12 | 24 | 48 | 96 |
| **2 - Unlikely** | 4 | 8 | 16 | 32 | 64 |
| **1 - Improbable** | 2 | 4 | 8 | 16 | 32 |

**Risk Score = Likelihood x Impact**

**Thresholds:** Low (1-8) | Medium (9-24) | High (25-48) | Critical (49+)

---

## Active Risks — Sorted by Q7 Mitigated Score (Descending)

### Critical / High Risks (Score 24+)

| # | Category | Risk Event | Owner | Strategy | Inherent Score | Q7 Score | Trend |
|---|----------|-----------|-------|----------|---------------|----------|-------|
| **5** | Technical | MPA design takes longer than expected and/or costs more than projected | Sidac | Mitigate | 64 | **48** | Increasing |
| **6** | Technical | Bottle/pump insertion speed will not meet throughput requirements | Petra | Manage | 96 | **40** | Increasing |
| **3** | Managerial | Insufficient resource bandwidth or loss of key personnel | Petra | Mitigate | 48 | **32** | Increasing |
| **17** | Technical | Lack of shared knowledge between teams delaying AI + robotics integration | Analytika | Mitigate | 48 | **32** | Stable |
| **1** | Operational | Human safety risk working with COBOTs in production environment | Petra | Avoid | 128 | **32** | Stable |
| **20** | Managerial | Procurement delays due to bandwidth, financial constraints, or wrong parts | Petra | Mitigate | 32 | **30** | Increasing |
| **14** | Technical | Excessive downtime from mechanical or software failure in production | Petra | Mitigate | 48 | **24** | Increasing |
| **15** | Technical | Recipe creation still requires manual recalibration after AI generation | Petra | Manage | 64 | **24** | Increasing |

### Medium Risks (Score 9-23)

| # | Category | Risk Event | Owner | Strategy | Inherent Score | Q7 Score | Trend |
|---|----------|-----------|-------|----------|---------------|----------|-------|
| **4** | Technical | Image recognition software takes longer/more resources than anticipated | Analytika | Mitigate | 64 | **16** | Stable |
| **9** | Regulatory | Manufacturing standards or regulation changes affecting project | Petra | Mitigate | 32 | **16** | Stable |
| **18** | Technical | Messaging standard for manufacturing communication not defined | Analytika | Mitigate | 48 | **16** | Stable |

### Low Risks (Score 1-8)

| # | Category | Risk Event | Owner | Strategy | Inherent Score | Q7 Score | Trend |
|---|----------|-----------|-------|----------|---------------|----------|-------|
| 2 | Managerial | Personnel issues between consortium collaborators | Petra | Transfer | 32 | 8 | Stable |
| 7 | Commercial | Vendors not complying with contract terms | Petra | Manage | 8 | 8 | Stable |
| 10 | Financial | Unforeseen spike in project costs | Petra | Mitigate | 16 | 8 | Stable |
| 8 | Resource | Shortage of high-skilled labor for maintenance/operation | Petra | Manage | 8 | 4 | Stable |
| 11 | Financial | Decrease in product demand / no payback on investment | Petra | Transfer | 4 | 4 | Stable |
| 12 | Managerial | Key manager absence costing time and money | Analytika | Manage | 6 | 4 | Stable |
| 13 | Redundancy | Power outage for extended period disrupting production | Petra | Mitigate | 4 | 4 | Stable |
| 16 | Technical | Insufficient access to product samples for AI vision training | Analytika | Mitigate | 16 | 4 | Decreasing |
| 19 | Managerial | Project not starting on-time | Petra | Mitigate | 12 | 4 | Stable |

---

## IP / Freedom to Operate Risks

### Background IP (BIP)

| Asset | Description | Owner | FTO Risk Score | Strategy | Notes |
|-------|-------------|-------|---------------|----------|-------|
| BIP 1 | Mechanical Parts Aggregation | Sidac | 4 | Accept | Trade secret; low FTO risk |
| BIP 2 | Computer Vision Software | Sidac | 4 | Accept | Trade secret; low FTO risk |
| BIP 3 | End of Arm Tooling | Sidac | 6 | Mitigate | Not unique to Petra; will keep as trade secret; can adapt/license if patent infringed |
| BIP 4 | Production Line Workflow | Petra | 2 | Mitigate | Trade secret; low risk |
| BIP 5 | COBOT Hardware/Software (UR5e, UR10e) | Universal Robots | 4 | Accept | Licensed commercial product; patent + copyright protected by UR |

### Foreground IP (FIP)

| Asset | Description | Owner | FTO Risk Score | Strategy | Notes |
|-------|-------------|-------|---------------|----------|-------|
| FIP 1 | Improved Computer Vision for Product Selection | Petra | 4 | Accept | Copyright + trade secret |
| FIP 2 | Improved End of Arm Tooling | Petra | **12** | Mitigate | Industrial design + patent planned; custom fingertip designs |
| FIP 3 | Improved Production Line Workflow | Petra | 4 | Mitigate | Trade secret + know-how (MPA redesign by Sidac) |
| FIP 4 | Data from Closure Insertion System | Petra | 2 | Accept | Copyright + trade secret |
| FIP 5 | In-Line Inspection System Software | Petra | 4 | Accept | Copyright + trade secret |
| FIP 6 | Data for In-Line Inspection System | Petra | 2 | Accept | Trade secret + copyright |
| FIP 7 | Case Packing System Software | Petra | 4 | Accept | Trade secret + copyright |
| FIP 8 | AI Algorithms (CNN, GD&T, Kinematic, Stereo Vision + PLC) | Petra | **12** | Accept | Patent + trade secret; prior art search by Gowling WLG found no existing technology |
| FIP 9 | Data for Case Packing System | Petra | 2 | Accept | Copyright + trade secret |

---

## Risk Trend Analysis (Q1 → Q7)

### Worsening Risks

| Risk | Q1 | Q3 | Q5 | Q7 | Commentary |
|------|-----|-----|-----|-----|-----------|
| **#5 (MPA Design)** | 16 | 16 | 24 | **48** | Tipping problem with tall caps/pumps discovered in Q6; elevated significantly. Pump insertion redesign is the primary mitigation. |
| **#6 (Throughput)** | 32 | 32 | 32 | **40** | Linked to insertion system errors; new product introduction causing failures. FlexiBowl + EOAT upgrade expected to mitigate. |
| **#3 (Resources)** | 16 | 16 | 16 | **32** | Team bandwidth stretched by insertion redesign effort on top of existing workstreams. |
| **#20 (Procurement)** | 18 | 18 | 18 | **30** | Tariff uncertainty and vendor lead times (FlexiBowl 12-16 weeks) contributing factors. |
| **#14 (Downtime)** | 18 | 18 | 18 | **24** | Insertion system errors causing unplanned downtime; changeover still manual in some areas. |

### Improving Risks

| Risk | Q1 | Q7 | Commentary |
|------|-----|-----|-----------|
| **#16 (AI Training Data)** | 8 | **4** | Access to product samples resolved; QC inspection workflow providing adequate training data. |

---

## Mitigation Actions — Q8 Priority

| Priority | Risk | Action | Owner | Target |
|----------|------|--------|-------|--------|
| 1 | #5, #6, #14 | Implement pump insertion system redesign per R.Commander analysis (FlexiBowl, Pickit 3D, custom pucks, EOAT upgrade) | Petra/Sidac | Q8-Q9 |
| 2 | #20 | Place FlexiBowl 800 order immediately (12-16 week lead time); secure Robotiq and OnRobot demo units | Petra | Q8 |
| 3 | #3 | Prioritize insertion redesign; defer non-critical tasks to free team bandwidth | Petra | Q8 |
| 4 | #17 | Schedule bi-weekly integration syncs between Analytika and Sidac on vision/PLC interface | All | Ongoing |
| 5 | #15 | Validate AI recipe accuracy on existing products; define acceptance criteria for autonomous recipe creation | Analytika | Q8-Q9 |
