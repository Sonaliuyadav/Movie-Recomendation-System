# Movie Recommendation System

This repository contains a Python-based movie recommendation system, implemented using various recommendation techniques. The system is designed to suggest movies to users based on different approaches, such as correlation, K-Nearest Neighbours (KNN), and collaborative filtering.

## Table of Contents
- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [How to Run](#how-to-run)
- [Modules](#modules)
  - [Section A: Simple Recommendation System](#section-a-simple-recommendation-system)
  - [Section B: Recommendation System using KNN](#section-b-recommendation-system-using-knn)
  - [Section C: Collaborative Filtering Recommendation Model](#section-c-collaborative-filtering-recommendation-model)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to build a movie recommendation system in Python. The system suggests movies to users based on:
1. **Correlation-based recommendations**: Suggesting similar movies by comparing their ratings.
2. **K-Nearest Neighbours (KNN)**: Using the KNN algorithm to find movies similar to those a user has liked.
3. **Collaborative Filtering**: Using user behavior data to recommend movies based on what similar users have watched. The system implements both memory-based methods (user-item and item-item filtering) and model-based methods (like Singular Value Decomposition - SVD).

## Project Structure

```
Movie-Recommendation-System/
│
├── Section_A_Simple_Recommendation_System.ipynb   # Basic correlation-based recommendation system
├── Section_B_KNN_Recommendation_System.ipynb       # KNN-based movie recommendation
├── Section_C_Collaborative_Filtering.ipynb         # Collaborative filtering (SVD & memory-based methods)
├── data/                                           # Movie datasets (ratings, movies)
│   ├── movies.csv
│   ├── ratings.csv
├── README.md                                       # Project documentation
└── requirements.txt                                # Required Python packages
```

## Tech Stack
- **Python 3.x**
- **Libraries**: 
  - pandas
  - numpy
  - scikit-learn
  - Surprise (for collaborative filtering)
  - matplotlib (for visualization)
  - seaborn (for enhanced data visualization)

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Movie-Recommendation-System.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Movie-Recommendation-System
   ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run each notebook to explore different recommendation models:
   - **Section A**: `Section_A_Simple_Recommendation_System.ipynb`
   - **Section B**: `Section_B_KNN_Recommendation_System.ipynb`
   - **Section C**: `Section_C_Collaborative_Filtering.ipynb`

## Modules

### Section A: Simple Recommendation System
- This section implements a basic recommendation system by calculating correlations between movie ratings. It uses the pandas `corrwith()` method to find similarities between movies and suggest the most correlated ones.

### Section B: Recommendation System using KNN
- This section uses the K-Nearest Neighbours (KNN) algorithm to recommend movies based on similarities between user preferences. KNN identifies movies that are most similar to those a user has liked.

### Section C: Collaborative Filtering Recommendation Model
- Collaborative filtering methods are used to recommend movies based on user behavior. This section implements:
  - **Memory-based methods**: User-item and item-item filtering.
  - **Model-based methods**: Singular Value Decomposition (SVD) for more accurate movie recommendations.

## Contributing

Contributions are welcome! If you'd like to improve the project, please feel free to submit a pull request. Here are a few ways you can contribute:
- Add new recommendation algorithms.
- Enhance the user interface (e.g., with Flask or Streamlit).
- Improve the data preprocessing steps.
- Fix any bugs or improve the code efficiency.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
