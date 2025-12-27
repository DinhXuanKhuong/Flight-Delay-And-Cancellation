# 5. Project summary

- **Le Minh Duc (Data Ingestion & Cleaning):**
  -  **Difficulties:** The primary difficulty was handling raw data inconsistencies, specifically identifying realistic outliers versus data errors during the "Outlier Detection" phase[cite: 11].  Additionally, ensuring zero null values remained required careful imputation strategies for specific columns
  -  **Learned:** I learned rigorous data cleaning standards using Python 3.11 and the importance of maintaining a read-only raw data directory to prevent corruption[cite: 29, 30].
- **Dinh Xuan Khuong (EDA & Visualization):**
  -  **Difficulties:** As the Project Lead, balancing the consensus-based decision-making process with the technical workload of generating distribution plots and correlation heatmaps was challenging[cite: 11, 24].  Finding the right visualizations to effectively show "Delay causes vs. Airlines" required multiple iterations
  -  **Learned:** I learned how to identify key trends through Univariate and Multivariate analysis and gained experience in project management and conflict resolution using GitHub Issues
- **Phan Trung Nhut (Modeling & Evaluation):**
  -  **Difficulties:** Achieving the strict acceptance criteria of 75% Accuracy and F1 Score > 0.7 was difficult using Random Forest and XGBoost.  Feature Selection and One-hot encoding also presented computational challenges due to the dataset size
  -  **Learned:** I mastered the end-to-end modeling pipeline, from feature engineering to calculating AUC and F1 metrics, and learned to manage dependencies between EDA deliverables and model training
- **Our group:**
  -  **If you had more time:** We would expand the "Ask question" phase to include more complex customer-benefit questions.  We would also refine our coding standards to include stricter code reviews with comprehensive end-to-end notebook runs

## Keys findings:


## Limitations:

-  **Dataset limitations:** The dataset contained null values that required imputation
-  **Analysis limitations:** The scope was limited to Random Forest and XGBoost algorithms; we did not explore Deep Learning approaches due to the sprint timeline
-  **Scope limitations:** The project timeline was compressed into two sprints (Dec 1 - Dec 18), limiting our ability to iterate extensively on feature selection

## Future Directions (If You Had More Time)

-  **What additional questions would you explore?** We would ask more questions related to the direct benefit for customers, ensuring each member contributes at least 2 additional meaningful inquiries
-  **What deeper analysis would you conduct?** We would perform a more granular "Feature Importance" check to refine the model further and potentially reduce dimensionality
-  **What alternative methods or approaches would you try?** We would experiment with different model architectures beyond tree-based methods to see if we can exceed the 75% accuracy baseline
-  **How could this work be expanded or improved?** We could automate the data pipeline further, ensuring that the "Data Ingestion" and "Cleaning" phases are fully integrated with the modeling scripts for real-time predictions

## Individual Reflections

### Phan Trung Nhut
 **Role:** Feature Engineering, Modeling & Evaluation 

**Challenges & Difficulties Encountered:**
-  **Specific Obstacles:** My main technical obstacle was tuning the Random Forest/XGBoost hyperparameters to ensure the model met the specific metric goals (Accuracy 75%, F1 > 0.7)
-  **How did you overcome them?** I focused heavily on "Feature Selection & Encoding" to ensure only the most relevant data points were used for training
-  **What was most challenging and why?** Meeting the December 18th deadline for the final model was pressure-filled, as my work depended entirely on the completion of the EDA and Cleaning phases

**Learning & Growth:**
-  **What have you learned?** I learned deep technical skills in model evaluation (AUC, F1) and how to interpret feature importance for real-world datasets
-  **How has this project shaped your understanding of data science?** It highlighted the critical link between "Feature Engineering" and final model performance—raw algorithms are not enough without good data preparation

### Le Minh Duc
 **Role:** Data Ingestion, Cleaning & Preprocessing 

**Challenges & Difficulties Encountered:**
-  **Specific Obstacles:** Formatting date/time columns correctly and ensuring no null values remained for the modeling team was a tedious but critical task
-  **How did you overcome them?** I utilized the `min_ds-env` Conda environment and standard Python libraries to automate the cleaning process
-  **What was most challenging and why?** The dependency chain—knowing that the "Outlier Detection" and cleaning had to be finished by Dec 7 so the rest of the team could start their work

**Learning & Growth:**
-  **What have you learned?** I learned how to maintain a clean schema and the importance of version control (Pull Requests) when managing shared data scripts
-  **How has this project shaped your understanding of data science?** I realized that data cleaning consumes a significant portion of the project timeline (Sprint 1) and is the foundation for all subsequent insights

### Dinh Xuan Khuong
 **Role:** Exploratory Data Analysis (EDA) & Visualization (Project Lead) 

**Challenges & Difficulties Encountered:**
-  **Specific Obstacles:** As the Lead, I had to ensure consensus on decisions while also delivering complex visualizations like distribution plots
-  **How did you overcome them?** I organized weekly 60-minute meetings to align the team and used "Acceptance Criteria" to define clear goals for my visualization tasks
-  **What was most challenging and why?** Identifying "5+ actionable insights" from the data required not just coding skills, but deep analytical thinking

**Learning & Growth:**
-  **What have you learned?** I learned to use tools like `black` for code styling and GitHub Issues for tracking tasks, which improved my workflow efficiency
-  **How has this project shaped your understanding of data science?** It taught me that EDA is not just about making charts, but about finding the "story" within the data to guide the modeling phase