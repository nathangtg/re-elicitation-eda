# iZone User Segmentation & Requirements Analysis

**Course:** SWE2033 Requirement Engineering
**Assignment:** Group Assignment 1: Requirements Elicitation & Tool Use
**Project Focus:** Requirements Elicitation and Analysis for the "iZone" University Portal
**Academic Session:** April 2025

---

## 1. Project Overview

This project undertakes a comprehensive requirements engineering process for the **iZone platform**, an essential student and alumni portal at Sunway University and College. Our primary objective is to elicit, analyze, and document user requirements to inform the enhancement of iZone. This initiative simulates a real-world scenario where understanding user needs is paramount for successful software evolution.

The core activities of this project include:
*   **Requirements Elicitation:** Employing anonymized surveys and semi-structured interviews to gather data from key stakeholders (current students and alumni).
*   **Data Analysis & User Segmentation:** Processing collected data to identify distinct user segments based on their interactions, satisfaction levels, and demographic profiles.
*   **Requirements Identification:** Deriving key functional requirements (FRs) reflecting user tasks and desired features, and non-functional requirements (NFRs) addressing system quality attributes like performance, usability, and stability.
*   **Prioritization & Justification:** Analyzing user feedback to determine priority areas for improvement and substantiating these with data-driven insights.

This endeavor aligns with industry best practices by emphasizing a user-centric approach to requirements engineering, ensuring that proposed enhancements are grounded in verified user needs and pain points.

## 2. Objectives

The strategic objectives of this project, in line with the SWE2033 Group Assignment, are:
*   To gain practical experience in the systematic elicitation, documentation, and management of software requirements for a real-world application.
*   To conduct thorough stakeholder analysis, focusing on the primary users of the iZone portal: current students and alumni.
*   To apply and evaluate the effectiveness of at least two distinct requirements elicitation techniques (surveys and interviews).
*   To document elicited requirements in a structured and comprehensible format, suitable for subsequent design and development phases.
*   To leverage appropriate tools for data analysis (Python with Pandas, Matplotlib, Seaborn) and to simulate the use of requirements management/collaboration tools.
*   To deeply understand the diverse needs, expectations, and frustrations of different iZone user segments.
*   To deliver actionable, data-backed recommendations for the strategic improvement of the iZone platform.

## 3. Methodology: Requirements Elicitation & Analysis

A multi-method approach was adopted for requirements elicitation to ensure both breadth and depth in understanding user needs for the iZone portal.

### 3.1. Elicitation Strategy

The core strategy involved:
1.  **Broad Quantitative & Qualitative Data Collection:** Using anonymized online surveys to reach a large and diverse group of current students and alumni, capturing common usage patterns, satisfaction levels, and pain points.
2.  **In-depth Qualitative Insights:** Conducting semi-structured interviews with selected representatives from key stakeholder groups (current students and alumni) to explore specific experiences, contextual factors, and detailed suggestions in greater detail.

This dual approach allows for cross-validation of findings and provides a holistic view of user requirements.

### 3.2. Elicitation Techniques Employed

#### 3.2.a. Anonymized Online Surveys
*   **Objective:**
    1.  Identify common iZone usage patterns, overall satisfaction, and prevalent pain points.
    2.  Gather user opinions on existing features and solicit suggestions for new functionalities.
    3.  Collect quantitative data on the perceived importance of various portal features and potential enhancements.
*   **Instrument:** A structured online questionnaire developed using Google Forms (see Appendix A of the full report), comprising 19 questions (multiple-choice, Likert scales, open-ended).
*   **Distribution & Sampling:** Distributed via online channels (email, WhatsApp, Microsoft Teams) using convenience and snowball sampling techniques from May 29th to June 18th, 2025. A QR code was also physically distributed on campus to boost participation.
*   **Respondents:** A total of **211 responses** were collected, primarily from current Sunway University students (42.7%), Sunway University alumni (23.7%), Sunway College alumni (23.2%), and current Sunway College students (10.4%).
*   **Challenges & Mitigation:**
    *   *Slow Initial Response Rate:* Mitigated by active on-campus promotion using QR codes.
    *   *Vague Questions (for some anonymous respondents):* Identified areas requiring further clarification, which were then explored in the semi-structured interviews.
*   **Key Output Sections (from Survey):** Demographics, iZone Usage & Experience, Specific Feedback & Potential Enhancements, Student Involvement & Feature Prioritization. (Detailed charts and figures are available in the full project report).

