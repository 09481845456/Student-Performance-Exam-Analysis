# Student-Performance-Exam-Analysis
### Project Description: Analyzing Student Performance Using Machine Learning

#### Objective:
The primary objective of this project is to analyze student performance in exams using machine learning techniques. The aim is to build a classification model that can predict whether a student will perform well based on various features such as gender, race/ethnicity, parental level of education, lunch type, and test preparation course completion. By leveraging machine learning, we can gain insights into the factors that influence student performance and identify areas where students may need additional support.

#### Dataset:
The dataset used for this project contains information about students' demographics and their scores in math, reading, and writing exams. The dataset includes the following columns:
- **gender**: Gender of the student (male/female)
- **race/ethnicity**: Race/ethnicity group of the student (group A, B, C, D, E)
- **parental level of education**: Highest level of education completed by the student's parents
- **lunch**: Type of lunch received (standard/free or reduced)
- **test preparation course**: Completion status of the test preparation course (none/completed)
- **math score**: Score in math exam
- **reading score**: Score in reading exam
- **writing score**: Score in writing exam

#### Methodology:
1. **Data Loading and Preprocessing**: 
   - Load the dataset into a Pandas DataFrame.
   - Encode categorical variables using Label Encoding.
   - Handle any missing values (if any).

2. **Feature Engineering**:
   - Calculate the average score across math, reading, and writing exams.
   - Create a binary label indicating whether a student's average score is above or below a threshold (e.g., 70).

3. **Exploratory Data Analysis (EDA)**:
   - Generate descriptive statistics for the scores.
   - Visualize the distribution of scores using box plots.
   - Analyze the difficulty level of each subject by calculating the percentage of students scoring below a certain threshold.
   - Assess the correlation between different scores using a heatmap.

4. **Model Building**:
   - Define features (X) and labels (y) for the classification model.
   - Split the data into training and testing sets.
   - Train a RandomForestClassifier to predict student performance.
   - Evaluate the model using accuracy score and classification report.

5. **Visualization and Interpretation**:
   - Use various visualizations to understand the dataset and model results:
     - Box plots to visualize the distribution of exam scores.
     - Bar charts to display difficulty levels.
     - Heatmap to show correlations between scores.
     - Pie chart for gender distribution.
     - Bar charts to compare average scores by gender, parental education level, and test preparation course.
     - Scatter plot to examine the relationship between reading and writing scores.

6. **Conclusion**:
   - Summarize the findings from the analysis.
   - Discuss the model's performance and potential improvements.
   - Provide insights and recommendations based on the analysis.

#### Visualizations Used:
1. **Box Plot**:
   - **Usage**: To visualize the distribution of math, reading, and writing scores.
   - **Insights**: Shows the spread, median, and potential outliers in the scores.

2. **Bar Chart**:
   - **Usage**: To display the difficulty level (percentage of students scoring below 70).
   - **Insights**: Identifies subjects where students are struggling the most.

3. **Heatmap**:
   - **Usage**: To visualize the correlation matrix of exam scores.
   - **Insights**: Highlights the relationships between different scores and the overall average score.

4. **Pie Chart**:
   - **Usage**: To show the distribution of students by gender.
   - **Insights**: Provides a visual representation of gender distribution in the dataset.

5. **Bar Chart (by Gender, Parental Education, and Test Preparation)**:
   - **Usage**: To compare average scores across different categories.
   - **Insights**: Reveals how factors like gender, parental education, and test preparation impact student performance.

6. **Scatter Plot**:
   - **Usage**: To examine the relationship between reading and writing scores.
   - **Insights**: Shows the correlation between two continuous variables and highlights patterns based on gender.


### Explanation of Visualizations:
1. **Box Plot of Exam Scores**:
   - **Description**: This plot displays the distribution of math, reading, and writing scores.
   - **Insight**: The plot reveals that the math scores have a broader range compared to reading and writing scores. The median scores for reading and writing are similar, while the math scores show a wider variability.

2. **Bar Chart for Difficulty Level**:
   - **Description**: This chart shows the percentage of students scoring below 70 in each subject.
   - **Insight**: The chart indicates that a higher percentage of students struggle with math compared to reading and writing. This suggests that math is the most challenging subject for the students in this dataset.

3. **Heatmap for Correlation Matrix**:
   - **Description**: This heatmap visualizes the correlation between different exam scores and the average score.
   - **Insight**: The heatmap highlights that all three scores (math, reading, and writing) are positively correlated with each other and the overall average score. The strongest correlation is between reading and writing scores.

4. **Pie Chart for Gender Distribution**:
   - **Description**: This pie chart shows the proportion of male and female students in the dataset.
   - **Insight**: The chart reveals the gender distribution,
