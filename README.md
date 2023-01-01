# Diabetes_ML_Models_LazyNotebook

As we can see all our dataframe variables are numeric expect our target variable (Outcome) which is boolean (0 or 1).
Quantitative Data Types

We have 6 distinct variables (Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, Age)
We have 2 continuous variables (ΒΜΙ, DiabetesPedigreeFunction)
We have 1 boolean target varible (Outcome)
\\\

Diabetes (Outcome)
Diabetes is a disease that occurs when your blood glucose, also called blood sugar, is too high. Blood glucose is your main source of energy and comes from the food you eat. Insulin, a hormone made by the pancreas, helps glucose from food get into your cells to be used for energy. Sometimes your body doesn’t make enough—or any—insulin or doesn’t use insulin well. Glucose then stays in your blood and doesn’t reach your cells.
\\\

Diastolic Blood Pressure

The diastolic is the pressure in the arteries when the heart rests between beats. This is the time when the heart fills with blood and gets oxygen.

Normal: Lower than 80
Stage 1 hypertension: 80-89
Stage 2 hypertension: 90 or more
Hypertensive crisis: 120 or more.
\\\

Triceps skin fold thickness (mm)
Higher TSF thickness was associated with lower all-cause and cardiovascular mortality, independent of BMI and MAMC. Our study revealed that the TSF thickness may be a convenient and credible indicator to predict mortality, especially in those with severe cardiovascular diseases.

the average TSF thickness was 18.7 ± 8.5 mm.

Women average TSF thickness 23.6 ± 7.5 mm ,women have much higher TSF thickness
Men average TSF thickness 14.3 ± 6.8 mm
\\\

insulin is a hormone that regulates the level of sugar (glucose) in the blood and that is produced by the beta cells of the islets of Langerhans in the pancreas. Insulin is secreted when the level of blood glucose rises—as after a meal.
\\\

Body mass index (BMI) is a tool that healthcare providers use to estimate the amount of body fat by using your height and weight measurements. It can help assess risk factors for certain health conditions.
\\\

Diabetes Pedigree Function indicates the function which scores likelihood of diabetes based on family history
\\\

This dataset contains zeros and some invalid values i.e., values that are logically impossible like glucose, insulin, BMI, or blood pressure value of 0. It is possible to either drop and ignore such inconsistent values while cleaning the dataset or replacing them with a more appropriate range of values. Since there are many zeros in columns ‘Skin Thickness’ and ‘Insulin levels’.We will replace the NaN values with the mean so that the size of the dataset stays the same. Also, the ‘replacing by mean value’ approach works well for features ‘BMI’, ‘glucose’ or ‘Blood pressure’.
\\\

Feature Scaling
We will use RobustScaler, removes the median and scales the data according to the quantile range (defaults to IQR: Interquartile Range). The IQR is the range between the 1st quartile (25th quantile) and the 3rd quartile (75th quantile).
\\\


