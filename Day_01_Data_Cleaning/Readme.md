### 📁 Task 01 – Data Cleaning and Pre-processing

---

### 📊 Dataset

* **Name:** Customer Personality Analysis
* **Source:** [Kaggle – Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
* **File Used:** `marketing_campaign.csv`

---

### 🛠 Tools & Technologies

* **Microsoft Excel:** Used for manual inspection, duplicate removal, and value standardization.
* **Python:** Used for programmatic data cleaning with the following libraries:
    * `pandas`
    * `numpy`
    * `jupyter notebook`

---

### 🔧 Steps Performed

#### ✅ Excel-Based Pre-processing

* Identified and replaced 24 missing values in the **`Income`** column.
* Removed 203 rows labelled as "2n Cycle" in **`Education`** and updated them to "Undergraduate".
* Applied **Remove Duplicates** on all columns.
* Performed basic data validation and formatting.

#### ✅ Python-Based Cleaning (`data_cleaning.ipynb`)

* Loaded the dataset using `pd.read_csv()` with the correct delimiter (`sep=';'`).
* Stripped whitespace from column names using `df.columns.str.strip()`.
* Checked for nulls (`df.isnull().sum()`), data types, and duplicates.
* Imputed missing **`Income`** values with the mean (`df['Income'].fillna(df['Income'].mean())`).
* Standardized column values and removed duplicates.
* Converted **`Dt_Customer`** to datetime format with `pd.to_datetime()`.
* Exported the cleaned data to `cleaned_dataset/marketing_campaign_cleaned.csv`.

---

### 📂 Deliverables

| File Name                                      | Description                                              |
| :--------------------------------------------- | :------------------------------------------------------- |
| `cleaned_data_excel.csv`                       | The cleaned version after Excel preprocessing.           |
| `cleaned_data_python.csv`                      | The final cleaned data after Python processing.          |
| `data_cleaning.ipynb`                          | The Jupyter Notebook with step-by-step Python cleaning.  |
| `interview_questions/task_1_questions_and_answers.md` | Common interview Q&A based on this task.                 |

---

### 🧠 Interview Prep Summary

Key questions related to:
* Missing value handling
* Duplicate removal
* Outlier treatment
* Column standardization
* Inconsistent formatting

✅ Answers are provided in the following file: `interview_questions/task_1_questions_and_answers.md`

---

### 📸 Screenshots

*Include these if Excel transformations were done manually:*
* Before and after views of duplicate removal
* Missing value identification
* Education column standardization
