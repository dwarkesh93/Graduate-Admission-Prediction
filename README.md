# Graduate-Admission-Prediction
The Graduate Admission Likelihood provides prediction of Graduate Admissions from a student profile perspective. This dataset was built with the purpose of helping students in shortlisting universities with their profiles. The intent is to generate a predicted output that gives them a fair idea about their chances for a particular university.

Using linear regression, it is observed that out of the 7 predictor variables that are associated to the response- Admission Likelihood state, 4 predictors’ coefficients, GRE, TOEFL, LOR, and CGPA are statistically significant
In model selection approach (using 5-fold cross-validated BIC), the model is defined as-
AdmitProb ~ GRE.Score + TOEFL.Score + LOR + CGPA
The table below summarizes how the in-sample model evaluation metrics establish the superiority of the final model over the basic full model.

Model	MSE	R-squared	Adj R-squared	AIC	BIC
Full Model Lm(Admit.Prob~.)	0.0042	0.7941	0.7894	-823	-789
Final Model
Lm(Admit.Prob~ GRE+ TOEFL+ LOR+ CGPA)	0.0037	0.808	0.806	-865	-842

Table 1: Model Performance Evaluation
It is also observed that the CART model does not generate commensurate results when compared with multiple linear regression models.


