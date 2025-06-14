# Final LLM Practical Assignemnet

# Employee Sentiment Analysis – Final LLM Assessment

**Name:** Greeshma Gudapati  
**Date:** 06/14/2025  
**Submission:** AI-project-submission

---

## 🔍 Overview

This project explores employee sentiment using a dataset of internal email messages. The goal was to label message sentiment, analyze employee engagement patterns, and build a basic prediction model based on communication behavior.

I used Python with HuggingFace Transformers (RoBERTa), pandas, matplotlib, and scikit-learn to carry out all six tasks described below. Every step of the analysis pipeline is documented in the Jupyter Notebook and this repository.

---

##  Tasks and Key Deliverables

### **Task 1: Sentiment Labeling**
- Used a pre-trained `cardiffnlp/twitter-roberta-base-sentiment` model to classify each message.
- Labels: `Positive`, `Negative`, and `Neutral`.
- Output: `sentiment_label` column added to dataset.

### **Task 2: Exploratory Data Analysis**
- Performed analysis on message length, frequency, and sentiment distribution.
- Created bar charts, box plots, and histograms.
- Insights: Most messages were Neutral, and Negative messages tended to be longer.

### **Task 3: Monthly Sentiment Score Calculation**
- Scored messages: `+1` for Positive, `–1` for Negative, `0` for Neutral.
- Aggregated sentiment scores per employee per month.
- Output: `employee_monthly_scores.csv`.

### **Task 4: Employee Ranking**
- Ranked top 3 Positive and Negative employees monthly.
- Used grouped bar plots to visualize monthly top scorers.
- Output: Sentiment ranking plots saved to `/visualization`.

### **Task 5: Flight Risk Identification**
- Applied a **rolling 30-day window** to flag employees sending **4+ negative messages**.
- Result: 10 employees identified as potential flight risks.
- Output: `flight_risk_df` table and associated plots.

### **Task 6: Predictive Modeling**
- Built a **Linear Regression model** using features like:
  - Message count
  - Average message length
  - Total word count
- Evaluated using R² and RMSE.  
- Output: Model performance plot and interpretation.

---

##  Folder Structure
.
├── GreenTreen_ProjectProblemStatement_SolutionGG.ipynb
├── README.md
├── Final_Report_GreeshmaGudapati.docx (optional)
├── visualization/
│   ├── eda_boxplot_length_sentiment.png
│   ├── eda_message_length_histogram.png
│   ├── eda_sentiment_distribution.png
│   ├── final_flight_risk_employees_Fixed.png
│   ├── monthly_score_distribution.png
│   ├── roberta_sentiment_distribution.png
│   ├── task6_sentiment_regression_plot.png
│   ├── top_negative_employees_over_time.png
│   └── top_positive_employees_over_time.png


##  Notes

- All labeling, scoring, ranking, and modeling are reproducible from the notebook.
- The project strictly followed LLM Final Assessment guidelines and FAQs.
- Visualizations and interpretations are designed to be concise and explainable.

---

##  Contact

For any clarification related to this submission, feel free to reach me at:

**Email:** gudapatigreeshma@gmail.com  
