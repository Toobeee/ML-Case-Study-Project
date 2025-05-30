# ML-Case-Study-Project
Global Tech University Admissions Optimizer
Global Tech University Admissions Optimizer

Backdrop & Urgency
Global Tech University (GTU) is a mid‑sized, research‑heavy institution that relies on international student tuition to fund new labs. 
 For the first time, applications have crossed 16 000—double pre‑pandemic volume—yet faculty reviewers are capped at 10 hours / week. Deans fear they will miss top talent or over‑award scarce scholarships.
Provost’s Monday email to the Data Science Center:
“We need a decision‑support tool that flags high‑probability admits by January 31st and projects how many merit scholarships we can promise without blowing the budget.”

Stakeholders & Conflicting Objectives
Stakeholder
What they care about
Pain point
Admissions Dean
Quick short‑list; budget forecast
Manual reviews lag 4 weeks
Scholarship Office
Notifying winners early
Over‑commit risk
EECS Department Chair
Diversifying research talent
GRE‑centric past decisions
International Office
Visa lead‑time
Late admit letters hurt F‑1 issuance



Data Story
Source: Five admission cycles (2019‑2023) exported from Slate CRM.
 Variables provided in the CSV mirror the public dataset:
Academic signals: GRE, TOEFL, CGPA


Subjective ratings: SOP quality, LOR strength


Institutional prestige: University rating (1–5)


Research indicator: 0 / 1 binary



Business Questions Driving Each Algorithm
Phase
Framing question
Regression Algorithm taught
Why it fits
Baseline
“On average, how do 10 GRE points or 0.1 CGPA move admit odds?”
Multiple Linear Regression
Coefficients ↔ policy levers; easy to explain to Deans.
What‑if rules
“If CGPA is high, can low TOEFL still succeed?”
Decision Tree
Transparent pathways; mirrors human reviewer logic.
Robust ranking
“Give us the most accurate top‑200 list under noisy data.”
Random Forest
Handles nonlinearities, lowers variance vs. single tree.





Final Scene
On demo day, teams project their model. The Admissions Dean tests a hypothetical applicant:
GRE 322, TOEFL 111, CGPA 8.9, University rating 3, strong research.
Tree visualization lights up a green leaf: 74 % admit chance.
 Students must defend the prediction path, interpret feature contributions, and answer: “Would you award a scholarship?”



Deliverables for Submission: 
As discussed in class, we will now be taking final submissions for your regression case study project. The goal is to ensure that you have a polished case study that you can confidently showcase in your portfolio and GitHub profile.
Please make sure that, in addition to the steps we covered during the sessions, your final submission also includes the following enhancements:
Random Forest Regressor Tuning
 Apply hyperparameter tuning (e.g., n_estimators, max_depth, min_samples_split, etc.) to improve the performance of your random forest model. You may use GridSearchCV or RandomizedSearchCV( justify your choice).


Decision Tree Regressor Optimization
 Tune your decision tree model using hyperparameters to increase accuracy and reduce overfitting.


Feature Selection-Based Modeling
 Use the feature importance scores from the random forest model to identify the top five features, and retrain your models using only these features. Compare the results.


Handling Multicollinearity in Linear Regression
 Detect and address multicollinearity in your multiple linear regression model (using tools like VIF or correlation matrices) to improve model reliability.



Once you’ve incorporated these points, please submit a final version of your work in the form of a GitHub repository, complete with:
A clear README.md file explaining your approach, results, and insights


Well-commented code and organized notebooks/scripts


Visualizations, if applicable

