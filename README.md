# Module-4-
Programming structure in R
> Freq <- c(0.6,0.3,0.4,0.4,0.2,0.6,.3,0.4,0.9,0.2)
> BP <- c(103,87,32,43,59,109,78,205,135,178)
> First <- c(1,1,1,1,0,0,0,0,NA,1)
> Second <- c(0,0,1,1,0,0,1,1,1,1)

> hospital.df <- data.frame(Freq,BP,First,Second,Final)

> #Create a boxplot
> boxplot(Freq,BP,First,Second,Final)  #First attempt at boxplot
 
> #BP and Freq are too large for other values and should be seperated
> boxplot(Freq)
> boxplot(BP)
 
> boxplot(First,Second,Final)
 
> #Create a histogram for each value
> hist(BP)
> hist(First) #Shows the frequency of patients being 'good' (0) or 'bad' (1), leaving out the NA.
> hist(Second) #Lists the frequency of patients as 'low'(0) or 'high'(1)
> hist(Final) #Lists frequency of patients  as 'low' (0) or 'high' (1)
