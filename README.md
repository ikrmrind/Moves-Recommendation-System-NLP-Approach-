# 🎬Movie Recommendation Engine
> A machine learning-powered movie recommendation web app that uses **NLP** to analyze movie attributes and deliver highly accurate, content-based recommendations — wrapped in a modern, **iOS-inspired glassmorphism interface**.

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=flat&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-2.x-000000?style=flat&logo=flask&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---
<img width="824" height="441" alt="image" src="https://github.com/user-attachments/assets/168c7562-b151-4fc3-92ef-e017508544c4" />


## ✨ Features

- 🧠 **Content-Based Filtering** — Uses **TF-IDF** (Term Frequency–Inverse Document Frequency) vectorization to analyze movie genres, overviews, and taglines.
- 📐 **Cosine Similarity Scoring** — Mathematically calculates similarity between thousands of films to serve the **top 10 closest matches**.
- 🎨 **Modern UI/UX** — Built with **Tailwind CSS**: responsive 2-column grid, soft shadow elevations, active touch reflexes, and floating glassmorphism navigation.
- ⚡ **Lightweight Backend** — **Flask**-powered API serving pre-computed models for rapid response times.

---

## 🛠️ Tech Stack

| Category | Technologies Used |
| --- | --- |
| **Machine Learning** | Python, Scikit-Learn, Pandas, NumPy, Pickle |
| **Backend** | Flask |
| **Frontend** | HTML5, Tailwind CSS |
| **Algorithms** | TF-IDF Vectorizer, Cosine Similarity |

---

## 🚀 Installation & Setup

**1. Clone the repository**

```bash
git clone https://github.com/ikrmrind/Moves-Recommendation-System-NLP-Approach-.git
cd Moves-Recommendation-System-NLP-Approach-

A machine learning-powered movie recommendation web application. This project uses Natural Language Processing (NLP) to analyze movie attributes and deliver highly accurate, content-based recommendations wrapped in a modern, iOS-inspired glassmorphism interface.

## ✨ Features

* **Content-Based Filtering:** Utilizes TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to analyze movie genres, overviews, and taglines.
* **Cosine Similarity Scoring:** Mathematically calculates the exact similarity between thousands of films to serve the top 10 closest matches.
* **Modern UI/UX:** Built with Tailwind CSS, featuring a responsive 2-column grid, soft shadow elevations, active touch reflexes, and floating glassmorphism navigation.
* **Lightweight Backend:** Flask-powered API serving pre-computed models for rapid response times.

## 🛠️ Tech Stack

| Category | Technologies Used |
| --- | --- |
| **Machine Learning** | Python, Scikit-Learn, Pandas, Numpy, Pickle |
| **Backend** | Flask |
| **Frontend** | HTML5, Tailwind CSS |
| **Algorithms** | TF-IDF Vectorizer, Cosine Similarity |

## 🚀 Installation & Setup

**1. Clone the repository**

```bash
git clone https://github.com/ikrmrind/Moves-Recommendation-System-NLP-Approach-.git
cd

```

**2. Create a virtual environment (Optional but recommended)**

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

```

**3. Install dependencies**

```bash
pip install flask pandas numpy scikit-learn

```

**4. Add your model files**
Ensure the following exported machine learning files are placed in the root directory alongside `app.py`:

* `vec_tfidf.pkl`
* `indices.pkl`
* `df.pkl`

**5. Run the application**

```bash
python app.py

```

The application will be available at `[http://127.0.0.1:5000/](http://127.0.0.1:5000/)`.

## 📁 Project Structure

```text
rewire_cinema/
│
├── app.py                 # Flask application and routing
├── model_training.ipynb   # Jupyter notebook containing the ML pipeline
├── vec_tfidf.pkl          # Pickled TF-IDF matrix
├── indices.pkl            # Pickled pandas Series mapping titles to indices
├── df.pkl                 # Pickled dataframe with movie metadata
└── templates/
    └── index.html         # Tailwind CSS frontend interface

```

## 🧠 How It Works

The recommendation engine is built on a content-based filtering algorithm. During the training phase, textual metadata (genres, overviews, and taglines) for over 45,000 movies is combined into a single "tags" string. This text is preprocessed (lowercased, punctuation removed, stop words stripped, and lemmatized) and converted into a matrix of TF-IDF features.

When a user searches for a movie, the application retrieves its pre-computed TF-IDF vector, calculates the cosine similarity against all other vectors in the dataset, and returns the top 10 most mathematically similar films.

---

**Author:** Muhammad Ikram
*Machine Learning Developer*

---

Would you like me to write up a quick requirements.txt file for this repo so visitors can install the dependencies with a single command?
