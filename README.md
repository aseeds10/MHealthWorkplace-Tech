# Title Opt 1: Predicting Mental Health Treatment-Seeking in the Tech Workplace
# Title Opt 2: Analyzing and Predicting Mental Health Outcomes in the Tech Industry
**mini intro opt 1** 
<br> Build a cleaned dataset and a machine learning model to predict whether someone seeks mental health treatment based on workplace factors, while highlighting workplace culture's impact.
<>br
<br>**mini intro opt 2** 
<br>This project uses the 2014 Mental Health in Tech Survey to explore how workplace factors impact mental health outcomes among tech workers. It aims to provide insight into how company size, supportiveness, remote work, and perceived stigma relate to mental health treatment, workplace interference, and fear of consequences.
<br>
<br>Ultimately, this project seeks to model predictors of mental health outcomes using a combination of workplace culture, demographic factors, and individual perceptions.

## Project Objectives
- Explore relationships between workplace attitudes toward mental health and treatment-seeking behavior.
- Determine how factors like company size, remote work status, and perceived supportiveness relate to negative workplace consequences for mental health conditions.
- Build a machine learning model to predict whether someone seeks treatment for a mental health condition based on their responses.
- Analyze how demographic and workplace factors influence perceived stigma and work interference.
## Dataset Overview
The dataset contains 1,259 responses from tech workers worldwide. Key columns include:
- treatment: Whether the respondent has sought treatment for a mental health condition.
- obs_consequence: Whether the respondent has observed negative consequences in the workplace for others with mental health conditions.
- mental_health_consequence: Perceived likelihood of facing negative consequences if discussing a mental health issue with their employer.
- no_employees: Size of the company.
- remote_work: Whether the respondent works remotely.
- tech_company: Whether the company is primarily a tech company.
- benefits, care_options, wellness_program, seek_help: Company-provided resources for mental health.

## Methods & Tools
- Python / Jupyter Notebook
- Pandas / NumPy / Matplotlib / **Seaborn (may remove)** for data cleaning and visualization
- Scikit-learn for machine learning
- Label encoding & One-Hot encoding for categorical variables
- StandardScaler for numerical features

## Mini Project Goals (1-Week Focus)
1. Clean and preprocess key features (gender, age, location, etc.)
2. Conduct exploratory data analysis (EDA) on:
3. Mental health treatment vs. workplace factors
4. Observed consequences vs. perceptions of stigma
5. Company size vs. supportiveness
6. Train a classification model (Logistic Regression, Random Forest, etc.) to predict:
   - treatment-seeking behavior (binary classification)
7. Evaluate model performance using accuracy, precision, recall, and AUC
8. Visualize key findings and model feature importance

## Key Challenges
- Normalizing text responses (especially for gender, state, and country)
- Handling missing values thoughtfully without distorting meaning
- Ensuring model interpretability and fairness (especially given sensitive topic)
- Using limited survey data (ex. yes/no vs long form responses) to answer complex and nuanced questions about mental health.

## Repository Structure
```
MHealthWorkplace-Tech/
│
├── Resources/
│   └── mental_health_survey.csv
|   └── TipsForML-KaggleTechSurvey.txt
│
├── notebooks/
|   └── 01_RawExplore.ipynb
|   └── 02_CleanSQL.ipynb
│   └── 03_VizWork.ipynb
│   └── 04_Machine1.ipynb
│
├── outputs/
│   └── visuals/
│   └── MLmodel/
│
├── README.md
└── requirements.txt
```
## Possible Extensions (that I may add to this repo, time permitting)
- NLP analysis of open-ended comments (e.g., using topic modeling or sentiment analysis)
- Compare predictions of different ML models (SVM, XGBoost, etc.)
- Build a dashboard (e.g., using Streamlit) to make results interactive
- Use clustering to find groups of employees with similar mental health and workplace experiences
- Compare US-based vs. international responses
- Add temporal analysis (timestamps) if viable
- Deep dive into the relationship between physical vs. mental health support in companies

## Author
Project by Arielmy M., created as part of a short-term portfolio mini-project under the guidance of mentor Seif D. :)

### Acknowledgments
I received assistance and/or gathered information from the following sources:
- Stack Overflow
- ChatGPT: for quick documentation/templates on python (or python library) functions
- data science mentor, Seif D.
- [**ADD MORE HERE**]
