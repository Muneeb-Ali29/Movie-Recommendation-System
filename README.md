# 🎬 Movie Recommendation System

Welcome to the **Movie Recommendation System** repository! This project employs content-based filtering to provide tailored movie recommendations by analyzing key metadata like genres, cast, crew, and keywords. This system is ideal for recommending movies with similar themes, genres, and characteristics to users.

---

## 📋 Project Overview
This project uses machine learning and Natural Language Processing (NLP) to create a recommendation system based on movie content. The model leverages the metadata from movies and credits datasets to generate meaningful and accurate movie suggestions.

### 🌟 Key Features
- **Content-Based Filtering**: Recommends movies similar to the selected movie based on content metadata.
- **Text Vectorization**: Processes and vectorizes text data from features like cast, crew, genres, and keywords.
- **Similarity Computation**: Uses cosine similarity to calculate the closeness of movies based on their content profiles.

---

## 📊 Datasets
This project uses two datasets:
- **Movies Dataset**: Contains key movie attributes like genres, keywords, language, release date, and more.
- **Credits Dataset**: Includes cast and crew information essential for deeper feature extraction.

> Both datasets contain 4,803 entries, representing individual movies.

---

## 🛠️ Libraries Used
- **NumPy** and **Pandas**: Data manipulation and numerical operations
- **Matplotlib**: Data visualization
- **JSON**: Parsing JSON objects within the data
- **NLTK**: Natural Language Processing for text stemming
- **Scikit-Learn**: Machine learning toolkit for vectorization and similarity measures

---

## 🧑‍💻 Methodology

### 1. **Data Preprocessing**
   - Merged **movies** and **credits** datasets based on `movie_id`.
   - Extracted relevant features such as `cast`, `crew`, `genres`, and `keywords` to create a robust movie profile.

### 2. **Feature Engineering**
   - **Tag Creation**: Combined cast, crew, genres, and keywords into a single textual feature called `tags`.
   - **Text Stemming**: Used `PorterStemmer` to standardize text by reducing words to their roots, e.g., "running" becomes "run".

### 3. **Text Vectorization**
   - Applied `CountVectorizer` to convert the tags feature into numerical format, creating a matrix representation for similarity calculation.

### 4. **Similarity Computation**
   - Calculated cosine similarity across the vectorized tags to identify similar movies.

### 5. **Recommendation System**
   - For a selected movie, the system retrieves the 10 most similar movies based on cosine similarity scores.

---

## 🔍 Key Findings
- **Accurate Genre-Based Recommendations**: Movies are well-aligned by genre, providing precise recommendations.
- **Enhanced Similarity with Keywords and Cast**: Including these features improves recommendation quality, capturing thematic and stylistic similarities.
- **Effective Vectorization**: CountVectorizer and cosine similarity form a solid foundation for content-based recommendations.

---

## 🚀 How to Use
1. **Clone** the repository:
    ```bash
    git clone https://github.com/yourusername/Movie-Recommendation-System.git
    ```
2. **Install the required libraries** (if not already installed):
    ```bash
    pip install numpy pandas matplotlib nltk scikit-learn
    ```
3. **Run the Jupyter Notebook** to see the model in action and explore similar movie recommendations.

---

## 📈 Future Improvements
- **Incorporate User Ratings**: Add collaborative filtering for a hybrid recommendation system.
- **Advanced NLP**: Integrate deep learning NLP models for improved similarity understanding.

---

## 📝 Conclusion
This Movie Recommendation System serves as an efficient content-based model that recommends movies with similar themes and attributes. It provides a foundation for further customization to build a fully personalized recommendation engine.

---

## 🛠️ Acknowledgments
Special thanks to [The Movie Database (TMDb)](https://www.themoviedb.org/) for providing the movie datasets used in this project.

---

### 📬 Contact
For queries or collaboration, reach out through GitHub or email: [muneebali786prof@gmail.com](mailto:muneebali786prof@gmail.com).

**Enjoy exploring and discovering movies!**

---

