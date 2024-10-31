# JAMB 2024 Performance Prediction Project

## Overview
This project applies machine learning to predict student performance in the 2024 Joint Admissions and Matriculation Board (JAMB) exams, examining a variety of factors, including student demographics, family background, socioeconomic status, study habits, and school-related variables. By building and evaluating predictive models, this study seeks to support educators and policymakers in making data-driven decisions to enhance educational outcomes, bridge performance gaps, and better identify students who may benefit from additional support.

## Problem Statement
The significant variance in JAMB performance across student demographics and backgrounds raises questions about the underlying influences on student outcomes. With admission into higher education depending on these scores, understanding these influences is crucial. This project aims to uncover how factors such as parental education, socioeconomic status, school type, and teacher quality impact JAMB scores, providing insights that can guide effective educational policies and student support systems.

## Aim of the Study
The primary goals of this analysis are to:
- Examine the relationships between various personal, familial, and academic factors and student performance in JAMB.
- Build and evaluate predictive models to forecast JAMB scores based on these factors.
- Provide actionable recommendations for educators and policymakers to improve student outcomes.

## Tools and Technologies
- **Python**: The primary language for data analysis and machine learning.
- **MySQL**: For managing and querying large datasets.
- **Pandas, Seaborn, Matplotlib**: Used for data cleaning, manipulation, and visualization.
- **Power Bi**: Used for Data Visualization
- **Scikit-Learn**: Provided foundational machine learning models.
- **XGBoost**: An advanced machine learning model used to improve prediction accuracy.

## Models Utilized
Several machine learning models were used in this project:
- **Linear Regression**: Assesses the linear relationships between features and JAMB scores.
- **Decision Tree Regressor**: Captures non-linear relationships through tree-based decisions.
- **Random Forest Regressor**: An ensemble model that averages multiple decision trees for better accuracy.
- **XGBoost Regressor**: Optimizes predictions through boosting, iteratively improving model performance.

## Model Evaluation Metrics
To evaluate each model’s predictive power, the following metrics were used:
- **R² (Coefficient of Determination)**: Measures how well the model explains variance in JAMB scores.
- **Mean Absolute Error (MAE)**: Represents the average difference between actual and predicted scores.
- **Mean Absolute Percentage Error (MAPE)**: Provides a percentage-based error measure for interpretability.

## Results and Model Comparison
| Model                   | R²    | MAE | MAPE |
|-------------------------|-------|-----|------|
| Linear Regression       | 0.262 | 33  | 20%  |
| Random Forest Regressor | 0.217 | 34  | 21%  |
| XGBoost Regressor      | 0.119 | 36  | 22%  |
| Decision Tree Regressor | 0.087 | 35  | 22%  |

The **Linear Regression model** performed the best, explaining approximately 26.2% of the variance in JAMB scores. Its relatively low MAE and MAPE indicate a strong predictive capability, making it suitable for understanding linear relationships within the data. While Random Forest showed comparable accuracy, XGBoost and Decision Tree models were less effective, suggesting limited applicability for more complex relationships in this dataset.

## Analysis and Insights
1. **Parental Education Level and Study Hours per Week**
   - **Findings**: Students with parents educated to tertiary levels scored highest, with an average of 184 and 20 study hours per week. Students with unknown parental education levels scored lowest, averaging 158 despite similar study hours.
   - **Insight**: Parental education level positively correlates with student performance, likely reflecting parents’ academic influence and support capacity.

2. **Parental Involvement and Gender**
   - **Findings**: Higher parental involvement led to better performance for both genders. For example, females with highly involved parents scored 185 on average, while those with low involvement scored 161.
   - **Insight**: Parental engagement is critical, suggesting it could help mitigate other performance disparities.

3. **Socioeconomic Status (SES)**
   - **Findings**: High-SES students scored an average of 190, compared to 160 for low-SES students.
   - **Insight**: Economic background has a strong impact on academic outcomes, highlighting the need for additional support for students from low-SES backgrounds.

4. **School Location**
   - **Findings**: Students in urban schools scored slightly higher (170) than those in rural areas (169).
   - **Insight**: Urban schools typically have more resources, which may explain this difference, though it remains small. Improved rural education resources could help reduce such disparities.

5. **Access to Learning Materials and Gender**
   - **Findings**: Access to study materials significantly affected scores, with both genders scoring 172 when resources were available.
   - **Insight**: Educational resources are crucial, suggesting that making learning materials widely accessible could have substantial benefits.

6. **School Type and IT Knowledge**
   - **Findings**: Students with high IT knowledge scored notably higher, especially in private schools (192). Public school students with high IT knowledge scored lower (183).
   - **Insight**: IT skills are increasingly essential, with private schools offering better training in this area. Improving IT support in public schools could bridge this gap.

## Recommendations
1. **Invest in Teacher Quality**: Training and development programs for teachers can improve the quality of instruction, directly benefiting student outcomes. Schools should prioritize workshops and skill-building sessions for educators.

2. **Encourage Consistent Study Habits**: Schools and families should promote structured study schedules to help students maintain consistent academic routines.

3. **Track and Encourage Assignment Completion**: Regular monitoring of assignment completion and engaging students in coursework positively correlates with performance. Teachers and administrators should support students in staying on top of their work.

4. **Address Proximity Challenges**: For students facing long commutes, schools could explore options for transportation assistance or study hubs closer to students' homes.

5. **Expand Access to Learning Materials**: Making learning materials readily accessible to all students, regardless of gender or location, would improve academic performance across the board.

6. **Enhance IT Education in Public Schools**: Public schools should receive more support in IT education, potentially through partnerships with technology firms, to provide students with critical digital skills.

## Conclusion
The analysis highlights several significant influences on JAMB performance, including parental education, socioeconomic status, access to resources, and school characteristics. By understanding and addressing these factors, educational stakeholders can create a more equitable environment that supports every student’s academic journey. Implementing these recommendations could improve national exam outcomes like JAMB and foster a fairer, more supportive education system. Through data-driven strategies and targeted interventions, this project contributes valuable insights toward the goal of elevating educational success for all students.
