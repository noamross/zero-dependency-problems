I would like to subset rows and columns that meet a certain condition into a new data frame. If the sum of the row or column = 0, then it is not included in the new data frame. Additionally, I would like to subset data based on a criteria looking at the rownames (or I guess it could be just a site name in a column). This seems like a fairly straight forward problem but I am pretty new to R... Any help would be greatly appreciated. I hope the code below makes it clear what I am asking.

My data looks something like the data frame produced below.

```
col1 <- c(1,0,0,2,5,1,0)
col2 <- c(0,0,1,1,1,0,0)
col3 <- c(0,0,0,0,0,0,0)
col4 <- c(0,0,1,1,0,1,0)
rownames(testdataframe) <- c("CA1","CA2","CA3","CA4","LN1","LN2","LN3")
testdataframe <- data.frame(col1, col2, col3, col4)

testdataframe_subset <- testdataframe[-(if sum of row = 0, exclude),-(if sum of column = 0, exclude)]
```
So, `testdataframe_subset` would look like `testdataframe[c(1,3:7),c(1,2,4)]`

```
testdataframe_subset_ca <- testdataframe_subset[(if first two letters in rowname = "CA")]
```

So, `testdataframe_subset_ca` would look like `testdataframe_subset[c(1:3),]`

Perhaps the solution is something like `all[which(condition)]` but I am not sure.
