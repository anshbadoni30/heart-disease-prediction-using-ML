Predicting heart disease using machine learning
1. Problem Definition
  In a statement,
  Given clinical parameters about a patient, can we predict whether or not they have heart disease?

2. Data
  The original data came from the Cleavland data from the UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+Disease
  There is also a version of it available on Kaggle. https://www.kaggle.com/datasets/sumaiyatasmeem/heart-disease-classification-dataset

3. Evaluation
  If we can reach 95% accuracy at predicting whether or not a patient has heart disease during the proof of concept, we'll pursue the project.

4. Features
  This is where you'll get different information about each of the features in your data. You can do this via doing your own research (such as looking at the links     above) or by talking to a subject matter expert (someone who knows about the dataset).

Create data dictionary
  1.age - age in years
  2.sex - (1 = male; 0 = female)
  3.cp - chest pain type
    0: Typical angina: chest pain related decrease blood supply to the heart
    1: Atypical angina: chest pain not related to heart
    2: Non-anginal pain: typically esophageal spasms (non heart related)
    3: Asymptomatic: chest pain not showing signs of disease
  4.trestbps - resting blood pressure (in mm Hg on admission to the hospital) anything above 130-140 is typically cause for concern
  5.chol - serum cholestoral in mg/dl
  6.serum = LDL + HDL + .2 * triglycerides
  7.above 200 is cause for concern
  8.fbs - (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
  '>126' mg/dL signals diabetes
  9.restecg - resting electrocardiographic results
    0: Nothing to note
    1: ST-T Wave abnormality
      can range from mild symptoms to severe problems
      signals non-normal heart beat
    2: Possible or definite left ventricular hypertrophy
        Enlarged heart's main pumping chamber
  10.thalach - maximum heart rate achieved
  11.exang - exercise induced angina (1 = yes; 0 = no)
  12.oldpeak - ST depression induced by exercise relative to rest looks at stress of heart during excercise unhealthy heart will stress more
  13.slope - the slope of the peak exercise ST segment
    0: Upsloping: better heart rate with excercise (uncommon)
    1: Flatsloping: minimal change (typical healthy heart)
    2: Downslopins: signs of unhealthy heart
  14.ca - number of major vessels (0-3) colored by flourosopy
    colored vessel means the doctor can see the blood passing through
    the more blood movement the better (no clots)
  15.thal - thalium stress result
      1,3: normal
      6: fixed defect: used to be defect but ok now
      7: reversable defect: no proper blood movement when excercising
  16.target - have disease or not (1=yes, 0=no) (= the predicted attribute)
