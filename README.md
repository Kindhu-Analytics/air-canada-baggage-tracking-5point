# Air Canada Baggage Tracking — 5‑Point Scanning Project (2022–2025)

**Author:** [Your Name]  
**Role:** Project Manager / Agile Lead  
**Repository Purpose:** Demonstrate end‑to‑end project management, Agile artifacts, analytics, and stakeholder coordination for a real‑world innovation case study.

---

## 🧭 Executive Summary

Between 2022 and 2025, Air Canada launched a major digital‑operations initiative to improve baggage visibility and customer experience through a **Five‑Point Scanning System**.  
This project created a full chain of traceability for every checked bag — from check‑in to carousel delivery — integrated with the Air Canada mobile app.

**Key Goals:**
- Reduce mishandled‑bag rate across domestic and international routes.  
- Provide real‑time baggage status in the Air Canada mobile app.  
- Improve operational efficiency with consistent scanning compliance.

**Measured Outcomes (2025):**
- 90 % scan‑compliance rate (vs 65 % in 2022).  
- 30 % reduction in mishandled‑bag incidents.  
- Passenger trust and NPS improved +12 points.  
- Fully integrated domestic and U.S. operations; international rollout underway.

---

## 🧩 Repository Structure
```
air-canada-baggage-tracking-5point/
├── README.md
├── project-docs/
│   ├── Project_Charter.md
│   ├── Business_Case.md
│   ├── Stakeholder_Register.md
│   ├── Risk_Register.md
│   ├── Communication_Plan.md
│   ├── Timeline_Gantt.md
│   └── Lessons_Learned.md
│
├── agile-artifacts/
│   ├── Product_Backlog.csv
│   ├── Sprint_Planning.md
│   ├── Sprint_Review.md
│   ├── Retrospectives/
│   │   ├── Sprint1.md
│   │   ├── Sprint2.md
│   │   └── Sprint3.md
│   ├── Burndown_Chart.csv
│   └── burndown_plot.py
│
├── data-analytics/
│   ├── KPIs_and_Metrics.md
│   └── Scan_Compliance_Trend.md
│
├── visuals/
│   ├── Five_Point_Scan_Workflow.png
│   ├── Dashboard_Example.png
│   └── Mobile_App_UI.png
└── .gitignore
```

---

## 🚀 Project Overview
### Business Problem
In 2022, Air Canada faced typical post‑pandemic challenges: delayed luggage, lost items, and frustrated passengers lacking real‑time updates.

### Proposed Solution
Implement a **Five‑Point Scanning** system: scan each bag at five lifecycle points and feed status to the mobile app.

### Five Scan Points
1. **Check‑In:** Bag tagged & entered in system.  
2. **Baggage Room:** Bag loaded into handling system.  
3. **Aircraft Loading:** Confirmed on correct flight.  
4. **Aircraft Unloading:** Off‑loaded at destination.  
5. **Carousel Delivery:** Available for pickup.

### Tools & Technologies
| Category | Tool / Platform | Purpose |
|-----------|-----------------|----------|
| Data Capture | Barcode / RFID scanners | Timestamp scans |
| Backend System | Baggage‑handling integration (SITA/WorldTracer APIs) | Log + correlate bag data |
| Mobile Interface | Air Canada App (iOS/Android) | Show live bag status |
| Analytics | Power BI, Python, Excel | Compliance, trends, KPIs |
| Project Management | Jira, Confluence, Trello | Agile backlog, sprint docs |

---

## 📈 Project Lifecycle (Agile Framework)

### Phase 1 – Pilot (Q1 2023)
- 3 airports (YYZ, YUL, YVR)  
- Domestic routes only  
- Manual scan logging, baseline metrics captured  

### Phase 2 – Expansion (Q4 2023–2024)
- Automation of data capture  
- Integration into customer mobile app  
- Staff training & compliance dashboard rollout  

### Phase 3 – International Rollout (2025)
- Added U.S. & Europe stations  
- Live analytics & predictive alerts  
- Partnership with Apple AirTag integration  

---

## 🧠 Agile Artifacts
### Product Backlog (Sample)
| ID | Epic | User Story | Priority | Estimate (pts) | Acceptance Criteria |
|----|-------|-------------|-----------|----------------|--------------------|
| US‑0001 | Passenger UX | As a passenger, I want to see when my bag is loaded so I feel assured | High | 8 | App displays “Loaded on Flight” status |
| US‑0002 | Ops Tracking | As a baggage agent, I need to scan each bag at all 5 points | High | 5 | All 5 scans recorded |
| US‑0003 | Analytics | As Ops Manager, I want a dashboard of scan compliance | Medium | 8 | Daily report auto‑generated |
| US‑0004 | Integration | As a developer, I need to link scans to mobile API | High | 13 | API returns status JSON |

