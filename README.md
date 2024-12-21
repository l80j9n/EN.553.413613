java c
Applied Stats and Data Analysis 
EN.553.413-613, Fall 2024 
Oct 31st, 2024 
Midterm 2 
Question 1 (22 points). Consider the linear model
Y = Xβ + ε,
where Y is a n-by-1 vector of response variables, X is an n-by-p design matrix, β is a p-by-1 vector of coefficients (we assume n > p), ε is a multivariate normal Nn(0, σ2In). Denote by b the least-squares estimate of β.
(a) TRUE or FALSE. Y ∼ Nn(Xβ, σ2I)
(b) TRUE or FALSE. Cook’s distance measures the influence of one predictor on all fitted values.
(c) TRUE or FALSE. Hβ = b.
(d) TRUE or FALSE. Studentized deleted residuals are the same as Internally Studentized Residuals.
(e) TRUE or FALSE. Polynomial regression is an example of Multiple Linear Regression.
(f) TRUE or FALSE. rank(X) = rank(XTX).
(g) TRUE or FALSE. SSR = ∥Y − Yb∥2.
(h) TRUE or FALSE. Externally studentized residuals are better than internally studentized residuals in determining outliers with respect to Y .
(i) TRUE or FALSE. Variance Inflation Factor helps us determine influential observations.
(j) TRUE or FALSE. Outliers with large leverage are always influential.
(k) TRUE or FALSE. As we add more predictors, the adjusted coefficient of multiple deter-mination Radj2 always increases.
Question 2 (16 points). In this problem we deal with the same multiple linear regression model as in Question 1.
(a) Write the least-squares objective function Q(β) that we need to minimize to fit a multiple linear regression. Write it in terms of Y, X, β.
(b) Take the derivative ∂β/∂Q and equate it to 0. How are these equations called?
(c) From part (b) find the formula for the least-squares estimate for the regression vector b in terms of matrices X, Y. What are conditions needed for the unique solution to exist?
(d) State the distribution of b. Make sure to specify mean and variance. You don’t need to derive anything here.
(e) This part could be solved independently from other parts. Compute the covariance ma-trix Cov(e, Y), where e is a vector of residuals, Y is a vector of observed response vari-ables. Simplify as much as you can. What are the dimensions of the matrix Cov(e, Y)?
Question 3 (16 points). Below is the sketch of a column space Col(X) of an n-by-2 design matrix X. The vector Y is an n-by-1 vector of values Yi, 1 is an n-by-1 vector of 1’s, X1 is an n-by-1 vector of predictor values Xi1. Let b be the least squares estimate of β.
• Vector (iv) is the orthogonal projection of Y onto Col(X).
• Vector (v) is the orthogonal projection of Y onto the vector of 1’s.

(a) Express vectors (i),(ii),(iii) in terms of Y, X, b, Y. Here, Y is an n-by-1 vector of Y ’s.
(b) Express vectors (i),(ii),(iii) in terms of Y, H, I, J, n, where H is the hat matrix, I is an n-by-n identity matrix, J is an n-by-n matrix of 1’s.
(c) Write the coefficient of multiple determination R2in terms of the norms of some or all vectors (i),(ii),(iii),(iv),(v), e.g. ∥(i)∥ is the norm of the vector (i).
(d) (BONUS Q) Prove that SSR = YT(H − n1J)Y. Show your steps.
Question 4 (20 points). Consider the following regression model:
Yi = β0 + β1X1i + β2X2i + εi
where the εi are iid N(0, σ2). We provide the following information:

