# SkillBridge_AI
AI-Powered CV Skill Gap Analysis and Personalized Course Recommendations
1. Project Overview

SkillBridge AI is a proposed AI-powered career development tool designed to help university students and recent graduates identify skill gaps and find suitable learning opportunities.

The planned system will allow users to upload their CVs and select a target occupation. It will compare the skills identified in their CVs with occupational requirements from the O*NET database.

Skills will be classified into three categories:

* Learn: Skills for which the CV provides no supporting evidence.
* Improve: Skills for which some evidence exists, but further development may be needed.
* Sufficient: Skills for which the available evidence appears to meet the target requirements.

The system will recommend beginner-level courses for skills categorized as Learn and intermediate or advanced courses for skills categorized as Improve.

The final goal is to provide users with a personalized learning roadmap.

2. Sustainable Development Goals

The project primarily supports:

SDG 4 – Quality Education (Target 4.4)

By helping individuals identify and develop skills relevant to employment.

It also contributes indirectly to:

SDG 8 – Decent Work and Economic Growth (Target 8.5)

By supporting career readiness and professional development.

3. Datasets

Two publicly accessible datasets were selected for this project.

Dataset 1: O*NET Occupational Database

Source: https://www.onetcenter.org/database.html

Version used: O*NET 31.0

Files analyzed:

* Occupation Data.xlsx
* Essential Skills.xlsx
* Knowledge.xlsx

The O*NET database provides information about occupations and their required skills and knowledge.

Dataset 2: Coursera Course Dataset

Source: https://huggingface.co/datasets/azrai99/coursera-course-dataset

File analyzed:

* coursera_course_2024.xlsx

This third-party dataset contains course titles, descriptions, skills, difficulty levels, and other course-related information.

It will support the planned course recommendation component.

4. Homework 1: Exploratory Data Analysis

Homework 1 focuses on dataset selection, data exploration, preprocessing, and visualization.

The analysis was performed using Python in Google Colab.

### Dataset Overview

| Dataset | Rows | Columns |
|---|---:|---:|
| O*NET Occupations | 1,016 | 3 |
| O*NET Essential Skills | 18,200 | 15 |
| O*NET Knowledge | 60,060 | 15 |
| Coursera Courses | 6,645 | 14 |

Data Preprocessing

The following preprocessing operations were performed:

* Inspected dataset dimensions and missing values.
* Checked for fully duplicated rows.
* Created copies of the original datasets.
* Removed an unnecessary index column from the Coursera dataset.
* Standardized whitespace in selected text fields.
* Examined missing values in course descriptions and difficulty levels.

Key EDA Findings

* The O*NET Occupation Data table contains 1,016 occupational records.
* Active Listening, Speaking, and Critical Thinking were among the skills with the highest average importance scores.
* The Coursera dataset contains 6,645 course records.
* Beginner-level courses represent the largest difficulty category.
* Data Analysis, Python Programming, and Machine Learning were among the most frequently listed course skills.
* The Coursera dataset contains 778 missing values in the Level column and 10 missing values in the Description column.

These findings help evaluate the suitability of the datasets for the proposed SkillBridge AI system.

5. Repository Contents

* SkillBridge_AI.ipynb: Python code for data exploration, preprocessing, and visualizations.
* eda_results/: EDA charts generated during the analysis.
* report/: Homework 1 project report.
* README.md: Project documentation.

6. How to Run the EDA

1. Download the O*NET and Coursera datasets from the sources listed above.
2. Open SkillBridge_AI.ipynb in Google Colab.
3. Upload the required Excel files to the /content/ directory.
4. Run the notebook cells in order.
5. Review the generated statistics and visualizations.

The notebook uses Python libraries including pandas, NumPy, Matplotlib, and Seaborn.

7. Future Development

The following components are planned for later project stages:

* CV text extraction and NLP-based skill identification.
* Comparison of CV evidence with occupational requirements.
* Classification into Learn, Improve, and Sufficient.
* Semantic matching between occupational skills and course descriptions.
* Personalized course recommendations.
* A simple user interface and model evaluation.

These components have not yet been implemented in Homework 1.

8. Project Status

Current stage: Homework 1 – Dataset Selection, Exploratory Data Analysis, and Concept Note.

The current repository documents the initial data analysis. The complete AI-powered application will be developed in later stages.
