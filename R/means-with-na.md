Simple data manipulation question:

I have two vectors, say:
```
c(1,3,NA,7,9)
c(3,NA,7,9,11)
```

I'd like to return a vector of same length that is the mean of each respective vector position, and also ignore the NA's (so take the average of one number, not two). I don't want NA's in my answer unless the same position in each vector has an NA.


So, the answer I want is:

```
c(2,3,7,8,10)
```

Anyone have an elegant solution to this problem? 

[Issue](https://github.com/noamross/zero-dependency-problems/issues/13)