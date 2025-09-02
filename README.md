# 🎮 Trends and Sentiment Mining for Gaming Applications

## 📖 Project Description
**Trends and Sentiment Mining for Gaming Applications** is an open-source project that analyzes user reviews from popular games like *Counter-Strike: Global Offensive*, *Dota 2*, and *Apex Legends*.  
The project uncovers **sentiment trends over time** to better understand player experiences and reactions to updates, events, and community shifts.

By combining **web scraping**, **natural language processing**, and **machine learning**, this tool provides actionable insights for both game developers and researchers interested in community feedback.

---

## ✨ Features
- 🔎 **Automated Web Scraping** with Selenium & BeautifulSoup  
- 🧹 **Data Preprocessing** (tokenization, stopword removal, normalization) using NLTK & pandas  
- 🤖 **Sentiment Analysis** via:
  - TextBlob (lexicon-based polarity scoring)
  - Hugging Face Transformers (context-aware classification)  
- 📊 **Visualization** with matplotlib to track sentiment trends over time  
- ⚡ Modular pipeline for easy extension to other games or datasets  

---

## ⚙️ Installation

### Prerequisites
- Python **3.7+**
- (Optional) ChromeDriver or other WebDriver if using Selenium
- NLTK corpora (stopwords, punkt, etc.)

### Setup
Clone the repository and install dependencies:
```bash
git clone https://github.com/yourusername/Trends-and-Sentiment-Mining-for-Gaming-Applications.git
cd Trends-and-Sentiment-Mining-for-Gaming-Applications
pip install -r requirements.txt
````

---

## 🚀 Usage

1. **Scrape Reviews**

   ```bash
   python data_collection.py
   ```

2. **Preprocess Data**

   ```bash
   python preprocess.py
   ```

3. **Run Sentiment Analysis**

   ```bash
   python sentiment_analysis.py
   ```

4. **Visualize Trends**

   ```bash
   python trend_visualization.py
   ```

Output includes:

* Cleaned review datasets
* Sentiment-labeled reviews
* Time-series visualizations of sentiment per game

---

## 🧠 Methodology

1. **Data Collection**: Scraping reviews and metadata from Steam pages
2. **Preprocessing**: Cleaning text with regex, stopword removal, and lemmatization
3. **Sentiment Analysis**:

   * TextBlob for quick polarity scoring
   * Transformers (BERT-based models) for nuanced classification
4. **Trend Analysis**: Rolling averages and comparative plots to reveal sentiment shifts

---

## 📊 Sample Results

Here’s an example of a sentiment trend output for multiple games:

<p align="center">
  <img src="images/sentiment_trend.png" alt="Sentiment Trend Example" width="600">
  <br/>
  <em>Average sentiment polarity of CS:GO, Dota 2, and Apex Legends over time.</em>
</p>

👉 To embed your own result plots, save them in an `images/` folder and include them with:

```markdown
![Sentiment Trend](images/sentiment_trend.png)
```

---

## ⚠️ Challenges & Limitations

* Sarcasm and irony detection remains difficult
* Gaming slang may reduce accuracy of general sentiment models
* Large datasets can be slow to process without GPU acceleration
* Temporal gaps or review spikes (e.g., review bombing) can bias results
* Currently limited to English-language reviews

---

## 🔮 Future Work

* Train custom models fine-tuned on gaming reviews
* Real-time dashboard for ongoing sentiment monitoring
* Integrate data from Reddit, Twitter, and Discord
* Aspect-based sentiment (e.g., gameplay vs. graphics)
* Developer-facing feedback loops

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add new feature'`
4. Push and open a PR

---

## 📚 References

* Fadhlurrahman, J. A. M., et al. (2023). *Sentiment Analysis of Game Reviews on Steam using BERT, BiLSTM, and CRF.*
* Guzsvinecz, T., & Szűts, J. (2023). *Length and sentiment analysis of reviews about video games on the Steam platform.*
* Dilmegani, C., & Arslan, E. (2025). *Top 7 Sentiment Analysis Challenges.*
* Hugging Face Transformers Documentation
* V7 Labs Blog – *AI Sentiment Analysis: Definition, Examples & Tools*

---

## 📌 License

This project is licensed under the MIT License. See the LICENSE file for details.

