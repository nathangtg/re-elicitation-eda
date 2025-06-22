# iZone Requirements Engineering Project

**Course:** SWE2033 Requirement Engineering  
**Assignment:** Group Assignment 1: Requirements Elicitation & Tool Use  
**Session:** April 2025  

## Project Overview

This project conducts comprehensive requirements engineering for the **iZone portal** at Sunway University and College. We employed systematic elicitation techniques to gather user requirements from students and alumni, then analyzed the data to identify user segments and derive functional/non-functional requirements.

## Objectives

- Apply requirements elicitation techniques (surveys and interviews) to a real-world system
- Analyze stakeholder needs through user segmentation
- Document functional and non-functional requirements based on user feedback
- Provide data-driven recommendations for system improvement
- Demonstrate proficiency with requirements engineering tools and analysis methods

## Methodology

### Requirements Elicitation Techniques

**1. Online Survey**
- **Participants:** 200+ respondents (students and alumni)
- **Distribution:** May 29 - June 18, 2025 via email, WhatsApp, Teams, and campus QR codes
- **Tool:** Google Forms with 19 structured questions
- **Data:** Usage patterns, satisfaction levels, feature priorities, and improvement suggestions

**2. Semi-Structured Interviews**
- **Participants:** 3 stakeholders (2 current students, 1 alumnus)
- **Platform:** Microsoft Teams (recorded with consent)
- **Duration:** ~4 minutes each
- **Focus:** In-depth experiences, specific pain points, and detailed recommendations

### Data Analysis & User Segmentation

- **Tools Used:** Python (Pandas, NumPy, Matplotlib, Seaborn)
- **Segmentation Criteria:** Usage frequency, satisfaction, task diversity, frustration levels
- **Requirements Derivation:** Functional Requirements (FRs) from user tasks; Non-Functional Requirements (NFRs) from performance/usability feedback

## Key Deliverables

1. **Analysis Script/Notebook:** Python-based data processing and segmentation analysis
2. **Segmentation Report:** Text summary of user segments and requirements (`report/izone_segmentation_analysis_report.txt`)
3. **Data Export:** Excel file with segment characteristics and requirements analysis (`report/izone_segmentation_analysis_report_data.xlsx`)
4. **Visualizations:** Charts and heatmaps showing user patterns and requirements priorities (`media/` folder)
5. **Narrative Analysis:** Jupyter Notebook with integrated findings (`iZone_Analysis_Story.ipynb`)

## Key Findings

- **User Segments Identified:** Power Users, Frustrated Users, Heavy Users, New/Inactive Users
- **Critical Pain Points:** Outdated UI, poor system performance, limited mobile usability
- **High-Priority Features:** Timetable access, academic results, fee payment functionality
- **Strong Demand For:** UI modernization, calendar integration, improved navigation
- **Segment-Specific Needs:** Different user groups require tailored solutions

## Technical Implementation

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn openpyxl scikit-learn
```

### Running the Analysis
1. Ensure `cleaned_izone_survey_data.csv` is in the root directory
2. Execute: `python izone_user_segmentation_analysis.py`
3. Or open and run `iZone_Analysis_Story.ipynb` in Jupyter

## Tools & Technologies

- **Elicitation:** Google Forms, Microsoft Teams
- **Analysis:** Python 3.x, Pandas, NumPy, Matplotlib, Seaborn
- **Documentation:** Jupyter Notebook, Excel
- **Collaboration:** Git/GitHub (version control)

## Project Impact

This requirements engineering process demonstrates:
- Effective multi-method elicitation combining quantitative and qualitative approaches
- Data-driven user segmentation for targeted requirement identification
- Systematic analysis leading to actionable improvement recommendations
- Professional application of requirements engineering tools and methodologies

The findings provide clear direction for iZone enhancement, prioritizing user experience improvements while addressing specific functional needs across different user segments.

---

**Note:** This project simulates real-world requirements engineering practices, emphasizing user-centric analysis and evidence-based recommendations for system improvement.