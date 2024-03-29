# Project title: 
  Building Machine Learning Model for solving employee retention problem.

# Project Overview:
  In this project, I used Python for model building and data analysis. I tested and trained different models to analyze a dataset and generate business insights for my stakeholders. In particular, I evaluated a logistic regression model and the following machine learning models: decision tree, random forest, XGBoost. I also updated my stakeholders through an executive summary where I presented my findings and came up with some possible solutions and propositions regardng the problem.

# Business Understanding:
  As a part of my 'Advanced Data Analytics Certificate' program I needed to complete a project in which I am a data professional working for company called 'Salifort Motors'. 
  Currently, there is a high rate of turnover among Salifort employees. Salifort’s senior leadership team is concerned about how many employees are leaving the company. Salifort strives to create a corporate culture that supports employee success and professional development. Further, the high turnover rate is costly in the financial sense. Salifort makes a big investment in recruiting, training, and upskilling its employees. If Salifort could predict whether an employee will leave the company, and discover the reasons behind their departure, they could better understand the problem and develop a solution.  
  As a first step, the leadership team asks Human Resources to survey a sample of employees to learn more about what might be driving turnover.  
Next, the leadership team asks me to analyze the survey data and come up with ideas for how to increase employee retention. To help with this, they suggest I design a model that predicts whether an employee will leave the company based on their job title, department, number of projects, average monthly hours, and any other relevant data points. A good model will help the company increase retention and job satisfaction for current employees, and save money and time training new employees. 

# Data Understanding:
This project uses a dataset called HR_capstone_dataset.csv. It represents 10 columns of self-reported information from employees of a multinational vehicle manufacturing corporation. 
The dataset contains:
14,999 rows – each row is a different employee’s self-reported information and 10 columns such as satisfaction_level, last_evaluation, number_project, average_monthly_hours, time_spend_company, work_accident, left, promotion_last_5years, department, salary.
First, I checked and then renamed some columns. Work_accident':'work_accident', 'Department':'department','time_spend_company':'tenure',  'average_montly_hours':'average_monthly_hours'.
Then, I checked for missing values and duplicates. I also created a boxplot to check for outliers in 'tenure' column:


![TenureOutliers](https://i.imgur.com/XWrSauG.png)

                          
I also created a number of visualisations to see the relationships between variables.
1. Monthly hours by number of projects(left vs. stayed) and number of projects (left vs. stayed)

   ![MonHoursBoxplot and NumberOfProjects histogram](https://i.imgur.com/Jtutu6U.png)


It seemed that most employees were overworked. I used boolean mask and value_counts function to see how many people of those who had 7 projects left. 145 people who had 7 projects left.

After that I made a number of other visualisations such as 'Average monthly hours vs. Promotion scatterplot', 'Monthly Hours vs. Last Evaluation scatterplot' etc.
In the end I created a correlation heatmap.

![Correlation Heatmap](https://i.imgur.com/FhCsa30.png)


My insights included following:
1. Most employees work more than average monthly hours.
2. People that worked the most hours and had the most projects left.
3. Also, people that worked below average hours and had low satisfaction levels also left(most probably were fired)
4. A lot of people who tenured for 4,5,6 years and had low satisfaction levels also left.
5. Some people who worked for a long time for company still have low level of salary and were not promoted. Among them are a lot of those who left.
                           
# Modeling and Evaluation:
Several models such as binomial logistic regression model, tree based model, and random forest model. As a result of comparison and evaluation of the performance the random forest model waas chosen.
The plot below showed that in this random forest model, 'last_evaluation', 'number_project', 'tenure', and 'overworked' have the highest importance, in that order. These variables are most helpful in predicting the outcome variable 'left'.  


![RF_Feature_Importance](https://i.imgur.com/wL5fPqJ.png)



The model's precisin score was	0.869903,recall score was	0.899598,	accuracy equaled to	0.960974, f1 to	0.884501, AUC was 0.936399.
All in all, it was stable well - performing final model.

# Conclusion:
1. Number of projects that employees work on can be decreased.
2. Promoting employees who have been with the company for at least four years can be helpful, or further research about why four-year tenured employees are so dissatisfied can be done.
3. Overtime must be rewarded or not required.
4. Employees should be aware of the company's overtime pay policies, therefore it is advisable to inform them about it. 
5. Company meetings acroos all personak should be conducted in order to discuss company work policy.
6. Employees should not be evaluated high only on the basis of having more working hours or more projects. Other features and characteristics should be evaluated, praised and rewarded as well.



