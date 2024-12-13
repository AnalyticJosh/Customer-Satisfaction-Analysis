# Customer Satisfaction Analysis

## **Overview**
This project focuses on analyzing customer satisfaction data to uncover insights into customer behavior, preferences, and areas of improvement. Using Python and its powerful data analysis libraries, the project performs sentiment analysis, trend identification, and key metric calculations to assist businesses in enhancing customer experiences.

## **Objectives**
- Measure and analyze customer satisfaction levels.
- Perform sentiment analysis on customer feedback.
- Identify key drivers of satisfaction and dissatisfaction.
- Provide actionable insights to improve customer experience.

## **Key Features**
- **Data Cleaning**: Preprocessing raw customer data to handle missing values, outliers, and inconsistencies.
- **Sentiment Analysis**: Classifying feedback as positive, neutral, or negative using text analytics.
- **Visualization**: Creating charts and graphs to visualize trends in customer satisfaction.
- **Metric Calculation**: Calculating Net Promoter Score (NPS) and other satisfaction indicators.

## **Technologies Used**
- **Python**: Primary programming language for analysis.
- **Libraries**:
  - `Pandas` and `NumPy`: Data manipulation and analysis.
  - `Matplotlib` and `Seaborn`: Data visualization.
  - `NLTK` or `TextBlob`: Sentiment analysis.
  - `Jupyter Notebook`: Interactive environment for coding and visualization.

## **Dataset Information**
- The dataset includes:
  - Customer feedback text.
  - Satisfaction scores (e.g., scale of 1–10).
  - Timestamps of feedback.
- Describe any notable features or issues in the dataset (e.g., imbalances, missing values).

## **Steps to Reproduce**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AnalyticJosh/Customer-Satisfaction-Analysis.git
   cd Customer-Satisfaction-Analysis
   ```

2. **Set Up the Environment**:
   - Ensure you have Python installed (3.7 or higher).
   - Install required libraries:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Notebook**:
   - Open `Customer Satisfaction Analysis.ipynb` in Jupyter Notebook.
   - Execute cells sequentially to load the dataset, process the data, and generate insights.

## **Sample Analysis**
### Sentiment Analysis
```python
from textblob import TextBlob

def analyze_sentiment(text):
    analysis = TextBlob(text)
    if analysis.sentiment.polarity > 0:
        return 'Positive'
    elif analysis.sentiment.polarity == 0:
        return 'Neutral'
    else:
        return 'Negative'

data['Sentiment'] = data['Feedback'].apply(analyze_sentiment)
```

### Net Promoter Score Calculation
```python
nps = (len(promoters) - len(detractors)) / len(responses) * 100
```

## **Results and Insights**
- Sentiment analysis revealed:
  - 60% positive feedback.
  - 25% neutral feedback.
  - 15% negative feedback.
- NPS indicated strong customer loyalty with a score of 45.

## **Visualizations**
- Include example charts:
  - Sentiment distribution.
  - NPS trends over time.
  - Word clouds for common terms in feedback.

## **Contributions**
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## **License**
This project is licensed under the MIT License.

---

For further inquiries or feedback, please contact [Joshua Amusan](mailto:joshuaanalyst2@gmail.com).

