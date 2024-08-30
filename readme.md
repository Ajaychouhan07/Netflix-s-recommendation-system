# Movie Recommendation System using Content-Based Filtering

This repository contains a simple movie recommendation system implemented in Python using content-based filtering techniques. The system suggests similar movies to a user based on their input of a favorite movie title.

## How the Recommendation System Works

The recommendation system operates in the following steps:

1. **Data Collection and Pre-Processing**: The system loads movie data from a CSV file, preprocesses it, and extracts relevant features like genres, keywords, taglines, cast, and director. These features are combined into a single text representation for each movie.

2. **Converting Text Data to Feature Vectors**: The combined text features for each movie are converted into numerical feature vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.

3. **Calculating Cosine Similarity**: Cosine similarity is calculated between all pairs of movies based on their feature vectors. This similarity matrix is used to find similar movies for a given input movie.

4. **Getting User Input**: The user is prompted to input their favorite movie name.

5. **Finding Similar Movies**: The system finds the closest match to the user's input among the available movie titles. Then, it retrieves the index of the matched movie and uses the similarity scores to suggest a list of similar movies.

## How to Use the Script

1. Ensure you have Python and required libraries installed.

2. Place your movie data CSV file in the specified location (`/content/drive/MyDrive/Datasets/movies.csv`).

3. Run the script in a suitable environment (e.g., Jupyter Notebook, Google Colab).

4. The script will prompt you to enter the name of your favorite movie.

5. After entering the movie name, the system will display a list of similar movies based on your input.

## Dependencies

The script uses the following Python libraries:

- `numpy`
- `pandas`
- `difflib`
- `scikit-learn`

Make sure to install these libraries using the following command:

```bash
pip install numpy pandas scikit-learn
```

## Disclaimer

This is a basic implementation of a movie recommendation system and is intended for educational purposes only. The effectiveness of the recommendations depends on the quality and quantity of data available.

## Credits

This script was created by Harsh Ranjan.

---

