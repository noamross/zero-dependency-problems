I would like to add a title to each of the resulting dataframes and then after applying rbind, have a column in the resulting combined file that identifies each so I can compare values. 

This is what the code looks like right now. I need the next steps. 

```
f <- c("NoChange_MINU", "T5only_MINU", "P2Only_MINU","t2p5_MINU")
s <- stack(f)
names(s) <- gsub('_MINU', '', f)
rcl <- matrix(c(0,0.2,1, 0.2, 0.4,2,.4,.6,3,.6,.8,4,.8,1,5), ncol=3, byrow=T)
r <- reclassify(s, rcl)
rl = list()
for (i in 1:nlayers(r)) { rl[[i]] = zonal(a, r[[i]], 'sum') }
rl
```

[Issue](https://github.com/noamross/zero-dependency-problems/issues/9)