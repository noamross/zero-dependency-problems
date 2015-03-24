---
source: Student homework question
---

I'm having some trouble applying things to a subset of the dataframe I'm using.

    > Diet121 <- subset(ChickWeight, Diet == 1 & Time == 21)

This works fine, and gives the subset I want, but when I try to apply the mean to the columns, I get an error message

    > apply(Diet121, 2, mean)
    weight Time Chick Diet
    NA NA NA NA
    Warning messages:
    1: In mean.default(newX[, i], ...) :
    argument is not numeric or logical: returning NA
    2: In mean.default(newX[, i], ...) :
    argument is not numeric or logical: returning NA
    3: In mean.default(newX[, i], ...) :
    argument is not numeric or logical: returning NA
    4: In mean.default(newX[, i], ...) :
    argument is not numeric or logical: returning NA

I'm assuming I'm doing something stupid such as not attaching something correctly. Is something wrong with 'mean'?
