## Movie Recommendation Web Application

### Overview
This web application recommends movies based on user input using a Flask backend with machine learning (ML) model integration for sentiment analysis and web scraping for additional movie details.

### Features
- **Recommendation System:** Provides movie recommendations based on user-selected criteria.
- **Auto-complete Search:** Offers suggestions while typing movie titles.
- **IMDB Reviews Analysis:** Scrapes IMDB for user reviews, analyzes sentiment using a pre-trained ML model.
- **Dynamic Rendering:** Renders movie details, reviews, and cast information dynamically on recommendation pages.

### Technologies Used
- **Python Libraries:** Flask, pandas, numpy, scikit-learn, BeautifulSoup
- **Machine Learning:** Pickle for model serialization, CountVectorizer for text vectorization, cosine_similarity for recommendation scores.
- **Web Technologies:** HTML/CSS, JavaScript (AJAX for asynchronous requests)

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Flask application:**
   ```bash
   python app.py
   ```
   The application will run locally on `http://localhost:5000/`.

### Usage
- **Home Page (`/` or `/home`):**
  - Displays an auto-complete search bar for movie titles.
  - Clicking on a movie title triggers a request to `/populate-matches` for related movies.

- **Recommendation Page (`/recommend`):**
  - Displays detailed information about a selected movie.
  - Renders movie posters, ratings, cast details, and user reviews fetched from IMDB.

### Files and Directories
- **`app.py`**: Flask application file containing routes and main logic.
- **`templates/`**: Directory containing HTML templates for rendering pages.
- **`static/`**: Directory for static files like images and CSS.

### Notes
- Make sure to have Python 3.x installed on your system.
- For development, ensure to set `debug=True` in `app.run()` to enable debugging features.
- Customize or expand functionality by modifying routes and templates as needed.

---
