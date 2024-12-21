java c
Applied Stats and Data Analysis 
EN.553.413-613, Fall 2024 
Oct 3rd, 2024 
Exam 1 
Question 2 (20 pts). The following TRUE/FALSE questions concern the Simple Linear Regression model
Yi = β0 + β1Xi + εi, E(εi) = 0, V ar(εi) = σ2, cov(εi, εj ) = 0, for i ≠ j.
(a) TRUE or FALSE. Yi and εj are uncorrelated for i ≠ j.
(b) TRUE or FALSE. Denote b0 as the least squares estimator for β0 and βˆ0 as some unbiased estimator for β0. The variance of b0 is smaller or equal than the variance of βˆ0.
(c) TRUE or FALSE. If the least squares estimator for β1 is 0, X and Y are not linearly related.
(d) TRUE or FALSE. Semi-studentized residual vs Xi plot can be used to find outliers.
(e) TRUE or FALSE. P ni=1 εi = 0.
(f) TRUE or FALSE. Variance stabilizing transform. can be used to transform. X.
(g) TRUE or FALSE. P ni=1 Yˆi(Yi − Yˆi) = 0.
(h) TRUE or FALSE. Using Working-Hotelling procedure to find joint confidence interval for mean response at Xh1 = 3 with three other points will give the same confidence interval for EYh1 comparing to joint confidence interval for mean response at Xh1 = 3 with ten other points.
(i) TRUE or FALSE. In the Correlation model of regression predictor Xi’s and the response variable Yi are both normal random variables.
(j) TRUE or FALSE. Var(ei) = σ2for all i.
Question 3 (15 pts). Let X1, X2, X3 ∼ iid N(0, 1), i.e. they are independent, identically distributed standard normal random variables. Let Y ∼ N(2, 1) and Y is independent on X1, X2, X3. For the following random variables state whether they follow a normal distribution, a t- distribution, a χ2 distribution, an F distribution, or none of the above. State relevant parameters (e.g. degrees of freedom, and means and variances for normal RVs)

Question 4 (20 pts). Suppose a data set {(Xi, Yi) : 1 ≤ i ≤ n} is fit to a linear model of the form.
Yi = β0 + β1xi + εi
where εi are independent, mean zero, and normal with common variance σ2. Here we treat Y as the response variable and X as the predictor variable. The output of the lm function is given. Some values are hidden by ‘XXXXX’. We provide you with additional value: X¯ = 1.11.
Coefficients:
Estimate Std. Error t value Pr(>|t|)
(Intercept) 0.9088 0.4791 1.897 0.0724
x 1.7480 0.7385 XXXXX 0.0281
---
Residual standard error: 1.088 on 20 degrees of freedom
Multiple R-squared: XXXXXX,Adjusted R-squared: XXXXXX
F-statistic: 5.602 on XX and XX DF, p-value: XXXXXX
(a) How many data points are there (what is n, the sample size)? What is the estimated mean of the response variable Y at Xh = 1 for this dataset?
(b) Based on all of this output, do you reject H0 : β1 = 0 in favour of Ha : β1 = 0 at level α = 0.01 significance? Why? What does the test tell us about the relationship between X and Y ?
(c) Based on all of this output, do you reject the H0 : β1 = 0 vs Ha : β1 > 0 at level α = 0.01 significance? Briefly explain why, or why not.
(d) The degrees of fr代 写EN.553.413-613, Fall 2024 Applied Stats and Data Analysis Exam 1Statistics
代做程序编程语言eedom, and the p-value of the F statistic are hidden. Is it possible to reconstruct all of them based on the data shown? Recover as many values as you can.
(e) Find MSE and Sxx =Pni=1(Xi − X¯)2 based on the data above
(f) Is it possible to find the coefficient of simple determination from the data shown? If yes, do it. If not, briefly explain why.
Question 5 (15 pts). Consider the following diagnostic plots for Model 1 and Model 2. Two simple linear regression models Y = β0 + β1X + ε are fitted to the two different datasets (X, Y ). For each model 3 diagnostic plots are shown: plot of Yi vs Xi, plot of semi-studentized residuals e*i versus fitted values Yˆi, QQ-plot of the semi-studentized residuals e*i.

(a) What is the main issue do you diagnose with the Model 1, if any? Why? Which plot was the most useful in diagnosing this problem? Be as specific in describing the issue as you can.
(b) What is the main issue do you diagnose with the Model 2, if any? Why? Which plot was the most useful in diagnosing this problem? Be as specific in describing the issue as you can.
(c) This question is unrelated to the above plots. Assume that you conclude that in the model the errors are not normally distributed. How does this affect your inference on b1? Briefly justify.
Question 6 (30 points). For the dataset of n = 100 observations a simple linear regression model Yi = β0 + β1Xi + εiis fit. The following estimates are obtained.

Above, ni, ki are some functions of Xi. We have listed additional information here

(a) Find niin terms of Xi. Show your work. You may use the least-squares solution formulas for b0, b1.
(b) Prove Var  Hint: You may use the fact that 
(c) What is the estimated variance s2 of the error term based on the data above?
(d) Find a 99% confidence interval for β0. Write it in the form. A ± B · t(C, D), compute values of A, B, C, D if possible.
(e) Find the joint confidence intervals with confidence at least 99% for β0, β1 in the form. Ai±Bi·t(Ci, Di). Compute values of Ai, Bi, Ci, Diif possible. Without any computation how does the interval for β0 for this part compare to the one in part (d)?
(f) This question is unrelated to the data above. Derive the expression for cov(b0, b1) in terms of some, or all, Xi, Yi, β0, β1, σ2. Simplify as much as you can.
Question 7 (15 points). Suppose we are given n data points {(X1, Y1, Z1),(X2, Y2, Z2), . . . ,(Xn, Yn, Zn)}. We are interested in fitting the linear regression model
Yi = α + βXi + εi and Zi = γ + βXi + ηi
for i = 1, 2, . . . , n, where εi and ηi are independent random variables N(0, σ2). Note that the slope β in both equations is the same.
(a) Derive the least squares estimates of α, β and γ.
Hint: Write a single least squares objective function as a function of α, β, γ and proceed, i.e.
Q(α, β, γ) = . . .
(b) What do you think should be an estimator for σ2for this model?





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
