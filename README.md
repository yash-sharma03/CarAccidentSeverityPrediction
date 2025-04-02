# CarAccidentSeverityPrediction

This project explores patterns in U.S. car accident data from 2016 to 2023, with the goal of understanding what factors contribute to more severe crashes. The dataset included over 7 million records across 49 states, covering variables like weather, time, location, and visibility.

	•	U.S. Accident Data (49 states, 45 features)
	•	Sourced from state DOTs, traffic sensors, cameras, and law enforcement data
	•	Target variable: Severity (1 = minor, 4 = major)

  Preprocessing


  
	•	Dropped columns with high missingness, applied imputation (median/“unknown”)
	•	Converted datatypes (boolean, datetime)
	•	Feature engineered time-based features (hour, day of week)
	•	Binarized severity variable
	•	Scaled numerical features, encoded categorical features (OneHotEncoder)
	•	Used SMOTE to balance the training data

  Models Used

  
	•	Logistic Regression
	•	Random Forest
	•	XGBoost
	•	Support Vector Machine (SVM)
	•	Neural Network

 Evaluation & Results

 
	•	Best Recall: Logistic Regression
	•	Best Accuracy: XGBoost
	•	Important features: Wind Direction, Weather Condition, State
	•	Evaluation focused on Recall, prioritizing correct identification of severe accidents.

 Business Use Cases

 
	•	Insurance: Rate risk by area
	•	Government: Safer traffic regulations and infrastructure planning
	•	Self-driving car companies: Improve decision-making models
	•	Emergency services: Smarter response allocation
	•	Rideshare & Maps: Smarter real-time rerouting

 Key Insights

 
	•	Accidents are most common in major urban centers due to congestion and infrastructure stress
	•	Morning rush hour is a peak accident time
	•	Fewer accidents in midwestern/northern regions due to lower traffic volume
	•	Logistic Regression and Neural Networks offer strong performance for prediction tasks
