
<img src="Kickstarter-logo.jpg" width="200" height="150"/>

# kickstarter-analysis
The dataset is used for various analyses and visualizations, aiming to explore patterns and trends in Kickstarter campaigns. The goal is to understand what makes a Kickstarter project successful or failed.
## Data Handling Summary
1-Drop unnecessary columns which including (url,comments,name) <br>
2-Removed duplicate rows <br>
3-New column were created for the purpose of deeper analysis, such as (in us) These column helped us understand project dynamics and identify key patterns that influence success. However, these columns were not relevant for machine learning model training, where we focus on the original, more fundamental features of the dataset.<br>
4-A small number of rows with missing values in (location,reward levels) were dropped would not significantly impact the dataset or analysis.<br>
## Data Dictionary
| Column Name         | Description                                                       | Data Type    |
|---------------------|-------------------------------------------------------------------|--------------|
| `project_id`        | A unique identifier for each project.                             | Integer      |
| `category`          | The category under which the project was launched (e.g., "Technology", "Art"). | Object       |
| `subcategory`       | A more specific classification within the main `category`                             | Object      |
| `location  `        | The geographic location of the project creator or where the project is based.          | Object      |
| `status`            | The final status of the project (e.g., "successful", "failed").   | Object  |
| `goal`              | The funding goal the project aims to raise in USD.                             | Float      |
| `pledged`           | The total amount of money pledged by backers in USD.              | Float        |
| `funded percentage` | The percentage of the funding goal that the project                             | Float     |
| `backers`           | The total number of backers for the project.                      | Integer      |
| `funded_date`       | The date and time when the project was launched.                  | Object     |
| `levels`            | Different tiers or levels of pledge amounts set by the project creator.                         | Integer     |
| `rewerd levels` | The corresponding rewards or perks that backers receive at each `level` | Object      |
| `updates` | Regular posts or emails to keep backers informed about progress, milestones, or challenges | Integer        |
| `duration`        | The duration of the project campaign in days                           | Float      |
## Quantitative Data Analysis
### Analysis of Kickstarter Project Data
Through the analysis of Kickstarter project data,able to uncover key insights into the factors influencing project success and failure. Below are some important findings:
- **Successful Projects**:
  - Tend to have **higher average pledge amounts**.
  - Attract **more backers** compared to failed projects.
  - The **average pledge** for successful campaigns is noticeably higher, indicating that backers are more committed to these projects.
- **Failed Projects**:
  - Have **lower average pledge amounts** and fewer backers.
  - The **lower pledge amount** suggests that backers are uncertain about the project’s potential or its deliverability.
### Data Limitations
While the analysis offers valuable insights, the dataset has its limitations:
- Missing Key
- Duplicates 
## Qualitative Analysis
### Pledge Goal:
**Recommendation:**  
Set a **realistic pledge goal** that aligns with both your project's needs and your community's expectations. The analysis indicates that projects with pledge goals that are neither too high nor too low tend to have higher chances of success.<br>
**Rationale:**  

- **Too high:** Backers may doubt the feasibility of the project, leading to a lack of trust and backing.
- **Too low:** A low goal can signal a lack of ambition or confidence in the project’s potential, which may discourage serious backers.
---
### Reward Structure:
**Recommendation:**  
Design a **tiered reward system** that encourages higher pledge amounts. Offer **exclusive rewards** for backers at higher pledge levels, such as limited edition items, early access, or special recognition.<br>

**Rationale:**  
Projects with a **compelling reward structure**, offering backers something valuable in return for their contributions, tend to perform better. The rewards should:
- Be aligned with the project’s overall theme.
- Offer backers a sense of participation and ownership in the project, which can increase the likelihood of higher pledges.
---
### Category and Target Audience:
**Recommendation:**  
Focus on **popular categories** such as **technology, design, and games**, which tend to have a more dedicated backer base. Understand your audience and tailor your project messaging and rewards to them.<br>

**Rationale:**  
- These categories often attract a **larger and more committed group of backers**, providing an easier path to success.
- When targeting your audience, make sure the project aligns with their interests and needs.
- Use messaging that resonates with their values and expectations, enhancing engagement and support.

