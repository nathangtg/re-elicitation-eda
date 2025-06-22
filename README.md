# iZone User Segmentation & Requirements Analysis

**Course:** SWE2033 Requirement Engineering
**Assignment:** Group Assignment 1: Requirements Elicitation & Tool Use
**Project Focus:** Analysis of the "iZone" platform (a university portal)
**Academic Session:** April 2025

## Table of Contents
1.  [Project Overview](#project-overview)
2.  [Objectives](#objectives)
3.  [Methodology](#methodology)
    *   [Data Collection (Hypothetical)](#data-collection-hypothetical)
    *   [Data Cleaning & Preparation](#data-cleaning--preparation)
    *   [User Segmentation](#user-segmentation)
    *   [Requirements Analysis (Functional & Non-Functional)](#requirements-analysis-functional--non-functional)
    *   [Priority Analysis](#priority-analysis)
4.  [Tools Used](#tools-used)
5.  [Key Deliverables & Outputs](#key-deliverables--outputs)
6.  [How to Run the Analysis](#how-to-run-the-analysis)
7.  [Key Findings & Insights](#key-findings--insights)
8.  [Reflection on Challenges (Brief)](#reflection-on-challenges-brief)

## 1. Project Overview

This project focuses on conducting a comprehensive requirements elicitation and analysis for the **iZone platform**, a real client within the Sunway campus ecosystem (simulated as a university portal for this analysis). The goal is to understand its current user base, their needs, pain points, and to derive actionable insights for future improvements, aligning with the principles of requirements engineering.

The analysis involves:
*   Segmenting iZone users based on their survey responses (usage, satisfaction, demographics).
*   Identifying key functional and non-functional requirements.
*   Analyzing the priorities for improvement from the user's perspective.
*   Justifying these requirements based on data-driven insights.

This project simulates the initial phases of a software development lifecycle, emphasizing the critical role of understanding user needs before design and implementation.

## 2. Objectives

The primary objectives of this analysis, aligning with the Group Assignment, are:
*   To gain hands-on experience in eliciting, documenting, and managing requirements for a software project.
*   To identify and analyze key stakeholders (simulated through survey respondent data).
*   To apply at least two different elicitation techniques (simulated through survey design and data interpretation).
*   To document requirements in a structured format (achieved through the analysis scripts and generated reports).
*   To utilize a requirements management or collaboration tool (Python with Pandas, Matplotlib, Seaborn for analysis; the output could be fed into tools like JIRA).
*   To understand the needs and frustrations of different iZone user segments.
*   To provide data-backed recommendations for improving the iZone platform.

## 3. Methodology

### Data Collection (Hypothetical)
For this analysis, we are using a pre-existing (or simulated) dataset: `cleaned_izone_survey_data.csv`. This dataset is assumed to be the output of a survey designed to capture user interactions, satisfaction, pain points, and desired features for the iZone platform. The survey implicitly acts as one of our primary elicitation techniques.

### Data Cleaning & Preparation
The Python script `izone_user_segmentation_analysis.py` (or the script embedded in the Jupyter Notebook) performs initial data loading and preparation. This includes:
*   Loading the cleaned survey data.
*   Mapping categorical data (e.g., usage frequency, affiliation) to numerical values for analysis.
*   Calculating derived metrics like task diversity and frustration level.

### User Segmentation
Users are segmented into distinct groups (e.g., Power Users, Frustrated Users, Heavy Users, New/Inactive Users) based on:
*   Usage frequency (`usage_frequency_numeric`)
*   Overall satisfaction (`overall_satisfaction`)
*   Task diversity (`task_diversity`)
*   Frustration level (`frustration_level`)
*   Affiliation (`is_current_student`)

### Requirements Analysis (Functional & Non-Functional)
*   **Functional Requirements (FRs):** Analyzed based on `main_tasks__*` columns (what users do) and specific feature columns like `calendar_integration`. Demand rates for each FR are calculated per user segment.
*   **Non-Functional Requirements (NFRs):** Analyzed based on `most_frustrating__*` columns (user pain points) and satisfaction ratings for aspects like `mobile_usability`, `attendance_satisfaction`, and `announcements_ease`. Issue severity for each NFR is calculated per user segment.

### Priority Analysis
User-stated priorities (from `top_priorities__*` columns) are analyzed to understand what improvements users deem most important.

## 4. Tools Used

*   **Python 3.x:** Primary language for data analysis.
    *   **Pandas:** For data manipulation and analysis.
    *   **NumPy:** For numerical operations.
    *   **Matplotlib & Seaborn:** For data visualization.
    *   **Scikit-learn:** (Potentially, though not heavily used in the provided script's final version for segmentation logic itself, which is rule-based).
*   **Jupyter Notebook:** For creating a narrative report (`iZone_Analysis_Story.ipynb`) that combines code, visualizations, and explanatory text.
*   **Git & GitHub (assumed):** For version control and collaboration.
*   **(Hypothetical/Next Step) JIRA/Google Docs:** The outputs of this analysis (user stories, requirement lists) would typically be managed in such tools. The current project uses Python for analysis and `.txt`/`.xlsx` for reporting.

## 5. Key Deliverables & Outputs

This repository/project contains the following key outputs, demonstrating the elicitation and analysis process:

1.  **Analysis Script/Notebook:**
    *   The core Python script/Jupyter Notebook (`izone_user_segmentation_analysis.py` or the one that generated the notebook) that performs the segmentation and requirements analysis.
2.  **User Segmentation & Requirements Analysis Report:**
    *   `report/izone_segmentation_analysis_report.txt`: A text-based summary of segments, characteristics, and requirements justification.
    *   `report/izone_segmentation_analysis_report_data.xlsx`: Excel file containing key data tables (Segment Characteristics, FR/NFR pivots, Segmented Data).
3.  **Visualizations (in `media/` folder):**
    *   `media/data_quality_visualizations.png`: Overview of survey data quality.
    *   `media/seg_dist_pie.png`: User segment distribution.
    *   `media/seg_satisfaction_box.png`: Satisfaction distribution by segment.
    *   `media/seg_usage_freq_box.png`: Usage frequency by segment.
    *   `media/taskdiv_vs_frustration.png`: Task diversity vs. frustration by segment.
    *   `media/segment_radar.png` (or line plot): Segment characteristics profile.
    *   `media/student_pct_bar.png`: Student percentage by segment.
    *   `media/fr_heatmap.png`: Functional requirements demand by segment.
    *   `media/nfr_heatmap.png`: Non-functional requirements issues by segment.
    *   `media/priority_matrix.png`: Top requirements by overall importance.
4.  **Narrative Storytelling Notebook:**
    *   `iZone_Analysis_Story.ipynb`: A Jupyter Notebook presenting the analysis findings in a storytelling format, integrating visualizations and interpretations.
5.  **This README.md file.**

These deliverables collectively represent:
*   **Stakeholder Analysis Document:** Implicit in the segmentation and characteristic analysis.
*   **Elicitation Plan & Execution Summary:** The methodology section and the script describe the approach.
*   **Techniques used:** Survey data analysis is the primary technique.
*   **Raw Elicitation Outputs:** The `cleaned_izone_survey_data.csv` (input) and `report/izone_segmentation_analysis_report_data.xlsx` (processed data).
*   **Initial Requirement List or User Stories:** FR and NFR lists in the report and heatmaps.
*   **Tool Output Evidence:** The generated reports, visualizations, and the script itself.

## 6. How to Run the Analysis

1.  **Prerequisites:**
    *   Python 3.7+
    *   Jupyter Notebook/JupyterLab (if running the `.ipynb` file)
    *   Required Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `openpyxl`. Install using pip:
        ```bash
        pip install pandas numpy matplotlib seaborn openpyxl scikit-learn
        ```
2.  **Data:**
    *   Ensure the `cleaned_izone_survey_data.csv` file is present in the root directory or provide the correct path to it. If it's not available, the script will generate a `dummy_cleaned_izone_survey_data.csv` for demonstration.
3.  **Running the Python Script (if a standalone .py script is the main driver):**
    ```bash
    python izone_user_segmentation_analysis.py [path_to_data.csv] [path_to_output_report.txt]
    ```
    If no arguments are provided, it will look for `cleaned_izone_survey_data.csv` or create the dummy file, and output to `segmentation_analysis_report.txt` (or `dummy_segmentation_analysis_report.txt`).
4.  **Viewing the Jupyter Notebook:**
    *   Navigate to the project directory in your terminal.
    *   Launch Jupyter Notebook or JupyterLab:
        ```bash
        jupyter notebook
        # or
        jupyter lab
        ```
    *   Open `iZone_Analysis_Story.ipynb`.
    *   Run the cells to see the output and visualizations. The notebook assumes images are in the `media/` folder and the report is in the `report/` folder.

## 7. Key Findings & Insights

(Refer to `report/izone_segmentation_analysis_report.txt` and `iZone_Analysis_Story.ipynb` for detailed findings. A brief summary:)

*   **Dominant "Frustrated Users" Segment:** A significant portion of users (approx. 50.2%) are classified as frustrated, highlighting major areas for improvement.
*   **Core FRs are Crucial:** Timetable, Academic Results, and Fee Payments are highly demanded across active segments.
*   **Performance & UI/UX are Key NFR Concerns:** Slow performance and outdated UI are major pain points. Mobile experience also needs significant attention.
*   **Distinct Needs of Segments:** Power Users leverage diverse features with high satisfaction, while Heavy Users, despite high usage, face more frustrations.
*   **Priorities:** Improving performance, UI/UX, and ensuring core functionalities are robust and reliable emerge as top priorities.

## 8. Reflection on Challenges (Brief)

*   **Data Limitations:** The analysis is based on the available survey data. Missing data or biases in the survey could affect the results. (For example, the NFR heatmap from the  data didn't show 'NFR2 - UI Modernization' due to a missing column in the dataset, highlighting the dependency on complete input data).
*   **Segmentation Nuances:** Rule-based segmentation is effective but might not capture all user subtleties. More advanced clustering could be explored in a larger project.
*   **Interpreting "Importance":** The "Top Requirements by Overall Importance" chart averages demand/severity. True prioritization would involve business value, effort, and strategic alignment, which are outside the scope of this user-centric analysis.
*   **Tool Usage Simulation:** While Python is used for analysis (a "tool"), the direct use of a dedicated RE tool like JIRA for managing these findings is a subsequent step, simulated here by structured outputs.