#  python code

This was a part of my internship project, we wanted to use the Robust Optimization approach when having missing DATA, since RO is used to seek an optimized solution that is resistant to perturbation in data, let's try it to minimize what could worst happen when having pertubation due to missing values .. So what matters is training the model based on RO logic (and the set of uncertainties is related to the method of imputation which was in our case Hot Deck multiple imputation technique), then the model that we used is an ANN. You could use whatever neural network model (based on the problem you have) just take into consideration that few changes would be necessary for the RO training function (& the other training testing functions of couse ^^).. Later on we would compare the maximum loss when using our RO model and the classical model when testing on both imputed/complete dataset.

PS: often when presenting this work to people, they tend to ask (so did you get to fill in the missing values ..) thinking that we did this to impute missing values our incomplete dataset. NO the purpose is to FIND A MODEL (a robust one) that provides us with a safe solution, since it is feasible for every perturbed dataset and optimal for the worst case dataset (and that's why it's called ROBUST actually ^^). Imputation was just a pass through (an important one of course) to figure the set of uncertainties (all the possible imputed values). AND as **Schafer** said "It’s important to highlight that the purpose of Multiple imputation is not to re-create the individual missing values as close as possible to the true ones, but **to handle missing data to achieve valid statistical inference.

# R code for imputation techniques 
It's a code showing the impact of imputation on the inferece when using different methods, here I'm showing mean imputation, determenistic & stochastic regression imputation. I've published a detailed article about this, you can find it here ==> [Medium profile](https://medium.com/@hadik.imane)




