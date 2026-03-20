# GigGuard AI
### AI-Powered Parametric Income Protection for India's Food Delivery Partners

**DEVTrails 2026 - Phase 1 Submission**  
*Seed Scale Soar University Hackathon*

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](YOUR_REPO_URL)
[![Live App](https://img.shields.io/badge/Streamlit-Live_App-brightgreen?logo=streamlit)](YOUR_STREAMLIT_URL)
[![Demo Video](https://img.shields.io/badge/YouTube-Demo_Video-red?logo=youtube)](YOUR_VIDEO_URL)

---

## 📖 Table of Contents
- [Problem Statement](#-problem-statement)
- [Our Solution: GigGuard AI](#-our-solution-gigguard-ai)
- [Persona & User Stories](#-persona--user-stories)
- [Core Workflow](#️-core-workflow)
- [Parametric Triggers](#-parametric-triggers)
- [Weekly Premium Model](#-weekly-premium-model)
- [AI/ML Integration Plan](#-ai-ml-integration-plan)
- [Fraud Detection Mechanisms](#-fraud-detection-mechanisms)
- [Tech Stack & Platform Choice](#-tech-stack--platform-choice)
- [Project Structure](#-project-structure)
- [Phase 1 Deliverables](#-phase-1-deliverables)
- [Business Model Viability](#-business-model-viability)
- [Critical Constraints Compliance](#-critical-constraints-compliance)
- [Future Roadmap](#-future-roadmap)
- [Team & Acknowledgments](#-team--acknowledgments)

---

## 🎯 Problem Statement

India's platform-based food delivery partners (Zomato, Swiggy) are the backbone of our fast-paced digital economy. However, external disruptions such as **extreme weather, pollution, and natural disasters** can reduce their working hours and cause them to lose **20–30% of their monthly earnings**.

**Current Reality:**
- **Average weekly earnings:** ₹8,000 - ₹15,000
- **Monthly income loss due to disruptions:** ₹6,400 - ₹18,000
- **Zero safety net:** They bear 100% of this loss with no income protection

> *"Last month, heavy rains in Mumbai stopped my deliveries for 6 hours. I lost ₹800 that day—my daughter's school fee installment. There was no compensation, no fallback."*  
> — **Raju, 28, Swiggy Delivery Partner, Andheri West**

## 💡 Our Solution: GigGuard AI

An **AI-enabled parametric insurance platform** that safeguards food delivery partners against income loss caused by external disruptions.

### What Makes It Different:

| Traditional Insurance | GigGuard AI (Parametric) |
| :-------------------- | :------------------------ |
| Claim after damage | **Automatic payout on trigger** |
| Submit documents, wait weeks | **Zero paperwork, instant credit** |
| Prove income loss | **Objective weather data = automatic verification** |
| Monthly/annual premiums | **Weekly pricing** matching gig payout cycles |

## 👤 Persona & User Stories

### Target User Profile
- **Age:** 22-35 years
- **Location:** Tier-1 cities (Mumbai, Delhi, Bangalore, Hyderabad, Pune)
- **Work Pattern:** 40-60 hours/week, week-to-week income dependency
- **Primary Pain Points:**
  - Monsoon rains stopping deliveries (4-6 hours lost)
  - Extreme heat (>45°C) forcing work breaks
  - Local curfews/strikes blocking access to delivery zones
  - App crashes during peak hours

### User Stories

| Story | Scenario | Loss | GigGuard AI Solution |
| :---- | :------- | :--- | :-------------------- |
| **Raju the Rain Warrior** | Mumbai monsoon, July 2024. Heavy rainfall in Andheri West (>15mm/hour). Raju couldn't work for 6 hours due to flooding. | **₹800** | Automatic detection → ₹800 instant payout |
| **Priya the Heat Survivor** | Delhi NCR, June 2024. Temperature hits 47°C. Zepto suspends outdoor deliveries for 3 hours due to heatwave advisory. | **₹450** | Temperature trigger fires → ₹450 credited to UPI |
| **Amit the Curfew Casualty** | Bangalore, August 2024. Sudden local curfew declared. All food deliveries suspended for 8 hours. | **₹1,000** | News API detection → Automatic payout |

## ⚙️ Core Workflow


## 📋 Parametric Triggers

| Trigger Type | Data Source | Threshold | Payout Rate | Max/Day |
| :----------- | :---------- | :-------- | :---------- | :------ |
| **Heavy Rain** | OpenWeatherMap API | >10mm/hour rainfall | ₹100/hour | ₹800 |
| **Extreme Heat** | IMD/Weather API | >45°C for 2+ hours | ₹100/hour | ₹600 |
| **Flooding** | Municipal alerts + Social signals | Official waterlogging alert | ₹120/hour | ₹1,000 |
| **Thunderstorms** | Weather API | Lightning + wind >50km/h | ₹100/hour | ₹800 |
| **App Crash** | Platform status API | >30 minutes downtime | ₹80/hour | ₹400 |
| **Curfew/Strike** | NewsAPI + Manual input | Official announcement | ₹100/hour | ₹800 |

**Important Note:** We insure **INCOME LOST** during these events, not the cost of fixing external issues (no vehicle repair, no health bills).

## 💰 Weekly Premium Model

### Premium Calculation Example (Raju, Mumbai)

| Component | Calculation | Example |
| :-------- | :---------- | :------ |
| **Base Premium** | ₹49 (Tier-1 cities) | ₹49 |
| **Zone Risk** | +₹20 per high-risk zone (Mumbai monsoon) | +₹20 |
| **Platform Discount** | -₹10 (verified partner) | -₹10 |
| **Weekly Hours** | +₹10 if >45 hours | +₹10 |
| **Loyalty Discount** | -₹5 after 4 weeks | ₹0 (new user) |
| **FINAL PREMIUM** | | **₹89/week** |

### Coverage Structure
- **Coverage Cap:** ₹2,000/week maximum payout
- **Payout Rate:** ₹100/hour of verified disruption
- **Payment Cycle:** Weekly (aligns with gig platform payouts)

## 🤖 AI/ML Integration Plan

### Phase 1 (Current): Rule-Based Foundation

| Feature | Implementation | Status |
| :------ | :------------- | :----- |
| **Risk Scoring** | Weighted algorithm: City (20%) + Zone history (30%) + Season (25%) + Hours (15%) + Platform (10%) | ✅ Implemented |
| **Premium Calculation** | Formula-based with 5-6 variables | ✅ Implemented |
| **Fraud Detection** | Basic rules: GPS match, time validation, duplicate prevention | ✅ Implemented |
| **Trigger Detection** | Weather API thresholds, manual curfew input | ✅ Implemented |

### Phase 2-3: ML Enhancement Roadmap

| Feature | Enhancement | Technology |
| :------ | :---------- | :--------- |
| **Dynamic Pricing** | ML model adjusts premiums based on claims history | Scikit-learn Random Forest |
| **Predictive Risk** | Forecast next week's disruption probability | Time-series forecasting (Prophet) |
| **Behavioral Fraud** | Anomaly detection on claim patterns | Isolation Forest |
| **Hyper-Local Weather** | Street-level prediction using multiple sources | Ensemble models |

## 🛡️ Fraud Detection Mechanisms

### Phase 1: Rule-Based Validation

| Check | Method | Action if Failed |
| :---- | :----- | :--------------- |
| **GPS Verification** | Claimed location must match disruption zone | Reject claim |
| **Time Validation** | Claim time must overlap with disruption period | Reject claim |
| **Duplicate Prevention** | Max 1 claim per day, 3 per week | Reject duplicate |
| **Platform Activity** | User must show "online" status during claimed hours | Flag for review |
| **Velocity Check** | Max 3 claims per week per user | Hold for manual review |

### Trust Score System
- **New Users:** Lower coverage limits (₹500/day max) for first 4 weeks
- **Verified Users:** Higher limits (₹2,000/day) after consistent usage
- **Suspicious Activity:** Temporary hold, admin manual review

## 🖥️ Tech Stack & Platform Choice

### Platform Choice: Web Application (Streamlit)
- **Why Web:** Food delivery partners primarily use mid-range Android phones with limited storage. Web apps require no installation, work across all devices, and allow instant updates.
- **Why Streamlit:** Rapid prototyping, Python-native ML integration, free cloud deployment, mobile-responsive design.

### Technology Stack

| Layer | Technology | Purpose |
| :---- | :--------- | :------ |
| **Frontend** | Streamlit, Folium, Plotly | Web UI, interactive maps, analytics charts |
| **Backend** | Python 3.9+, SQLite, APScheduler | Core logic, lightweight DB, background monitoring |
| **APIs (Mock/Sandbox)** | OpenWeatherMap, OpenStreetMap, Razorpay Test Mode, Mock SMS & Platform APIs | Weather, geolocation, payments, notifications |
| **Deployment** | Streamlit Cloud, GitHub | Free hosting, version control |


## 🚀 Phase 1 Deliverables

### 1. The Idea Document (This README)
- ✅ Persona-based scenarios (3 user stories)
- ✅ Weekly premium model explanation
- ✅ Parametric triggers defined
- ✅ AI/ML integration plan
- ✅ Tech stack and architecture
- ✅ Web vs Mobile justification

### 2. GitHub Repository
- [ ] Clean code structure
- [ ] Functional Streamlit prototype
- [ ] Mock data for demonstration
- [ ] `requirements.txt` with dependencies

### 3. 2-Minute Video
**Script Outline:**
- **0:00-0:20:** Introduce Raju, Mumbai Swiggy partner, lost ₹800 in rain
- **0:20-0:50:** Onboarding demo - zone selection, risk score, premium quote
- **0:50-1:20:** Simulate rain trigger → automatic notification → payout
- **1:20-2:00:** Dashboard showing protected earnings, next week's weather risk

## 📊 Business Model Viability

### Unit Economics (Per 1000 Active Users)

| Metric | Calculation | Amount |
| :----- | :---------- | :----- |
| Weekly Premium Revenue | 1000 users × ₹75 avg | ₹75,000 |
| Monthly Revenue | × 4.3 weeks | ₹3,22,500 |
| Expected Claims (30% users) | 300 claims × ₹600 avg | ₹1,80,000 |
| **Gross Margin** | | **44%** |
| Operating Costs | Tech, support, marketing | ₹72,500 |
| **Net Profit Margin** | | **22%** |

### Weekly Pricing Justification
Gig workers operate week-to-week with no salary security. Monthly premiums create cash flow mismatch—they might not have ₹300 at month start, but can afford ₹75/week after earning. Weekly pricing aligns with their income cycle and platform payout schedules (Swiggy/Zomato pay weekly).

## ⚠️ Critical Constraints Compliance

| Constraint | Our Approach |
| :--------- | :----------- |
| **Income Loss Only** | ✅ We cover lost wages during disruptions, not vehicle repair or health costs |
| **Weekly Pricing** | ✅ Strictly weekly premiums (₹49-₹149/week) matching gig payout cycles |
| **Food Delivery Focus** | ✅ Specific to Zomato/Swiggy partners, not generic gig workers |
| **External Disruptions Only** | ✅ Weather, curfews, app crashes—not personal health/accidents |
| **AI Integration** | ✅ Risk scoring, fraud detection, predictive modeling planned |

## 🔮 Future Roadmap

### Phase 2: Automation & Intelligence
- [ ] Real-time weather API integration
- [ ] Automated claim generation and processing
- [ ] SMS notification system (Twilio)
- [ ] Basic ML risk scoring
- [ ] Admin dashboard for manual reviews

### Phase 3: Scale & Optimization
- [ ] Advanced fraud detection (GPS spoofing detection)
- [ ] Predictive analytics dashboard
- [ ] Instant payout system (Razorpay live)
- [ ] Mobile app (Flutter/React Native)
- [ ] Multi-language support (Hindi, Marathi, Tamil)

## 👥 Team & Acknowledgments

### Team
*Santhosh Kumar B
*
*Tamilselvan
*
*Mohan M
*
*Prajeeth H
*

### Acknowledgments
DEVTrails 2026 Hackathon - Guidewire  
Mentors and organizers for this opportunity to build for India's gig economy

---

**🔗 Links:**
- GitHub Repository: [https://github.com/Santhosh-Kumar-ctrl/Devtrails_2026/tree/main]
- Demo Video: [YOUR_VIDEO_LINK]

*Built with ❤️ for India's delivery partners who keep our cities running, rain or shine.*
