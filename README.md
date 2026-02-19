# LightsOut - NGen Project 14091

**Fully Autonomous End-to-End Flexible Assembly System Enabled by AI & Robotics**

## Overview

LightsOut is an NGen-funded advanced manufacturing project (#14091) to build a fully autonomous, flexible end-to-end assembly line for personal care contract manufacturing. The system eliminates manual changeover and PLC programming requirements by leveraging AI-driven recipe creation, advanced computer vision, collaborative robotics, and novel mechanical engineering.

The project is led by Petra Hygienic Systems (PLX), a Canadian contract manufacturer founded in 1993, in partnership with Sidac Systems (robotics/mechanical integration) and Analytika/Mastrin (AI/ML recipe creation).

## The Problem

Mid-market contract manufacturers face two critical bottlenecks:

1. **Mechanical inflexibility** -- Equipment cannot handle diverse packaging formats without extensive manual changeover, resulting in significant downtime between production runs
2. **PLC programming dependency** -- Every new product requires manual recipe creation by expensive vendor programmers, preventing manufacturers from taking on new projects efficiently

These bottlenecks are particularly acute for contract manufacturers running production runs under 100,000 pieces, where changeover costs and downtime erode margins.

## The Solution

LightsOut is a Digital Twin platform consisting of:

- **Flexible Robotic Assembly** -- UR5e and UR10e COBOTs with universal EOAT for pump/cap insertion and case packing, handling packaging from 15ml to 1L without extensive changeover
- **AI-Powered Recipe Creation** -- Analytika's generative AI model uses computer vision to automatically create PLC recipes from incoming material inspections, eliminating manual programming
- **Vision Inspection System** -- Leverages the existing QC inspection workflow to index packaging parameters and feed AI/ML models for intelligent recipe generation
- **Digital Twin Control Tower** -- Real-time production optimization integrating robotics hardware, AI, and process control

### How It Works

```
Incoming Materials → QC Vision Inspection (indexes parts → feeds AI model)
                                    ↓
                     AI Recipe Engine → generates PLC instructions
                                    ↓
        Hopper → Feeder → COBOT 1 (picks pump/cap via vision guidance)
                                    ↓
              MPA (Mechanical Parts Accumulator — buffers parts)
                                    ↓
        COBOT 2 (picks from MPA → inserts pump/cap into bottle)
                                    ↓
         Filler → Capper → Vision QC → Case Packing → Palletizing
```

## Project KPIs

| # | KPI | Target |
|---|-----|--------|
| 1 | **Flexibility** | Handle all packaging from 15ml to 1L containers without extensive changeover |
| 2 | **Throughput** | 30-45 pieces per minute (sustained) |
| 3 | **Reduced Downtime** | 5 hours reduced changeover time per job |
| 4 | **Autonomous Operation** | Zero manual PLC programming for new products |

## Consortium Partners

| Partner | Role | Contribution |
|---------|------|-------------|
| **Petra Hygienic Systems (PLX)** | Project Lead | Production environment, line integration, project management, IP ownership |
| **Sidac Systems** | Mechanical & Robotics | COBOT integration, MPA, hopper/feeder, vision QC, EOAT, mechanical design |
| **Analytika (Mastrin)** | AI & Software | Generative AI PLC recipe creation, computer vision algorithms, Digital Twin |

## Project Budget

| Partner | Budget | Claimed to Date |
|---------|--------|----------------|
| Petra | $1,510,000 | $861,000 |
| Analytika (Mastrin) | $975,000 | $408,000 |
| Sidac | $601,000 | $91,000 |
| **Total** | **$3,088,286** | **$1,359,614** |

NGen reimburses 37% of eligible expenses.

## Current Status

**Project Phase:** Execution (Phase 3 of 5) | **Overall Completion:** ~54% | **Current Quarter:** Q7

The assembly line is built and operational at Petra. The primary challenge is the **pump/cap insertion system redesign** -- the current system generates excessive errors with newly introduced products. Research and solution analysis is complete (see [docs/](docs/)); implementation of the redesign is the next major milestone.

## Repository Structure

```
lightsout/
├── README.md                    # This file
├── docs/
│   ├── PROJECT_PLAN.md          # Work Breakdown Structure and timeline
│   ├── MILESTONES.md            # Milestone register with dates and status
│   ├── RISK_REGISTER.md         # Project risk matrix (Q7 current)
│   ├── IP_PLAN.md               # Background and Foreground IP strategy
│   ├── COMMERCIALIZATION.md     # Commercialization plan per partner
│   ├── PARTNERS.md              # Consortium partner profiles
│   └── BUDGET.md                # Financial tracking and NGen claims
└── agentic-swarm/               # Multi-agent AI system (submodule)
```

## NGen Quarterly Deliverables

Each quarter, the project submits to NGen:
- **Presentation** -- Progress against each task, KPI updates, partner updates, financials, IP, commercialization
- **Risk Register** -- Updated threat/opportunity tracking with mitigated scores
- **Project Plan** -- Comprehensive WBS with completion percentages
- **Milestone Register** -- Milestone status updates in Salesforce
- **Claim** -- Financial reimbursement submission for eligible expenses
- **IP Plan** -- Background/Foreground IP tracking and FTO assessments
- **Commercialization Plan** -- Market sizing, go-to-market activities, partner plans

## Key Documents (SharePoint)

Project documentation is maintained in SharePoint at:
`petrasoap.sharepoint.com/sites/VincePersonal/Shared Documents/NGen`

Organized into:
- `Context/` -- Initial application documents, quarterly review archives (Q1-Q6), reference materials
- `Last Meeting Documentation/` -- Most recent quarterly review (Q7) documents
- `R.Commander Analysis/` -- AI-generated research and solution analysis for pump insertion redesign
- `Claude Action Items/` -- Active prompts and task definitions
