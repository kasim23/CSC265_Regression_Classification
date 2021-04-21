# CSC265_Regression_Classification
Building Regression and Classification models.

Based on what we covered on the
modules 1, 2 and 3, you will reflect statistical methods by analyzing data and building predictive models
using train and test data sets. The data sets are about college students and their academic performances
and retention status, which include categorical and numerical variables.
Throughout the data analysis, we will consider only two response variables, 1) current GPA of students,
a numerical response variable, call it y1=Term.GPA and 2) Persistence of student for following year,
a binary response variable (0: not persistent on the next term, 1:persistent on the next term), call it
y2=Persistence.NextYear.
• Term.gpa is an aggregated gpa up until the current semester, however, this does not include this current
semester. In the modeling of gpa, include all predictors except ‘persistent“
• The data shows the N.Ws, N.DFs, N.As as the number of courses withdrawn, D or Fs, A’s respectively
in the current semester
• Some rows were made synthetic so may not make sense: in this case, feel free to keep or remove
• It may be poor to find linear association between gpa and other predictors (don’t include persistent
in gpa modeling)
• Scatterplot may mislead since it doesn’t show the density
Briefly, you will fit regression models on y1 and classification models on y2 using the subset of predictors in
the data set. Don’t use all predictors in any model.

A. Touch and Feel the Data - 5 pts
• Import Data Set and Set Up:
Open the data set StudentDataTrain.csv. Be familiar with the data and variables. Start exploring it.
Practice the code at the bottom and do the set-up.
• Do Exploratory Data Analysis:
Start with Exploratory Data Analysis (EDA) before running models. Visually or aggregatedly you can
include the description and summary of the variables (univariate, and some bivariate analyses). If you keep
this part very simple, it is ok.

B. Build Regression Models - 20 pts - each model 5 pts
Build linear regressions as listed below the specific four models to predict y1 with a small set of useful
predictors. Please fit all these by justifying why you do (I expect grounding justifications and technical
terms used), report the performance indicators in a comparative table, MSEtrain, MSEtest, R2
adj,train and
R2
adj,test using train and test data sets. The regression models you will fit:
1. Best OLS SLR
2
2. Best OLS MLR using any best small subset of predictors (using any selection methods)
3. Best MLR Ridge with any best small subset of predictors
4. Best MLR Lasso with any best small subset of predictors
For tuning parameter, justify with statistical methods/computations why you choose.

C. Build Classification Models - 20 pts - each model 5pts
Build four classification models as below. Please fit all these, include performance indicators for train and
test data sets, separately. Include confusion matrix for each. For each train and test data set, report:
accuracy, recall, precision, and f1 in a cooperative table. For LR or LDA, include ROC curve, area and
interpretation. The classification models you will fit:
1. Logistic Regression (LR) with any best small subset of predictors
2. KNN Classification with any best small subset of predictors
3. Linear Discriminant Analysis (LDA) with any best small subset of predictors
4. Quadratic Discriminant Analysis (QDA) with any best small subset of predictors
Justify why you choose specific K in KNN with a grid search or CV methods.

D. Overall Evaluations and Conclusion - 5 pts
Briefly, make critiques of the models fitted and write the conclusion (one sentence for each model, one
sentence for each problem - regression and classificaton problems we have here). Also, just address one
of these: diagnostics, violations, assumptions checks, overall quality evaluations of the models, importance
analyses (which predictors are most important or effects of them on response), outlier analyses. You don’t
need to address all issues. Just show the reflection of our course materials.
