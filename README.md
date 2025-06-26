# AI News Summarizer Pro

**AI News Summarizer Pro** is an AI-powered web application built with Streamlit that delivers concise, personalized news summaries. Utilizing natural language processing (NLP) models and NewsAPI.org, it provides summarized news articles, sentiment analysis, and a personalized feed across topics such as Technology, Health, Business, Politics, Sports, and Entertainment. Developed by Soumin Mujumdar and Vidhi Binwal from Symbiosis Institute of Technology (SIT), Pune, this project demonstrates expertise in AI and web development.

## Key Features

- **Search and Summarize**: Enter a topic to retrieve the latest news with AI-generated summaries and headlines.
- **Popular Topics**: Access news from categories including Technology, Health, Business, Politics, Sports, and Entertainment.
- **Sentiment Analysis**: Analyze the emotional tone of articles using AI-powered sentiment scoring.
- **Personalized Feed**: View a curated "For You" section based on reading history and preferences.
- **User Interface**: Navigate a responsive, custom-styled interface for an intuitive user experience.

## Technology Stack

- **Frontend and Framework**: Streamlit
- **Backend Services**: NewsAPI.org
- **AI Models**: Transformers / Hugging Face (e.g., DistilBERT for summarization, VADER for sentiment analysis)
- **Styling**: Custom CSS for enhanced layout and interaction design
- **Dependencies**: Python, requests, python-dotenv, NLTK

## Project Structure

```
├── app.py                       # Main Streamlit application
├── config.py                    # Page configuration and CSS loader
├── styles.py                    # Custom CSS styles
├── components/
│   ├── sidebar.py              # Sidebar with user settings
│   ├── news_card.py            # Renders news cards
│   └── recommendations_page.py  # Personalized "For You" section
├── services/
│   ├── news_service.py         # Handles NewsAPI calls
│   ├── ai_service.py           # Manages NLP models for summarization and sentiment analysis
│   └── user_preferences.py     # Manages reading history and preferences
└── utils/
    └── ui_utils.py             # UI helper functions for messages and buttons
```

## Prerequisites

- Python 3.8 or higher
- A valid NewsAPI key from [NewsAPI](https://newsapi.org/)
- pip for installing dependencies
- (Optional) A virtual environment for dependency management

## Installation and Setup

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/ai-news-summarizer.git
   cd ai-news-summarizer
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure the NewsAPI key**  
   - Obtain a key from [NewsAPI](https://newsapi.org/).
   - Create a `.env` file in the project root with:
     ```env
     NEWS_API_KEY=your-api-key-here
     ```
   - Alternatively, input the key through the application’s sidebar.

4. **Run the application**  
   ```bash
   streamlit run app.py
   ```

5. **Access the application**  
   Open a browser and navigate to `http://localhost:8501`.

## Screenshots

- News Feed: Browse the latest news with AI-generated summaries.  
  [Insert path/to/news_feed_screenshot.png]
- Sentiment Analysis: View sentiment scores for each article.  
  [Insert path/to/sentiment_screenshot.png]

*Replace placeholders with actual image paths hosted on GitHub or an external service.*

## Contributions

- **Soumin Mujumdar**: Co-developed the Streamlit frontend, integrated NewsAPI, implemented NLP models for summarization and sentiment analysis, and collaborated on debugging and testing.
- **Vidhi Binwal**: Co-developed the Streamlit frontend, designed custom CSS for the user interface, implemented user preference logic, and collaborated on debugging and testing.
- Both contributors ensured a robust, optimized application through joint efforts in development and testing.

## Testing

To run unit tests for API calls and NLP functions:
```bash
pytest tests/
```

*Ensure the `tests/` folder contains appropriate test scripts.*

## Live Demo

Access the application at [https://ai-news-summarizer.streamlit.app](https://ai-news-summarizer.streamlit.app).  
*Update with the actual deployment link if available.*

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For questions or feedback, please use [GitHub Issues](https://github.com/your-username/ai-news-summarizer/issues) or email your-email@example.com.

## Acknowledgments

- NewsAPI for providing real-time news data.
- Hugging Face for NLP models and resources.
- Symbiosis Institute of Technology, Pune, for supporting innovation and learning.
