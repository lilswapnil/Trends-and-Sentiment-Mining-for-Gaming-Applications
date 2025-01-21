# Mining Sentiments & Analyzing Trends in Gaming Applications

## Project Description
This project focuses on sentiment analysis and trend visualization of user reviews from popular gaming platforms like Steam. By examining reviews for games such as *Counter-Strike: Global Offensive*, *Dota 2*, *Apex Legends*, and others, it provides valuable insights into community opinions and emerging trends. The system leverages tools like **TextBlob** for detecting sentiment polarity, **Transformers** for deep learning-based sentiment analysis, and various data visualization techniques to track how user feedback evolves over time.

---

## Installation

### Prerequisites
Ensure the following requirements are met before proceeding:

- **Python 3.7 or higher**
- Required Python libraries:
  - `beautifulsoup4` for web scraping
  - `pandas` for data manipulation
  - `nltk` for natural language preprocessing
  - `textblob` for sentiment analysis
  - `transformers` for advanced NLP analysis
  - `matplotlib` and `seaborn` for visualizations

### Installation Command
Install the required libraries using the following command:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Follow these steps to execute the project:

### 1. Data Collection

Scrape user review data from gaming platforms using BeautifulSoup. Run the script with:

```bash
python data_collection.py
```

The collected data will be saved as a CSV file named `reviews_data.csv`.

### 2. Preprocessing

Clean and preprocess the collected data by executing the preprocessing script:

```bash
python preprocess.py
```

This generates a cleaned dataset that is ready for sentiment analysis.

### 3. Sentiment Analysis

Perform sentiment classification by running:

```bash
python sentiment_analysis.py
```

#### Models Used:
- **TextBlob**: For basic sentiment analysis.
- **HuggingFace Transformers**: For nuanced and deep sentiment analysis.

### 4. Visualization

Visualize sentiment trends and shifts using:

```bash
python trend_visualization.py
```

The script generates outputs such as:
- Rolling average graphs for sentiment trends.
- Annotated plots showcasing significant sentiment shifts.

---

## Key Features
- **Multi-Level Sentiment Analysis**: Combines rule-based and deep learning approaches for comprehensive results.
- **Trend Visualization**: Highlights how sentiment evolves over time with intuitive graphs.
- **Flexible and Scalable**: Easily adaptable to analyze reviews for other gaming titles.

---

## Acknowledgments
Special thanks to the open-source Python community and the creators of the tools used in this project, including BeautifulSoup, TextBlob, and HuggingFace Transformers.
