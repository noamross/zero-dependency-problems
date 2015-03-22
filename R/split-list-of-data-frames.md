I have what I think is a list of data frames and I want to break the list into its data frames. I am importing a series of files into R using these two lines of code

```
yieldfiles <- paste0("/accessdata/yield", c("corn.csv", "cc.csv","tomato.csv","wheat.csv")) 
yield <- lapply(yieldfiles, read.csv, header=TRUE, sep = ",", stringsAsFactors=FALSE) 
```

When I do this, I get a list of data frames. I use the command

`yield[[1]]`

or

`yield[1]`

to access the first data frame in the list.

What I want to do is split this list up into its component data frames. I think I should use split(), but I'm not sure what the f argument would be. Of course if there is a better way to import the data so I don't have to do this that would also be cool. Thanks!
