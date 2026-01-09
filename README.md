# Movies-Recommender-System

### Project Overview
This project implements a Movie Recommendation System that suggests movies based on user preferences and viewing behavior. It uses data analysis and machine learning techniques to deliver personalized recommendations, helping users discover relevant and interesting movies efficiently.
The system also integrates an external movie API to fetch real-time movie posters and metadata. This enhances the user experience by providing visually rich recommendations along with accurate and up-to-date movie information.

### Dataset Source: TMDB 5000 Movie Dataset
The TMDB (The Movie Database) Dataset is a rich collection of movie metadata, sourced via TMDB's API, offering details like titles, budgets, revenues, user ratings, genres, cast, release dates, and plot summaries for thousands of films, ideal for data analysis, building recommendation systems, and exploring trends in cinema.

### Approach

#### 1. Data Understanding and Feature Selection

&#9679; Analyzed the movie dataset and identified relevant features such as title, genres, keywords, overview, cast, and crew.

&#9679; Selected only content-based attributes required for generating recommendations.

#### 2. Data Preprocessing

&#9679; Combined selected features into a single text column for each movie.

&#9679; Performed text cleaning by converting text to lowercase and removing unnecessary words.

#### 3. Feature Extraction
 
&#9679; Converted textual data into numerical vectors using CountVectorizer.

&#9679; Limited the vocabulary size to the top 5,000 most frequent words for efficiency.

#### 4. Similarity Calculation

&#9679; Applied Cosine Similarity to compute similarity scores between movie vectors.               

&#9679; Stored similarity scores for fast recommendation retrieval.

#### 5. Recommendation Generation
 
&#9679; Accepted a movie title as input from the user.         

&#9679; Retrieved movies with the highest cosine similarity scores.      

&#9679; Recommended the top 5 most similar movies.