We use lm in R to fit a linear regression model, obtaining the output below:
Estimate Std. Error t value Pr(>|t|)
(Intercept) 0.8436 0.4591 1.837 0.1256
x1 0.4052 0.1346 3.011 0.0297
x2 0.8340 XXXXXX XXXXX 0.0150
---
Residual standard error: 0.5353 on 5 degrees of freedom
Multiple R-squared: 0.8327,Adjusted R-squared: 0.7657
F-statistic: 12.44 on 2 and 5 DF, p-value: 0.01145
(a) State the null and the alternative hypothesis for the model utility test for this model. What is your conclusion at the significance level α = 0.02? Briefly explain.(b) Is β1 significant at the significance level α = 0.02? Is β2 significant at the significance level α = 0.02? Briefly explain.
(c) Rewrite the hypothesis test H0 : β1 = β2 in the form. of the General Linear Test:
H0 : Cβ = γ, Ha : Cβ ≠ γ.
Identify C and γ and state their dimensions. What is going to be the degrees of freedom for the computed F∗statistic? You do not need to compute any statistic here.
(d) The plot below shows the 98% Confidence Intervals for β1, β2 individually (along the axes) and the joint 98% Confidence Region (the ellipse). Shade, or indicate otherwise, the areas where (0, 0) might lie in this plot consistent with the R output above.
(e) Standard error for the slope β2 is hidden by XXXXX. Recover it using the data provided above.
Question 5 (20 points). Consider a fitness study tracking weekly calorie burn among par-ticipants. Let X1 represent the total distance run in kilometers, X2 the average intensity of workout sessions as a percentage (ranging from 0 to 100), and X3 an indicator variable that is 1 if the participant had a recovery day in that week and 0 otherwise. The outcome variable Y denotes the total weekly calorie burn. We fit the multiple linear regression model:
Yi = β0 + β1Xi1 + β2Xi2 + β3Xi3 + β4Xi1Xi3 + β5Xi2Xi3 + εi
where εi are i.i.d. N(0, σ2). The regression output from fitting this model is shown below:
Coefficients:
Estimate Std. Error t value Pr(>|t|)
(Intercept) 2799.28178 23.47759 119.232 < 2e-16 ***
x1 0.13253 1.51817 0.087 0.930835
x2 -1.00306 0.59743 -1.679 0.100247
x3 120.25577 33.25913 3.616 0.000767 ***
x1:x3 0.34690 2.15538 0.161 0.872873
x2:x3 0.07701 0.84579 0.091 0.927869
---
Residual standard error: 3.225 on 44 degrees of freedom
Multiple R-squared: 0.9979,Adjusted R-squared: 0.9977
F-statistic: 4257 on 5 and 44 DF, p-value: < 2.2e-16
The first 3 rows of the dataset are the following
Y                    X1                   X2                    X3
2746           7                       56                       0
2709           20                   90                       0
2858           13                   73                       1
(a) How many observations are in the full dataset?
(b) Write only the first three rows of the design matrix X for this model. What are the dimensions of the full design matrix X for this model?
(c) Do you notice any issues with this model? If you do, how would you fix the issue?
(d) Write the mean calorie burn for a week that includes a recovery day, expressed in terms of all, or some, X1, X2, and X3.
(e) Should the model above include only X3 based on the results above? Briefly justify.
(f) Should both interaction terms be included? Write the Reduced and Full model, specify how the F∗statistic needs to be computed. Do not compute it. What are the degrees of freedom for that F statistic? Can we make a conclusion about this based on the results shown above? Briefly explain.
Question 6 (16 points). The table below contains leverages hii, residuals ei, internally studentized residuals ri, externally studentized residuals tifor the model with 2 predictors and 8 observations.

Table 1: Values of hii, ei, ri, and ti.
(a) Which points seem to be outliers with respect to X? Briefly justify.
(b) What should be the decision rule to identify observations outlying with respect to Y at the significance level α = 0.10? Write it in the form.|A| ≥ t(B, C) Identify A, B, C. Be as specific as you can.
(c) Below is the Cook’s distance plot for this dataset. Based on this plot, which two ob-servations appear the most influential here? Determine approximately the value of the Cook’s distance for these observations based on the plot below.




         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
