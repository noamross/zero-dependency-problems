---
source: Student homework question
---

I tried plotting for the first question and got:

    > subset(ChickWeight, Chick == 1)
      weight Time Chick Diet
    1 42 0 1 1
    2 51 2 1 1
    3 59 4 1 1
    4 64 6 1 1
    5 76 8 1 1
    6 93 10 1 1
    7 106 12 1 1
    8 125 14 1 1
    9 149 16 1 1
    10 171 18 1 1
    11 199 20 1 1
    12 205 21 1 1

    > plot( log_weight, log_Time, main="Scatter plot of weight vs Time", xlab="log Time", ylab="log weight" )

    Error in plot(log_weight, log_Time, main = "Scatter plot of weight vs Time", :
    object 'log_weight' not found

what am I doing wrong here?
