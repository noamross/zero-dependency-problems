Does anyone know why using an apply() statement to draw multiple lines on a plot with abline() returns "NULL" in addition to drawing the lines?  I am creating a plot in an R Markdown PDF document, and my document would look nicer if it didn't have "NULL" printed along with the plot.  

Here is an example of the problem:

```
> plot(1)
> x <- cbind(c(0.8, 1.0, 1.2), c(0, 0, 0))
> apply(x, 1, abline)
NULL
```
