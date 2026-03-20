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
- [Fraud Detection](#-fraud-detection-mechanisms)
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

### 1. Onboarding Flow (5 Minutes)

```mermaid
graph LR
    A[Phone Number<br/>(10 digits)] --> B[OTP Verification<br/>(6-digit SMS)];
    B --> C[Platform Select<br/>(Zomato/Swiggy)];
    C --> D[Work Zone Map<br/>(Select 3 zones)];
    D --> E[Weekly Hours<br/>(40-60 hours)];
    E --> F[AI Risk Score<br/>(Calculated)<br/>Score: 78/100];
    F --> G[Premium Quote<br/>₹89/week<br/>[Pay via UPI]];
graph TD
    subgraph Trigger Detection
        A[TRIGGER EVENT DETECTED<br/>Heavy rain (>10mm/hr) in Andheri West] --> B{AUTOMATIC CLAIM INITIATION};
    end
    
    subgraph Verification
        B --> C[GPS verification:<br/>User in affected zone?];
        B --> D[Time match:<br/>During scheduled work hours?];
        B --> E[Platform check:<br/>Was 'online' on Swiggy?];
        C & D & E --> F[Loss calculation:<br/>6 hours × ₹133/hour = ₹800];
    end

    subgraph Fraud & Payout
        F --> G[AI FRAUD DETECTION<br/>• GPS match<br/>• Time match<br/>• No duplicate<br/>• No suspicious pattern];
        G --> H[INSTANT PAYOUT<br/>• Notification: "Rain detected! ₹800 credited"<br/>• UPI transfer<br/>• Total time: 2-3 minutes];
    end
