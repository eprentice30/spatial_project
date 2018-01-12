# survival_project
Comparing effects on survival time of different treatments for Carcinoma 

The main question we wanted to answer was if there was a difference in survival times for two different treatments (radiation therapy, and radiation with chemotherapy). We started off by getting an estimate for each covariate's affect on the survival function with the Kaplan-Meier estimate. We saw that treatment was insignificant, while t\_stage, n\_stage, and the condition were significant. This gave us a reasonable hypothesis of what would be significant when we did a multivariate model.

The two types of models we considered were the Cox Proportional Hazards model and the Accelerated Failure Time model. We were able to verify the assumption that the hazards are proportional (through the Logrank test), therefore the Cox model was satisfactory. Through stepwise selection, the final covariates in our model were the treatment, n\_stage, and t\_stage. We had to leave the type of treatment in the model because it was our main focus, even though it was insignificant through the entire process.  When we ran a stepwise regression model in SAS we found that treatment was left out of the final model do to it's insignificance.

Therefore it is reasonable that there is not a significant difference between the two treatments.
