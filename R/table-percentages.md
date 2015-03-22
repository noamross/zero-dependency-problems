I have some words in my dataframe `df` each belonging to category A or B. Within each category  the words may be of type 1, 2 or 3. I used the `table()` function to show how the words are distributed across the categories and types. The output looks like:
  
             category
    type     A    B
    1        30  79
    2        12  94
    3        29  6 

As you can see the table counts frequencies, but I want it to calculate the percentages instead. I have tried `prop.table` but I get the following error 

>Error in FUN(X[[1L]], ...) : only defined on a data frame with all numeric variables


I couldn't find a solution anywhere else; please help. Thank you.

Here's my sample data:

    head(items)

           item   type category
    [1]    PA100   1    A
    [2]    PB101   2    A
    [3]    UR360   2    A
    [4]    PX977   3    B
    [5]    GA008   3    B
    [6]    GR446   3    A
    
[Issue](https://github.com/noamross/zero-dependency-problems/issues/18)
