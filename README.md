# Beauty Insight Lab MVP: Integrated Dashboard
[![Next.js](https://img.shields.io/badge/Next.js-16.1-black)]() [![FastAPI](https://img.shields.io/badge/FastAPI-Python-009688)]() [![Vercel](https://img.shields.io/badge/Deployment-Vercel-triangle)]() [![GA4](https://img.shields.io/badge/Analytics-GA4-orange)]()

> [!IMPORTANT]
> This repository is a public introduction to the 'Beauty Insight Lab' project. The actual source code is currently private for commercial security reasons." (이 레포지토리는 프로젝트 소개용입니다. 실제 소스 코드는 상용 보안을 위해 비공개로 전환되었습니다

> **K-Beauty Export Tracker & AI Localization Agent**
> From Real-time Customs Data Analysis to FDA-Compliant Marketing Transcreation.

Welcome to the **Beauty Insight Lab MVP** monorepo. This repository houses the complete tech stack for the "K-Beauty Export Tracker" and "AI Localization Agent". [Live Link](https://www.beautyinsightlab.com/)

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="./Export Tracker.png" alt="K-Beauty Export Tracker" width="100%" />
        <br />
        <b>K-Beauty Export Tracker Live</b>
      </td>
      <td align="center">
        <img src="./localization view.png" alt="AI Localization Agent" width="100%" />
        <br />
        <b>AI Localization Agent Live</b>
      </td>
    </tr>
  </table>
</div>

---


## 🚀 Why This Project?

> **"Hyper-Growth vs. Hyper-Complexity"**
> K-Beauty is entering its 3rd structural shift. While the market is exploding (14.5% YoY), the barriers to entry—regulatory and cultural—are higher than ever.

Traditional translation fails to capture K-Beauty's nuance, and raw data fails to provide market context. This project bridges the gap between **Data** and **Action**.

- **The Problem: Cultural Mismatch**: 
    1. **"Dewy" vs "Greasy"**: What Koreans call "Mul-gwang" (Radiance) is often perceived as "Oily/Dirty" in the US without proper context.
    2. **Regulatory Minefield**: Direct translation of K-Beauty terms (e.g., "Whitening", "Medicinal") leads to FDA compliance violations and Amazon account bans.
- **The Solution: K-Beauty Trade OS**: 
    1. **Real-time Tracker**: Analyzing export weight/price trends to find the "Winning Sector".
    2. **Context-Aware Agent**: A "Safety-First" localization engine that filters risks and *transcreates* for the US market context.

---

## ✨ Key Features

### 1. 📊 Expert Item Analysis Engine (Export Tracker)
* **Deep HSK Mapping**: Implemented `Matrix Aggregation` (e.g., Mask Sheets = 3304 + 3307) for accurate category analysis.
* **Unit Price Analytics**: Real-time calculation of `$ / kg` to track premiumization trends.
* **AI Market Prediction**: Google Gemini 2.5 generates context-aware market reports based on raw data.

### 2. 🇺🇸 Context-Aware Localization Agent (AI Tool)
* **Safety First (FDA Compliance)**: Detects high-risk keywords and provides **Educational Cards** explaining *why* they are banned (e.g., "Whitening" → "Brightening").
* **Transcreation Logic**: Aligns with 2026 US trends ("Clean Clinical", "Verification"). mapping "Mugwort" (Mass) vs "Artemisia" (Premium) based on brand positioning.
* **Deep Mapping**: Maps K-Slang (e.g., "인생템") to US Gen-Z vernacular (e.g., "Holy Grail").

### 3. 🔄 VoC Data Flywheel
* **Customer Feedback Loop**: We don't just infer; we learn. Every Friday, the model is updated with real "Voice of Customer" data (e.g., negative reviews on "Scent").
* **Physical Logic**: Solves product misunderstandings (e.g., translating "Melts Sebum" instead of "Oil" to prevent "Breakout" fears).

---

## 📂 Project Structure

This monorepo is organized into the following workspaces:

- **`frontend/`**: 
  - **Stack**: Next.js 16 (App Router), Tailwind CSS, TypeScript.
  - **Role**: The main dashboard interface and Localization Tool UI.
  - **Key Features**: HSK Category Analysis, AI Localization Page, Non-China Index Visualization.

- **`backend/`**:
  - **Stack**: Python (FastAPI), Poetry.
  - **Role**: AI Agent responsible for "Translation-Agent" logic and strategic verification.
  - **Deployment**: Render (Web Service) / Fly.io.

---

## 🏗️ Architecture & Technical Challenges
### Monorepo & Service Pattern
- **Unified Context**: Centralized management of K-Beauty Data Platform and AI Modules in a single repo.
- **Service Pattern**: To overcome Vercel's serverless limitations (no loopback calls), we refactored the API calls using a Service Pattern, ensuring direct function execution without network overhead.

### Structured Output & Logging
- **Pydantic Schema**: Enforces structured JSON output (Strategy Points, Summary) from the LLM for "Explainable AI".
- **Structured Logging**: Replaced print statements with JSON-formatted logs for ELK/CloudWatch integration.

---

## 📅 Development Journey (Jan 2026)

| Date | Milestone | Description |
|:---:|:---|:---|
| **Jan 23** | **Private Beta Transition** | • **MIT Final Release**: Archived public MVP version (`mit-final-version`).<br>• **Showcase Launch**: Opened public gateway for project introduction.<br>• **Commercial Security**: Transitioned core monorepo to Private for IP protection. |
| **Jan 21** | **Context Engineering & Blog** | • **Project Rules**: Established `project_rules.md` for context-aware AI coding.<br>• **Blog Revamp**: Redesigned Tech Blog with Sticky TOC & Hybrid Layout.<br>• **UX Enhancement**: Added Reading Progress bar and "Executive Summary" blocks. |
| **Jan 16** | **Strategic Scale-Up** | • **Forecast Engine Refinement**: Upgraded to 'High-Tech' mode with structural shift detection (Prophet) & correlated mock data logic.<br>• **Investor Pitch Deck**: Launched `/pitch` endpoint with interactive React slides for IR meetings.<br>• **UI/UX Polish**: Implemented 'Coming Soon' overlay with Framer Motion animations. |
| **Jan 15** | **AI Forecasting Core** | • **Prophet Integration**: Deployed `/api/v1/predict` with seasonality & macro-regressors.<br>• **Multi-Source Loader**: Unified Customs Data (36mo), FRED (Exchange Rate), and Google Trends.<br>• **Trend Radar**: Visualized real-time user interest patterns. |
| **Jan 14** | **Interactive Pitch Deck** | • **Web-based Deck**: Built a responsive slide deck using Next.js 16 & Embla Carousel.<br>• **Mobile Context**: Implemented "Landing Page" scroll mode for mobile investors.<br>• **Data Storytelling**: Visualized traction data using animated Recharts. |
| **Jan 12** | **SEO & Analytics Upgrade** | • Implemented **Triple-Track SEO** (Dataset, App, Blog) for targeted exposure.<br>• Enhanced **GA4 Event Tracking** for granular user behavior analysis.<br>• Fixed **Markdown Rendering** readability issues. |
| **Jan 10** | **Knowledge Archive** | • **Tech Blog System**: Built a file-based CMS using Next.js MDX Remote.<br>• **Developer Experience**: Solved "Soft Break" issues for seamless Markdown writing. |
| **Jan 09** | **Real-world Data Refinement** | • Collected **Amazon Anua Bestseller** (Serum/Cleanser) 1-star reviews to identify pain points.<br>• Updated **Agent Mapping Tables** based on real negative feedback (e.g., texture, scent issues). |
| **Jan 08** | **Pilot Launch & Feedback** | • Distributed to developer communities (**GeekNews**, LinkedIn).<br>• Collected pilot user feedback and enabled **GA4 Custom Events** to track usage patterns. |
| **Jan 07** | **Integrated E2E Testing** | • Conducted Load Testing on the full pipeline: **Frontend ↔ Backend ↔ OpenAI**.<br>• Verified system stability under concurrent requests. |
| **Jan 06** | **Context-Aware Refactoring** | • Implemented dynamic prompt injection based on HSK Categories.<br>• Applied "Verification" strategy for US Market fit. |
| **Jan 04** | **Stability Engineering** | • Solved Vercel deployment issues ($0 data bug) via Service Pattern refactoring. |
| **Jan 03** | **Professional Edition** | • **Expert Item Engine**: Implemented dynamic HSK mapping (e.g., Mask Sheets = 3307+3304).<br>• **Unit Price Analytics**: Added real-time `$/kg` calculation to track premiumization.<br>• **Context Injection**: Enhanced AI prompts with item-specific regulatory context. |
| **Jan 02** | **Data Pipeline Stability** | • **Real-time Connection**: Stabilized Korea Customs API by solving parameter & encoding issues.<br>• **Algorithm Fix**: Corrected timezone-related date calculation errors. |

> 📘 **Explore More**:
> - **Development Logs**: [Beauty Insight Lab Blog](https://www.beautyinsightlab.com/blog)
> - **Vision & Agenda**: [Project Slides](https://www.beautyinsightlab.com/slides)
---

© 2026 Beauty Insight Lab Inc. (DeDeveloped by 박용락)
