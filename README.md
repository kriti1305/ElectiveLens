# 🎓 ElectiveLens

### AI-Powered Elective Recommendation System

**ElectiveLens** is a machine learning-based recommendation system that helps students identify elective subjects that best match their interests, skills, academic profile, and career preferences.

The system analyzes a student's profile and compares it with available elective subjects using **TF-IDF text representation**, **Cosine Similarity**, and **Jaccard Similarity** to generate relevant recommendations.

---

## 🚀 Features

* 🎯 Personalized elective recommendations
* 🧠 NLP-based text processing
* 📊 TF-IDF feature representation
* 🔍 Cosine Similarity for semantic matching
* 🔗 Jaccard Similarity for keyword overlap
* 📈 Combined quality/relevance scoring
* 📁 CSV-based dataset support
* 🖥️ Simple and easy-to-use application interface
* 🧪 Automated testing with Pytest

---

## 🔄 How It Works

```text
Student Profile
       ↓
Text Preprocessing
       ↓
TF-IDF Representation
       ↓
Cosine Similarity
       +
Jaccard Similarity
       ↓
Combined Quality Score
       ↓
Ranked Elective Recommendations
```

### Recommendation Pipeline

1. **Student Profile Input**

   * Interests
   * Skills
   * Academic information
   * Career preferences

2. **Text Preprocessing**

   * Cleaning and normalization
   * Tokenization
   * Removal of unnecessary text

3. **TF-IDF Representation**

   Student and elective descriptions are converted into numerical vectors using Term Frequency–Inverse Document Frequency (TF-IDF).

4. **Similarity Calculation**

   Two complementary similarity measures are used:

   * **Cosine Similarity** — measures similarity between TF-IDF vectors.
   * **Jaccard Similarity** — measures overlap between important terms.

5. **Quality Score**

   The similarity results are combined to calculate an overall relevance score.

6. **Recommendation**

   Electives are ranked according to their scores and the most relevant options are presented to the student.

---

## 🛠️ Tech Stack

| Technology       | Purpose                            |
| ---------------- | ---------------------------------- |
| **Python**       | Core development                   |
| **Pandas**       | Data processing                    |
| **NumPy**        | Numerical operations               |
| **Scikit-learn** | TF-IDF and similarity calculations |
| **Pytest**       | Automated testing                  |
| **CSV**          | Dataset storage                    |
| **Git & GitHub** | Version control                    |

---

## 📂 Project Structure

```text
ElectiveLens/
│
├── data/
│   └── *.csv
│
├── src/
│   └── *.py
│
├── tests/
│   └── test_*.py
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

> The exact structure may vary depending on the current version of the project.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/kriti1305/ElectiveLens.git
cd ElectiveLens
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

Run the main application using:

```bash
python app.py
```

Follow the application's instructions to enter the required student information and generate elective recommendations.

---

## 🧪 Running Tests

The project includes automated tests using **Pytest**.

Run:

```bash
pytest
```

For a more detailed output:

```bash
pytest -v
```

---

## 📊 Recommendation Method

ElectiveLens combines multiple similarity techniques rather than relying on a single metric.

### TF-IDF

TF-IDF identifies words that are important within the student profile and elective descriptions.

### Cosine Similarity

Measures the angle between the student-profile vector and elective vectors to determine how closely they match.

### Jaccard Similarity

Measures the overlap between the important terms present in the student profile and each elective.

### Combined Score

The resulting similarity measures are combined to produce a relevance score used to rank electives.

This approach helps the system consider both **semantic similarity** and **keyword overlap** when generating recommendations.

---

## 🎯 Use Case

Elective selection can be difficult when students have multiple options and limited information about how each subject aligns with their interests.

ElectiveLens aims to provide a **data-driven and personalized approach** by matching student profiles with elective descriptions.

It can be extended to support:

* Career-oriented elective recommendations
* Skill-gap analysis
* Course recommendation systems
* Personalized learning paths
* Academic advising systems

---

## 🔮 Future Improvements

* [ ] Add a web-based user interface
* [ ] Improve recommendation accuracy with additional ML models
* [ ] Add user authentication
* [ ] Store student recommendation history
* [ ] Add visual analytics and recommendation explanations
* [ ] Support larger and more diverse datasets
* [ ] Deploy the application as a cloud-based service

---

## 👩‍💻 Project

**ElectiveLens** is an academic machine learning project focused on applying **Natural Language Processing and similarity-based recommendation techniques** to personalized elective selection.

---

## 📄 License

This project is intended for educational and academic purposes.


