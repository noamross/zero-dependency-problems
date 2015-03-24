---
source: Local R-help listserv
---

I'm trying to write a for-loop that finds the high tide in a vector of 10-minute tide recordings.  When it finds the high tide, I'd like it to spit that value into a new vector.  I generated some simple sample data (attached) that simulates the dataset with integers.  So far, I have:


```
d <- read.csv("numbers.csv", header=T)

m=0

for (i in 1:length(d$numbers)) {

if(d$numbers[i]>=m) {d$numbers[i] -> m} 

else {m=m}

}
```

[Issue](https://github.com/noamross/zero-dependency-problems/issues/10)