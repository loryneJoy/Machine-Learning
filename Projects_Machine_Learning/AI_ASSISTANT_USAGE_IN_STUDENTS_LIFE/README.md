#  AI Assistant Usage Analysis

This project explores how students interact with an AI assistant in their academic life. Using a dataset of student usage patterns, we perform **Exploratory Data Analysis (EDA)**, visualization, and some preprocessing to uncover insights about session lengths, task types, and overall usage trends.

##  Project Overview

The notebook performs the following key steps:

###  Part A: Basic EDA

1. **Dataset Loading** – Reads the CSV file containing AI assistant usage data.
2. **Data Overview** – Checks dataset shape, column names, and data types.
3. **Missing Values** – Identifies and counts missing data.
4. **Descriptive Statistics** – Summarizes key numerical variables (e.g., `SessionLengthMin`, `TotalPrompts`).
5. **Unique Values** – Analyzes categorical features (`StudentLevel`, `Discipline`, `TaskType`).
6. **Value Counts** – Determines the most common task types.

###  Data Preprocessing

* **Encoding categorical features** using `LabelEncoder` and `OneHotEncoder`.
* Handling missing values if necessary.

###  Visualization & Insights

* Distribution plots (session length, prompts used).
* Bar charts for task types and disciplines.
* Correlation heatmaps to identify relationships between variables.

##  Tools & Libraries Used

* **Python 3**
* **Pandas, NumPy** – Data manipulation
* **Matplotlib, Seaborn** – Visualization
* **Scikit-learn** – Data preprocessing

##  Dataset

The dataset `ai_assistant_usage_student_life.csv` contains:

* **SessionID** – Unique session identifier
* **StudentLevel** – Level of study (e.g., Undergraduate, Graduate)
* **Discipline** – Student’s academic field
* **SessionDate** – Date of AI assistant usage
* **SessionLengthMin** – Session duration in minutes
* **TotalPrompts** – Number of prompts used per session
* **TaskType** – Task performed with AI assistant
* **AI\_AssistanceLevel** – Measured level of assistance required
* **FinalOutcome** – Outcome of session
* **UsedAgain** – Whether the student used the AI again (Boolean)
* **SatisfactionRating** – Feedback rating

##  Results & Findings

From the analysis of **10,000 student sessions**, we found:

* **Session Length & Prompts**

  * Average session length: **\~20 minutes**
  * Longest session: **\~111 minutes**
  * Average number of prompts per session: **\~6**

* **Task Type Popularity**

  * **Writing** tasks were the most common (3,101 sessions).
  * Followed by **Studying** (2,040), **Homework Help** (1,959), and **Coding** (1,948).
  * Less frequent tasks: **Brainstorming** (476) and **Research** (476).

* **Categorical Diversity**

  * **3 student levels** represented.
  * **7 disciplines** included.
  * **6 task types** analyzed.

* **Dataset Quality**

  * No missing values were found in the dataset.

These insights highlight how students rely on AI assistants most frequently for **writing support**, but also make substantial use of them in studying, coding, and homework help.

##  How to Run

1. Clone this repository

   ```bash
   git clone https://github.com/loryneJoy/ai-assistant-usage.git
   cd ai-assistant-usage
   ```
2. Open the notebook in Google Colab.
3. Run cells step by step to reproduce the analysis.

##  Conclusion

This analysis demonstrates that AI assistants are becoming an integral part of student learning. The data shows:

* Students use them **most heavily for writing and academic support tasks**.
* Sessions are typically short but effective, averaging **20 minutes and 6 prompts**.
* The diversity of disciplines and levels represented suggests that AI tools are widely adopted across academic fields.

Overall, AI assistants appear to **enhance productivity and support learning**, making them valuable study companions. This study provides a foundation for further research into **how AI can be optimized for different student needs**.
