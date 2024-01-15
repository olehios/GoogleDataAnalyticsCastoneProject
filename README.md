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
![Visualization Badge](https://drive.google.com/file/d/1XnKnWjwPi8XQrLY7dgMqiW1xzQt74bKS/view?usp=drive_link)

                          
                           
                         
                           
