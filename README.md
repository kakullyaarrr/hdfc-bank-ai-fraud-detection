# hdfc-bank-ai-fraud-detection
📌 Problem Statement

Rule-based fraud systems cannot keep pace with the growth of digital payment fraud in India. They miss new fraud patterns and block too many genuine transactions — a real cost to a bank serving 100+ million customers. This project examines how AI/ML classification and anomaly-detection techniques can be applied to score transactions for fraud risk in real time, and what that means for HDFC Bank's business, customers, and regulatory obligations.

🏦 Solution Summary

A hybrid approach — supervised binary classification (logistic regression, Random Forest / XGBoost) trained on labelled historic fraud data, paired with unsupervised anomaly detection (Isolation Forest / autoencoders) to catch novel fraud patterns that have no prior label. Each transaction is scored in real time; low-risk transactions pass, medium-risk triggers step-up verification, high-risk is held for human review.

🛠️ Tools Used
Tool	Purpose
Claude	Research, fact-checking against primary sources, case study structuring, deck generation
🔑 Key Prompts
"HDFC Bank AI fraud detection machine learning"
"RBI annual report bank frauds amount FY2025 digital payment fraud India statistics"
"HDFC Bank number of customers branches FY2026 annual results total deposits"

Full prompt log, the basic → improved prompt comparison, and the AI-output critical evaluation are documented in PROMPT_PORTFOLIO.md.

📊 Key Findings
Fraud reported by Indian banks rose from ₹13,930 cr (FY24) to ₹36,014 cr (FY25) to ₹48,021 cr (FY26) — RBI Annual Reports.
Fraud in transaction data is typically well under 1% of volume, making accuracy a misleading metric; precision and recall matter far more.
HDFC Bank's own regulatory filings confirm technology investment in risk management but do not disclose specific fraud-model performance figures — a gap that shaped how the case study's claims were framed.
✅ Recommendations
Run a hybrid model, not a single algorithm
Optimise decision thresholds for business cost, not raw accuracy
Build explainability in from the start (e.g. SHAP)
Audit false-positive rates for fairness every quarter
Keep human investigators in the loop for high-value decisions
Close the feedback loop — retrain on every confirmed fraud and dispute
🎓 Learnings
A prompt naming a specific, authoritative source produces citable evidence; a general topic prompt produces confident-sounding but unverifiable claims.
Secondary sources can describe a real company's AI use in specific technical language without that language coming from the company itself — always check the primary filing.
The most defensible move when data doesn't exist in a primary source is to say so, not to fill the gap with a plausible-sounding number.
📁 Repository Contents
File	Description
HDFC_Fraud_Detection_MERGED.pptx	Final 12-slide submission deck — Part A + Part B combined
HDFC_Fraud_Detection_PartA.pptx	Standalone Part A business case study deck
PROMPT_PORTFOLIO.md	Part B — full prompt log, prompt improvement, tool usage, verification, critical evaluation
README.md	This file
📚 References

See the References slide in the deck and the source list in PROMPT_PORTFOLIO.md. Primary sources used: HDFC Bank's Form 20-F (FY2026, U.S. SEC), HDFC Bank Q4 FY26 earnings presentation, RBI Annual Reports (FY24–FY26).

All figures were verified against primary sources rather than secondary summaries. AI tools assisted the research process; analysis, structuring, and conclusions reflect the student's own understanding of the material.