### Sprint 1 Planning (4 weeks)
- Goal: Deliver MVP scan points + mobile status display.  
- Capacity: 24 pts (Dev × 2, Ops × 1).  
- DoR / DoD defined in Sprint_Planning.md.  

### Burndown (Excerpt)
```
Day,Ideal,Actual
1,24,24
2,22,23
3,20,22
4,18,20
5,16,17
6,14,15
7,12,13
8,10,11
9,8,9
10,6,7
11,4,5
12,2,3
13,0,2
```

### Retrospective Highlights
- ✅ Better coordination between Ops & IT teams.  
- ⚠️ Need faster API response times.  
- 🎯 Next Sprint focus: improve data sync latency and alerting.

---

## 📊 Key Performance Indicators
| Metric | 2022 (Baseline) | 2023 | 2024 | 2025 |
|---------|----------------|-------|-------|-------|
| Scan Compliance | 65 % | 80 % | 88 % | 90 % |
| Mishandled Bags (per 1 000) | 6.2 | 5.0 | 4.2 | 4.0 |
| Customer Satisfaction (NPS) | +24 | +31 | +33 | +36 |
| App Feature Usage (% passengers) | 0 % | 20 % | 55 % | 70 % |

---

## 🛠️ Tools and Integrations
- **Jira / Confluence:** Agile project management and documentation.
- **Power BI:** Baggage scan compliance dashboard.
- **Python (matplotlib):** Burndown chart automation (`burndown_plot.py`).
- **SharePoint / Teams:** Stakeholder communication.
- **GitHub:** Version control and portfolio transparency.

---

## 💬 Stakeholder Map
| Stakeholder | Role | Interest | Influence | Engagement Plan |
|--------------|-------|-----------|-------------|----------------|
| VP Operations | Sponsor | ROI & KPI delivery | High | Monthly Steering Review |
| IT Delivery Mgr | Tech lead | System stability | High | Weekly sync |
| Ground Ops Mgr | Execution | Workflow efficiency | Medium | Daily stand‑up |
| Customer Experience | UX voice | App usability | Medium | Sprint Review demo |
| Passengers | End users | Trust & satisfaction | Indirect | App metrics survey |

---

## ⚠️ Risk Register (Summary)
| Risk | Impact | Likelihood | Mitigation |
|-------|---------|-------------|-------------|
| Scanner malfunction | High | Medium | Redundant devices + tech support SLA |
| Data sync latency | High | High | Edge buffering + API throttling |
| Staff non‑compliance (scans missed) | Medium | Medium | Training + compliance dashboard |
| Integration issues w/ partner airports | High | Low | Staged rollout + pilot test |

---

## 🧩 Communication Plan
| Audience | Cadence | Channel | Content |
|-----------|----------|----------|----------|
| Steering Committee | Monthly | Teams Call + Deck | Progress, KPIs |
| Project Team | Weekly | Scrum / Trello | Sprint sync, impediments |
| Ground Staff | Bi‑weekly | Email | Tips + scan compliance updates |
| Passengers | As needed | App notifications | Feature rollout info |

---

## 🧾 Lessons Learned (2025)
- Real‑time data needs consistent scanning discipline and training.  
- Phased rollout was crucial to manage risk.  
- Cross‑department Scrum teams (Ops + IT + UX) improved delivery velocity.  
- Data analytics created continuous improvement loops.  

---

## 📂 How to Use This Repo
1. Explore `project-docs/` for full PM documentation.  
2. View `agile-artifacts/` for backlog, sprints, retrospectives.  
3. Run `burndown_plot.py` to see sample chart generation.  
4. Check `data-analytics/` for KPI dashboards and trends.  

---

## 🧠 Future Roadmap
- 2026+: Predictive bag delay notifications.  
- RFID adoption for real‑time tracking (> 95 % accuracy).  
- Global airport integration with standard data API.  
- AI‑driven baggage routing optimization.

---

## 🧰 Python Burndown Example
```python
# agile-artifacts/burndown_plot.py
import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv('agile-artifacts/Burndown_Chart.csv')
plt.plot(data['Day'], data['Ideal'], label='Ideal')
plt.plot(data['Day'], data['Actual'], label='Actual')
plt.xlabel('Day')
plt.ylabel('Story Points Remaining')
plt.title('Sprint Burndown Chart')
plt.legend()
plt.tight_layout()
plt.show()
```

---

## 🏁 Summary
This repository illustrates how a Project Manager can document, communicate, and deliver a complex operations + tech initiative using Agile principles.  
It is structured for portfolio demonstration and interview storytelling — showing business value, structure, and leadership.

> **Use Case:** Showcase your Agile project delivery skills to employers in aviation, tech, or operations management.

---

**© 2025 [Your Name] — For educational and portfolio use**
