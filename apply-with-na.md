I have a data frame (tadlengths) with five columns of tadpole lengths for a bunch of different treatments. I want to average the five lengths. I did this by:

```
meanlength = apply(tadlengths, 1, mean)
```
However, sometimes I only had four lengths, so there are NAs in those rows. I want to average the four lengths on those rows, but the code above gives me "NA" for those rows. I feel like there is a very, very, easy solution for this, but I can't figure it out!

