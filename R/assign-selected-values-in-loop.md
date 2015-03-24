---
source: Local R-help listserv
---

This seems like it should be simple, so I'm not sure why I am having trouble.  

I have a data frame of character strings, like this one, in which all values should say "ab", but some of the b's are missing, so I need to correct those values.  

```
df1 <- data.frame(A=c("ab", "a", "ab"), B=c("a", "ab", "a"))
```

Luckily, I have a list of the row indices where these errors occur in each column of the data frame.  

```
l1 <- list(A=2, B=c(1,3))
```

I tried to write a for-loop to iterate through the columns and paste in the necessary "b" at each of the rows indicated by the list:

```
for(i in c(1:2)) {
  df1$i[l1$i] <- paste0(df1$i[l1$i], "b")
}
```

But my for-loop is returning an error:

Error in `$<-.data.frame`(`*tmp*`, "i", value = character(0)) : 
  replacement has 0 rows, data has 3

What am I doing wrong?