#### 3.2.b. Semi-Structured Interviews
*   **Objective:**
    1.  Gain genuine, in-depth insights into individual user experiences with the iZone system.
    2.  Identify specific pain points and gather detailed recommendations that might not be fully captured by surveys.
    3.  Explore underlying reasons for user satisfaction or dissatisfaction with particular aspects of iZone.
*   **Execution:**
    *   **Platform:** Microsoft Teams for remote, one-on-one sessions.
    *   **Participants:** Three carefully selected stakeholders:
        *   Raymond Tham Chun Keet (Current BSc Computer Science Student, Sunway University)
        *   Sohom Chakma (Current BSc Computer Science Student, Sunway University)
        *   Wong Meng Yong "Enoch" (Alumnus, Diploma in IT, Sunway College; currently Monash University)
    *   **Interviewer:** Jaeden Ting Yiyong (Group Member).
    *   **Format:** Each interview (approx. <4 minutes) followed a pre-designed guide of 10 open-ended questions covering demographics, usage, overall impression, pain points (general, performance, UI), timetable feedback, calendar integration interest, priority improvements, and willingness for future involvement. Sessions were recorded with consent.
*   **Key Output Areas (from Interviews):** Detailed narratives on iZone usage, specific frustrations with UI and performance, opinions on the timetable feature, enthusiasm for calendar integration, and varied perspectives on prioritization. (Full transcripts are available in Appendix B, C, D of the full project report).

### 3.3. Data Analysis & Synthesis
Upon completion of the elicitation phase:
1.  **Survey Data Processing:** Quantitative data from surveys was statistically summarized. Qualitative responses from open-ended questions were themed and analyzed for recurring patterns.
2.  **Interview Data Processing:** Interview recordings were transcribed. Transcripts underwent qualitative content analysis to identify key themes, user stories, and specific requirements.
3.  **Cross-Validation:** Findings from surveys and interviews were triangulated to validate requirements and gain a richer understanding.
4.  **User Segmentation & Requirements Derivation:** The processed data was then fed into the analytical Python script for user segmentation, and derivation of FRs and NFRs as detailed below.

### 3.4. User Segmentation (Post-Elicitation Analysis)
Users are segmented into distinct groups (e.g., Power Users, Frustrated Users, Heavy Users, New/Inactive Users) based on analyzed survey data covering:
*   Usage frequency
*   Overall satisfaction
*   Task diversity
*   Frustration level
*   Affiliation

### 3.5. Requirements Analysis (Functional & Non-Functional - Post-Elicitation Analysis)
*   **Functional Requirements (FRs):** Identified from survey responses about main tasks performed and desired features, as well as interview discussions.
*   **Non-Functional Requirements (NFRs):** Derived from survey questions about frustrations and specific ratings (e.g., mobile usability, stability), and detailed discussions in interviews regarding performance, UI, and usability.

### 3.6. Priority Analysis (Post-Elicitation Analysis)
User-stated priorities from surveys (e.g., "top 3 areas of priority") and explicit statements from interviews were analyzed to understand what improvements users collectively deem most critical.

## 4. Tools & Technologies

*   **Elicitation:**
    *   **Google Forms:** For designing and distributing online surveys.
    *   **Microsoft Teams:** For conducting remote semi-structured interviews and session recording.
*   **Data Analysis & Visualization:**
    *   **Python 3.x:** Primary language for data processing and analysis.
        *   **Pandas:** For data manipulation, cleaning, and structuring.
        *   **NumPy:** For numerical computations.
        *   **Matplotlib & Seaborn:** For generating static visualizations.
*   **Reporting & Collaboration:**
    *   **Jupyter Notebook:** For creating the interactive, narrative analysis report (`iZone_Analysis_Story.ipynb`).
    *   **Microsoft Word/Google Docs (implicitly):** For initial drafting of survey questions, interview guides, and report sections.
    *   **Git & GitHub (assumed):** For version control and collaborative development of analysis scripts and documentation.

## 5. Key Deliverables & Outputs

This project yields the following deliverables, comprehensively documenting the requirements engineering process and its outcomes:

1.  **Full Project Report (External Document - Not in this repo, but referenced):**
    *   Detailed Elicitation Plan, Survey Instrument (Appendix A), Interview Transcripts (Appendix B, C, D), and complete analysis.
2.  **Analysis Script/Notebook:**
    *   The core Python script/Jupyter Notebook (`izone_user_segmentation_analysis.py` or the one used for `iZone_Analysis_Story.ipynb`) that performs the post-elicitation data analysis, segmentation, and requirements derivation.
