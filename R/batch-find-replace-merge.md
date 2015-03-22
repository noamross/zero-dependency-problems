I have a data processing question that probably has an easy answer, but I can't figure it out. I have a data set on zooplankton that includes species/genus names, and I want to lump them into families or orders. I have a separate data frame of all the species and what orders they are in. I want to make a new column in my original data frame with the larger group that the species falls into. For example:

```
animalsdf = data.frame(length = c(5,4,3,5,6), weight = c(3,4,5,6,9), species = c("rat", "mouse", "lizard", "lizard", "turtle"))

groups = data.frame(species = c("rat","mouse","lizard","turtle"), class = c("mammal", "mammal", "reptile", "reptile"))
```
I feel like I should be able to do something like this

```
llply(animalsdf$species, function(p) {
  llply(groups, function(){sub(groups[,1], groups[,2], p)})
})
```

But that doesn't work

I also tried this

```
animalsdf$class = as.character(animalsdf$species)

for (x in 1:nrow(groups) {
    for (i in 1:nrow(animalsdf)) {
    animalsdf$class[i] = sub(groups[x,1], groups[x,2], animalsdf$class[i])
   }
}
)
```

But that didn't work either.

I can get it to work for one class at a time by doing this:

```
  for (i in 1:nrow(animalsdf)) {
    animalsdf$class[i] = sub(groups[1,1], groups[1,2], animalsdf$class[i])
}
```

I feel like I should be able to figure this out, but after three hours of trying I thought I'd let some fresh eyes look at it.

[Issue](https://github.com/noamross/zero-dependency-problems/issues/4)
