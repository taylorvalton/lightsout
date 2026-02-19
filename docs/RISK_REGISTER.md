# LightsOut Risk Register

**NGen Project 14091** | **Last Updated:** Q8 (February 2026)

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

## Active Risks — Sorted by Q8 Mitigated Score (Descending)

### Critical / High Risks (Score 24+)

| # | Category | Risk Event | Owner | Strategy | Inherent Score | Q7 Score | Q8 Score | Trend |
|---|----------|-----------|-------|----------|---------------|----------|----------|-------|
| **5** | Technical | MPA design takes longer than expected and/or costs more than projected | Sidac | Mitigate | 64 | 48 | **36** | Decreasing |
| **6** | Technical | Bottle/pump insertion speed will not meet throughput requirements | Petra | Manage | 96 | 40 | **32** | Decreasing |
| **17** | Technical | Lack of shared knowledge between teams delaying AI + robotics integration | Analytika | Mitigate | 48 | 32 | **32** | Stable |
| **1** | Operational | Human safety risk working with COBOTs in production environment | Petra | Avoid | 128 | 32 | **32** | Stable |
| **3** | Managerial | Insufficient resource bandwidth or loss of key personnel | Petra | Mitigate | 48 | 32 | **24** | Decreasing |
| **15** | Technical | Recipe creation still requires manual recalibration after AI generation | Petra | Manage | 64 | 24 | **24** | Stable |

### Medium Risks (Score 9-23)

| # | Category | Risk Event | Owner | Strategy | Inherent Score | Q7 Score | Q8 Score | Trend |
|---|----------|-----------|-------|----------|---------------|----------|----------|-------|
| **20** | Managerial | Procurement delays due to bandwidth, financial constraints, or wrong parts | Petra | Mitigate | 32 | 30 | **20** | Decreasing |
| **14** | Technical | Excessive downtime from mechanical or software failure in production | Petra | Mitigate | 48 | 24 | **18** | Decreasing |
| **4** | Technical | Image recognition software takes longer/more resources than anticipated | Analytika | Mitigate | 64 | 16 | **16** | Stable |
| **9** | Regulatory | Manufacturing standards or regulation changes affecting project | Petra | Mitigate | 32 | 16 | **16** | Stable |
| **18** | Technical | Messaging standard for manufacturing communication not defined | Analytika | Mitigate | 48 | 16 | **16** | Stable |
| **21** | Technical | Suction EOAT bellows cup degradation under continuous production | Sidac | Mitigate | 48 | — | **16** | NEW |
| **22** | Technical | Centering nest 3D print tolerances drift affecting insertion precision | Sidac | Mitigate | 32 | — | **12** | NEW |
| **23** | Technical | FlexiBowl puck design iteration delays across 5+ product families | Sidac | Mitigate | 32 | — | **12** | NEW |

### Low Risks (Score 1-8)

| # | Category | Risk Event | Owner | Strategy | Inherent Score | Q7 Score | Q8 Score | Trend |
|---|----------|-----------|-------|----------|---------------|----------|----------|-------|
| 2 | Managerial | Personnel issues between consortium collaborators | Petra | Transfer | 32 | 8 | 8 | Stable |
| 7 | Commercial | Vendors not complying with contract terms | Petra | Manage | 8 | 8 | 8 | Stable |
| 10 | Financial | Unforeseen spike in project costs | Petra | Mitigate | 16 | 8 | 8 | Stable |
| 8 | Resource | Shortage of high-skilled labor for maintenance/operation | Petra | Manage | 8 | 4 | 4 | Stable |
| 11 | Financial | Decrease in product demand / no payback on investment | Petra | Transfer | 4 | 4 | 4 | Stable |
| 12 | Managerial | Key manager absence costing time and money | Analytika | Manage | 6 | 4 | 4 | Stable |
| 13 | Redundancy | Power outage for extended period disrupting production | Petra | Mitigate | 4 | 4 | 4 | Stable |
| 16 | Technical | Insufficient access to product samples for AI vision training | Analytika | Mitigate | 16 | 4 | 4 | Decreasing |
| 19 | Managerial | Project not starting on-time | Petra | Mitigate | 12 | 4 | 4 | Stable |

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

## Risk Trend Analysis (Q1 → Q8)

### Improving Risks (Q8)

| Risk | Q1 | Q5 | Q7 | Q8 | Commentary |
|------|-----|-----|-----|-----|-----------|
| **#5 (MPA Design)** | 16 | 24 | 48 | **36** | Pump insertion retrofit (WBS 3.22) approved and underway. MPA modification work package (3.22.3) addresses tipping problem with guide rails and anti-tip mechanisms. |
| **#6 (Throughput)** | 32 | 32 | 40 | **32** | Multi-pick suction EOAT design validated in simulation. Sequential insertion approach (7.9-10.5s) fits within 12s COBOT 2 cycle budget at 30 PPM. |
| **#3 (Resources)** | 16 | 16 | 32 | **24** | End-of-line componentry (3.14-3.17) deferred to 2027, freeing team bandwidth for pump insertion priority. |
| **#20 (Procurement)** | 18 | 18 | 30 | **20** | FlexiBowl 800 order placed; Photoneo PhoXi M selected over Pickit M-HD (better recipe engine compatibility). Key procurement decisions resolved. |
| **#14 (Downtime)** | 18 | 18 | 24 | **18** | Bellows suction cups + centering nests eliminate mechanical finger gripper failure modes. Predictable wear pattern (cups are consumable). |
| **#16 (AI Training Data)** | 8 | 4 | 4 | **4** | Stable — adequate product samples and training data available. |

### New Risks (Q8)

| Risk | Q8 Score | Commentary |
|------|----------|-----------|
| **#21 (Suction Cup Degradation)** | **16** | Bellows cups are consumables; need maintenance schedule. Mitigated by spring-loaded mounts and spare inventory. |
| **#22 (3D Print Tolerance Drift)** | **12** | Centering nests require dimensional accuracy. Mitigated by periodic calibration and SPC monitoring. |
| **#23 (Puck Design Iterations)** | **12** | 5+ product families require individual puck designs. Mitigated by parametric CAD approach and rapid 3D printing. |

### Net Risk Score Change: **-42 points** (5 risks improved, 3 new risks added)

---

## Mitigation Actions — Q9 Priority

| Priority | Risk | Action | Owner | Target |
|----------|------|--------|-------|--------|
| 1 | #5, #6 | Complete WBS 3.22.1 (parts presentation) and begin 3.22.2 (EOAT fabrication) | Sidac | Q9 |
| 2 | #21 | Establish bellows cup replacement schedule and spare parts inventory | Sidac | Q9 |
| 3 | #17 | Continue bi-weekly Analytika-Sidac integration syncs; begin 3D vision evaluation (3.22.4.1) | All | Q9-Q10 |
| 4 | #15 | Validate recipe engine parametric detection profiles with first pump family | Analytika | Q9-Q10 |
| 5 | #22, #23 | Validate centering nest dimensional tolerance with SPC; complete puck designs for top 3 product families | Sidac | Q9 |
