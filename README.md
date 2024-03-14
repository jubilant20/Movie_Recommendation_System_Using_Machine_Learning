# Movie_Recommendation_System_Using_Machine_Learning

This is a movie recommendation system based on content based similarity. It recommends movies similar to the user's input movie, based on genres, keywords, taglines, cast, and directors.

## Dataset

The dataset used for this project is from the TMDB `movies.csv` file, which contains information about movies such as title, genres, keywords, taglines, cast, director, budget, and vote average.

## Methodology

1. **Data Cleaning:** Null values in the selected features (`genres`, `keywords`, `tagline`, `cast`, `director`) were replaced with empty strings.

2. **Feature Extraction:** The selected features were combined into a single feature vector using TF-IDF vectorization.

3. **Similarity Calculation:** Cosine similarity was used to calculate the similarity scores between movies based on their feature vectors.

4. **Recommendation Function:** A function was created to recommend movies based on the user's input movie title. It finds the closest match, retrieves the similarity scores, and sorts the movies by similarity score.

5. **Genre-based Recommendation:** Users can also get recommendations based on a specific genre. The system filters movies based on the user's input genre and suggests similar movies from that genre.

6. **Director-based Recommendation:** Users can get recommendations based on their favorite director. The system lists movies directed by the specified director.

7. **Rating-based Recommendation:** Users can input their preferred movie rating, and the system suggests movies with ratings equal to or greater than the input.

8. **Budget-based Recommendation:** Users can specify a budget range, and the system suggests movies within that budget range.

## Data Visualization

1. **Top 10 Movies by Genre:** Bar chart showing the top 10 movies in a selected genre based on their vote average.

2. **Distribution of Movie Ratings:** Histogram showing the distribution of movie ratings in the dataset.

3. **Top 10 Movies by Director:** Horizontal bar chart showing the top 10 movies directed by a selected director based on their vote average.

4. **Top 10 Movies by Budget:** Bar chart showing the top 10 movies in a specified budget range based on their budget.

## Usage

1. Install the required libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`.
2. Run the `recommend_movies_by_title`, `recommend_movies_by_genre`, `recommend_movies_by_director`, `recommend_movies_by_rating`, or `recommend_movies_by_budget` functions with appropriate inputs to get movie recommendations.

## Results

The system successfully recommends movies based on user inputs, providing a personalized movie recommendation experience.

## Author

[Jubilant K J](https://github.com/jubilant20)

