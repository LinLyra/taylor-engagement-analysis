# Taylor Swift Engagement Analysis 🎤💍  

This project analyzes **YouTube comments** related to Taylor Swift’s engagement news.  
We apply the **Elaboration Likelihood Model (ELM)** and **sentiment analysis** to study persuasion routes, attention dynamics, and economic-like behavior in online discussions.  


## 1. Motivation  
Taylor Swift’s engagement triggered massive online discussions across platforms.  
We aim to answer:  
- Which persuasion route dominates? (**central/logical** vs **peripheral/emotional**)  
- Is sentiment mainly **positive or negative**, and how does it evolve?  
- Do online opinion dynamics resemble **economic models** (e.g., herding, polarization, overreaction)?  


## 2. Data Collection  
- **Source**: YouTube Data API v3  
- **Query**: engagement-related keywords (e.g., *“Taylor Swift engagement Travis Kelce”*)  
- **Selection**: top 5 most viewed videos (≥500k views)  
- **Records**: ~5,700 comments (including replies)  
- **Preprocessing**:  
  - Removed duplicates and spam  
  - Normalized emojis, punctuation, and irrelevant symbols  
  - Filtered irrelevant threads  


## 3. Methods  
- **Classification**  
  - Central vs Peripheral persuasion routes (ELM framework)  
  - Sentiment polarity (Positive / Neutral / Negative)  
- **Statistical modeling**  
  - Bayesian updating of sentiment probability  
  - Rolling variance (polarization)  
  - Herding dynamics: early vs late convergence  
- **Validation**  
  - Human-audited 100 comments  
  - Inter-rater reliability:  
    - Sentiment: 99% accuracy (Kappa=0.98)  
    - ELM path: 88% accuracy (Kappa=0.66)  


## 4. Key Findings  
- **Peripheral route dominates (~80%)**, showing emotional rather than logical responses.  
- **Negative sentiment outweighs positive**, though both are significant.  
- **Herding effect**: early positivity declines as late comments converge to negativity.  
- **Polarization**: high variance initially → steady decline → shared negative consensus.  
- **Attention dynamics**: sharp spike after the news, then decay.  
- **Engagement**: positive/central comments receive **higher average likes** despite being fewer.  


## 5. Technical Stack  
- **Python**: `pandas`, `scikit-learn`, `matplotlib`, `numpy`  
- **API**: YouTube Data API v3  
- **NLP**: Regex preprocessing, Gemini API for assisted classification  
- **Statistics**: Bayesian updating, rolling variance, Cohen’s Kappa  


## 6. Results Preview  
- **ELM path**: Peripheral (~80%) vs Central (~20%)  
- **Sentiment distribution**: Negative > Positive > Neutral  
- **Validation accuracy**:  
  - Sentiment = 99% (Kappa=0.98)  
  - ELM path = 88% (Kappa=0.66)  

📊 Example plots included in the notebook:  
- Sentiment distribution  
- Bayesian updating curve  
- Herding dynamics  
- Attention spikes  


## 7. Research Value  
- Shows how **communication theory (ELM)** and **economic models** can be applied to social media data.  
- Provides insights into **herding and overreaction** in digital attention markets.  
- Framework is generalizable to other online events (e.g., elections, product launches, crises).  



## Author  
**Long Lin** – Independent Researcher  
