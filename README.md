# Predicting Mental Health Treatment-Seeking in the Tech Workplace
<br>This project uses the 2014 Mental Health in Tech Survey to explore how workplace factors impact mental health outcomes among tech workers. It aims to provide insight into how company size, supportiveness, remote work, perceived stigma, and more relate to mental health treatment-seeking behaviors, workplace interference, and fear of consequences.
<br>
<br>Ultimately, this project seeks to model predictors of mental health outcomes using a combination of workplace culture, demographic factors, and individual perceptions.
<br>
<br> ***Note: In it's original form, the mini-projects scope is limited to creating a ML model to predict a target feature, but I hope to add more components and exploration to this project as time goes on.***

## Project Objectives
- Explore relationships between workplace attitudes toward mental health and treatment-seeking behavior.
- Determine how factors like company size, remote work status, and perceived supportiveness relate to negative workplace consequences for mental health conditions.
- Build a machine learning model to predict whether someone seeks treatment for a mental health condition based on their responses. **As time permits/flows, I plan to explore other potential target features in the dataset.**
- Analyze how demographic and workplace factors influence perceived stigma and work interference.
## Dataset Overview
The dataset contains 1,259 responses from tech workers worldwide. Data was sourced from a 2014 Mental Health in Tech Survey (https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey). Key columns include (but are not limited to):
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
- One-Hot encoding for categorical variables
- StandardScaler for numerical features **may remove**

## Mini Project Goals (1-2 Week Focus)
1. Clean and preprocess key features (gender, age, location, etc.)
2. Conduct exploratory data analysis (EDA) in general and on factors potentially driving treatment-seeking behaviors. Future exploration may include:
   - Mental health treatment vs. workplace factors
   - Observed consequences vs. perceptions of stigma
   - Company size vs. supportiveness
   - and more!
6. Train a classification model (Logistic Regression, Random Forest, etc.) to predict:
   - treatment-seeking behavior (binary classification)
7. Evaluate model performance using accuracy, precision, recall, and AUC
8. Visualize key findings and model feature importance

## Key Challenges
- Normalizing text responses (especially for gender and comments)
- Handling missing values thoughtfully without distorting meaning
- Ensuring model interpretability and fairness (especially given sensitive topic)
- Selecting target feature that can represent target focus (mental health). Despite my belief that treatment-seeking was a good target, the case can be made as well to features that measure the perception of the workplace culture, observations of negative consequences for MH needs, feelings on workplace stigma around mental health, and more.
- Using limited survey data (ex. yes/no vs long form responses, limited sample size; majority of participants mostly restricted to certain locations and a certain year, etc) to answer complex and nuanced questions about mental health.

## Repository Structure
```
MHealthWorkplace-Tech/
│
├── Resources/
│   └── 01_mental_health_survey.csv
|   └── 02_KaggleTechSurveyInfo.txt
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
│   └── Findings.txt
│
├── README.md
└── requirements.txt
```
## Possible Extensions (that I may add to this repo, time permitting)
- NLP analysis of open-ended comments (e.g., using topic modeling or sentiment analysis)
- Compare predictions of different ML models (ex. SVM, etc.)
- Build a dashboard (e.g., using JavaScript, Flask API, etc. OR Tableau Public) to make results interactive. Ideally with API connectivty for potential for future participants' data to update visualizations.
- Use clustering to find groups of employees with similar mental health and workplace experiences. Explore reported outcomes and perceptions for each group. Potentially use this to glean insight from their comments, as well (natural language processing (NLP) algo).
- Compare US-based vs. international responses
- Deep dive into the relationship between physical vs. mental health support in companies. Is this an overall issue of unsupportive workplace environments in these participants' tech environments or is perceived lack of support of treatment-seeking specifically mental health related?
- Select other features as target features; look at prediction accuracy with new feature and explore whether this other target feature correlates more to mental health factors of interest for tech workers.

## Author
Project by Arielmy M., created as part of a short-term portfolio mini-project.

### Acknowledgments
I received assistance and/or gathered information from the following sources:
- Stack Overflow (troubleshooting etc.)
- ChatGPT: for quick documentation/templates on python (or python library) functions and parameters
- Data science mentor, Seif D.