3.  **User Segmentation & Requirements Analysis Summaries:**
    *   `report/izone_segmentation_analysis_report.txt`: A text-based summary of key segments, their characteristics, and FR/NFR justification based on the analyzed data.
    *   `report/izone_segmentation_analysis_report_data.xlsx`: An Excel file containing pivotal data tables (Segment Characteristics, FR/NFR demand/severity pivots, full segmented dataset).
4.  **Data Visualizations (located in `media/` folder):**
    *   A suite of charts and heatmaps visually representing data quality, segment distributions, satisfaction levels, usage patterns, FR demand, NFR issues, and overall requirement priorities. (See list in previous README version for specifics).
5.  **Narrative Storytelling Notebook:**
    *   `iZone_Analysis_Story.ipynb`: A Jupyter Notebook that synthesizes the analysis findings into a coherent narrative, integrating visualizations and interpretive commentary.
6.  **This README.md file:** Providing an overview of the project, methodology, and deliverables.

These deliverables collectively represent the outputs required by the assignment, including stakeholder analysis, elicitation summaries, identified requirements, and tool usage evidence.

## 6. How to Run the Post-Elicitation Analysis

(This section assumes the elicitation has been completed and data is available in `cleaned_izone_survey_data.csv` format, as used by the Python analysis script).

1.  **Prerequisites:**
    *   Python 3.7+
    *   Jupyter Notebook/JupyterLab
    *   Required Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `openpyxl`. Install using pip:
        ```bash
        pip install pandas numpy matplotlib seaborn openpyxl scikit-learn
        ```
2.  **Input Data:**
    *   Ensure the `cleaned_izone_survey_data.csv` file (derived from the survey elicitation and potentially augmented with themes from interviews) is present in the root directory or provide the correct path. A dummy file will be generated by the script if the actual data file is not found, for demonstration purposes.
3.  **Running the Python Analysis Script (if applicable as standalone):**
    ```bash
    python izone_user_segmentation_analysis.py [path_to_data.csv] [path_to_output_report.txt]
    ```
4.  **Viewing the Jupyter Notebook Analysis Story:**
    *   Navigate to the project directory in your terminal.
    *   Launch Jupyter Notebook or JupyterLab.
    *   Open `iZone_Analysis_Story.ipynb` and execute the cells.

## 7. Key Findings & Insights from Analysis

(This section summarizes findings *after* the elicitation data has been analyzed by the script. Refer to `report/izone_segmentation_analysis_report.txt` and `iZone_Analysis_Story.ipynb` for comprehensive details.)

*   **Prevalence of "Frustrated Users":** A significant user segment expresses notable dissatisfaction, primarily linked to UI outdatedness, system performance, and feature gaps.
*   **Criticality of Core Functions:** Timetable access, academic results, and fee payment remain paramount functional requirements.
*   **Demand for Modernization & Performance:** Strong user desire for UI modernization, improved system performance, enhanced mobile usability, and better navigation.
*   **Calendar Integration is Highly Valued:** Both survey and interview data indicate strong interest in integrating iZone timetable with personal calendar tools (Google/Outlook Calendar).
*   **Varied Segment Needs:** While Power Users are generally satisfied, they also echo concerns about mobile usability. Heavy Users experience more frustrations despite frequent use. Alumni and current students share concerns about UI but may have different priorities for other features.

## 8. Reflection on Elicitation & Analysis Process

*   **Strength of Multi-Method Elicitation:** Combining surveys for breadth and interviews for depth provided a richer, more nuanced understanding of user needs than either method alone. Interviews helped clarify ambiguities from survey responses.
*   **Engagement for Survey Responses:** Active on-campus promotion was crucial for achieving a good survey response rate.
*   **Value of Remote Interviews:** Using MS Teams facilitated convenient participation for interviewees and streamlined recording.
*   **Data Synthesis Challenges:** Integrating qualitative insights from interviews with quantitative survey data requires careful thematic analysis and interpretation to ensure a cohesive understanding.
*   **Tooling for Analysis:** Python and its data science libraries proved effective for processing the collected data and generating actionable insights and visualizations.
*   **Iterative Nature:** The process of drafting survey questions, pilot testing (implicitly), and then using interview findings to elaborate on survey points reflects an iterative approach to requirements gathering.

This project demonstrates a practical application of the requirements engineering lifecycle, from planning elicitation activities to analyzing collected data and formulating data-driven recommendations for a real-world system.