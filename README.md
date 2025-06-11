# Final LLM Practical Assignemnet

##  Project Summary

This project analyzes employee messages to derive sentiment and engagement insights using Python and NLP techniques. It includes sentiment labeling (via TextBlob), exploratory data analysis (EDA), monthly scoring, employee ranking, flight-risk identification, and a linear regression model for predicting sentiment trends.

## Contents

- `GreenTreen_ProjectProblemStatement_SolutionGG.ipynb`: Main notebook with code and markdown annotations.
- `Practical_Assessment_GreeshmaReport.pdf`: Final report detailing approach, findings, and model evaluation.
- `labeled_dataset.csv`: Output file with sentiment-labeled messages.
- `test(in).csv`: Provided input dataset.
- `visualization/`: Contains saved visual plots used in analysis.
- `README.md`: Summary file (this one).

## Highlights

### Top 3 Positive Employees (Monthly, Sample):
- **don.baughman@enron.com**
- **johnny.palmer@enron.com**
- **lydia.delgado@enron.com**

### Top 3 Negative Employees (Monthly, Sample):
- **rhonda.denton@enron.com**
- **john.arnold@enron.com**
- **patti.thompson@enron.com**

### Flight Risk Employees:
These employees were flagged as flight risks based on the following condition:
They sent 4 or more negative messages within a rolling 30-day period.
Identified Employees:
- **bobette.riner@ipgdirect.com**
- **johnny.palmer@enron.com**
- **lydia.delgado@enron.com**
- **patti.thompson@enron.com**
- **rhonda.denton@enron.com**
- **sally.beck@enron.com**
- **john.arnold@enron.com**
## Key Visualizations (saved in `/visualization`):
- `sentiment_distribution.png`: Sentiment label counts.
- `message_length_by_sentiment.png`: Message lengths per sentiment.
- `top_active_employees.png`: Most active message senders.
- `top_positive_employees.png`: Top positive employees per month.
- `top_negative_employees.png`: Top negative employees per month.
- `actual_vs_predicted.png`: Model performance plot (linear regression).

## Modeling
A **linear regression model** was trained using:
- Message count
- Average message length
- Total word count

**Model Results:**
- **R² Score:** 0.148
- **RMSE:** 1.31

---

## Contact
Prepared by **Greeshma Gudapati** as part of the LLM Practical Assessment for GreenTreen.
