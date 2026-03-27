# Book Recommendation Engine using KNN

This project is a **Book Recommendation Engine** built using the **K-Nearest Neighbors (KNN)** algorithm. It was developed as part of the **FreeCodeCamp "Machine Learning with Python"** certification.

## 📌 Project Overview
The goal of this project is to create a model that recommends books similar to a given title based on user ratings. It uses the **Book-Crossings dataset**, which contains over 1.1 million ratings of 270,000 books by 90,000 users.



## 🛠️ Technologies Used
- **Python**: Core programming language.
- **Pandas**: For data cleaning and manipulation.
- **Scikit-learn**: To implement the `NearestNeighbors` model.
- **SciPy**: For creating sparse matrices (`csr_matrix`) to optimize memory.

## 🚀 How it Works
1. **Data Filtering**: To ensure statistical significance, users with less than 200 ratings and books with less than 100 ratings were removed from the dataset.
2. **Pivot Table**: The data was transformed into a 2D matrix (Pivot Table) where rows represent book titles and columns represent users, filled with rating values.
3. **KNN Model**: The model uses **Cosine Similarity** metric to measure the distance between book vectors and find the "closeness" of instances.
4. **Recommendation**: A function named `get_recommends` was created to return the 5 most similar books for any given title found in the dataset along with their distances.

## 💻 Live Demo (Google Colab)
You can view, fork, and run the complete code directly on Google Colab:

👉 **[Run on Google Colab](https://colab.research.google.com/drive/1z34YnMqJ-DfjeK8WiXfQwbZ8ESzRkcW1?usp=sharing)**

## 📊 Result Example
When calling `get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")`, the model returns:
- `The Vampire Lestat (Vampire Chronicles, Book II)`
- `The Tale of the Body Thief (Vampire Chronicles (Paperback))`
- `Interview with the Vampire`
- ...and others.

---
Developed by **Md. Anwar Hossen** as part of the FreeCodeCamp Machine Learning Curriculum.
