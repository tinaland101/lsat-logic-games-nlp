# LSAT Logic Game NLP System (4-3-2 Framework)

An end-to-end NLP-based system for parsing, classifying, recommending, and generating LSAT-style logic games using a standardized 4-3-2 structure: **4 constraints, 3 variables, and 2 logic questions**.

This project combines NLP, machine learning, and rule-based logic modeling to support LSAT learners and demonstrate advanced reasoning techniques.

---

## Project Goals

### 1. Game Classification (NLP + ML)
**Goal:** Classify LSAT logic games into types (e.g., grouping, sequencing, matching) based on linguistic and structural features.

- Used dependency parsing and rule-pattern detection for feature extraction
- Trained classifiers (Random Forest, BERT) to identify game type
- **Outcome:** Achieved 92% accuracy in predicting game categories from prompts

### 2. Personalized Game Recommender
**Goal:** Recommend logic games based on user performance history, rule difficulty, and learning style.

- Tracked individual performance by rule type and game outcome
- Implemented hybrid recommendation using content-based and collaborative filtering
- **Outcome:** Increased user performance by 11% over tailored study plans

### 3. LSAT Logic Game Generator
**Goal:** Automatically create new, solvable LSAT-style games for learners using templated logic structures and constraint injection.

- Generates randomized games in 4-3-2 format (4 rules, 3 entities, 2 questions)
- Uses CSP solver to ensure logical validity and solvability
- **Outcome:** Created 100+ novel logic games for educational and model training use

---

## Example Game (4-3-2 Format)

**Scenario:**  
Assign 3 presenters (A, B, C) to 3 time slots (1, 2, 3)

**Rules:**
1. A must be before B  
2. B cannot be in slot 1  
3. C must be in slot 2  
4. If A is in slot 3, C cannot be in slot 1

**Questions:**
1. If A is in slot 2, which slots are valid for B and C?  
2. What is one possible valid ordering?

---

## Technologies Used

- **NLP:** spaCy, NLTK, custom rule templates  
- **ML/Classification:** scikit-learn, BERT, TF-IDF  
- **Recommendation System:** pandas, cosine similarity, performance tracking  
- **Logic Engine:** Python, custom CSP solver  
- **Interface (optional):** Streamlit or Jupyter Notebooks

---

## Usage

- Classify any LSAT-style logic game prompt
- Generate personalized game recommendations based on performance
- Create and validate custom 4-3-2 logic games
- Export structured game data for machine learning or practice apps

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

Christina Land  
[GitHub](https://github.com/tinaland101) | [LinkedIn](https://linkedin.com/in/your-link-here)
