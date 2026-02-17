# DiningDossier: AI-Powered Restaurant Intelligence

**DiningDossier** is an automated marketing intelligence system designed to empower digital agencies with high-precision lead generation. By transforming raw geolocation data into comprehensive, sales-ready tactical reports in under 30 seconds, the tool eliminates the "Blind Sales Problem"—the common agency struggle of spending hours on manual research for generic, low-conversion pitches.

---

## The Problem: The "Blind Sales" Cycle

Marketing agencies often waste up to **4 hours of research** for every 1 hour of actual calling. Sales teams frequently "fly blind," cold-calling establishments without knowing their specific operational needs, digital gaps, or reputation risks. This manual labor leads to high opportunity costs and generic strategies that fail to convert.

## The Solution: An Automated Intelligence Pipeline

DiningDossier provides an end-to-end automated pipeline that scouts, analyzes, and reports on potential leads.

1. **Stage 1: The Scout (Apify Client)**
Deploys digital reconnaissance to scrape live Google Maps data, including reviews, ratings, contact info, and operational details.


2. **Stage 2: The Brain (Gemini 3 Flash)**
Utilizes advanced Large Language Models to analyze unstructured review text. It identifies Unique Selling Propositions (USPs), spots service shortcomings, and generates targeted sales strategies.


3. **Stage 3: The Reporter (FPDF)**
Synthesizes intelligence into a professional, one-page tactical dossier featuring color-coded sections and ready-to-use cold-call scripts.



---

## Technical Mechanics

The project is built with a robust pipeline featuring multiple safeguards to ensure data quality and system stability:

* **Schema Validation:** Uses Pydantic and `JsonOutputParser` to enforce strict output structures, preventing messy or hallucinated results.


* **Resilient Design:** Includes `try-except` blocks for graceful error handling and hard-coded `time.sleep` delays to manage API rate limits.


* **Text Sanitization:** Implements a custom `clean()` function to replace "smart quotes" and special characters, preventing PDF generation crashes.


* **Optimized Analysis:** Restricts review analysis to a 2,000-character window to optimize performance and control operational costs.


## Core Features

* **Multi-Market Support:** Dynamic search queries with country suffixes allow the tool to work across various geographies, such as Canada and Bangladesh.


* **Actionable Insights:** Automatically identifies "Warning Signals," such as service pacing issues or digital visibility gaps, and provides specific "Strategic Attack Plans".


* **Script-Ready Openers:** Generates high-impact "Golden Cold Call Openers" tailored to each lead's specific reputation and operational status.



## Future Roadmap

* **Horizontal Expansion:** Applying the model to new verticals like salons, clinics, and retail outlets.


* **Data Deepening:** Integrating "Social Listening" for Instagram/Facebook presence and Pixel detection for ad-readiness audits.


* **Architecture Scaling:** Implementing parallel crawls and batched AI processing to increase throughput.


**Developed by:** Shahad Islam Mugdho **Presented to:** Damil Alam Prakash & Mr. Avi Noel, Red Minstrel Marketing
