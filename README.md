### *I've got 99 problems, but dependencies ain't one*

This is a collection of actual problems / questions gleaned programming listservs, Stack Overflow, and workshops. It serves two purposes:

-   **Examples and exercises:**  These serve as raw material from which to create teaching examples and exercises.
-   **Reverse instructional design:** The problems also serve as tools for instructors to develop lessons and teaching methods.  I am currently working on a [lesson](https://github.com/noamross/getting-unstuck-R) on problem-solving approaches and "getting unstuck."  The goal of the lesson is to teach students how to solve problems
like the ones presented here.  Determining the pathways to solving the problem for a beginner will help in developing material for the lesson.

Each problem as an associated [issue](https://github.com/noamross/zero-dependency-problems/issues) to discuss how instructors would demonstrate solving the problem, and how novices (usually those with only a [Software Carpentry](http://software-carpentry.org/) or [Data Carpentry](http://datacarpentry.org/) workshop behind them), would be able to reach the solution.  Some relevant questions to answer for each problem are:

-  What information is required that is NOT in the basic SWC/DC curriculum?
-  Where would one find the answer in the help system, and how would one find it?
-  What google search would yield the answer?
-  What does a minimum reproducible example look like?

These were selected because they are at a relatively basic level - just beyond the material taught in workshops.  They are *zero-dependency* in that they are issues encountered in base R/python/shell, not those having to do with use of specific packages, nor specific data sets. That does not mean that using a package isn't the right *answer* to the question, but discovering the appropriate package is part of the puzzle to solve.

(I note that the vast majority of questions I found in the first round of searching my local R-help listserv were package-specific, though, which might be important in thinking through how to teach problem solving.).

Also in this repo you'll find [an analysis of R errors on Stack Overflow](https://github.com/noamross/zero-dependency-problems/blob/master/misc/stack-overflow-common-r-errors.md), which is a larger-scale exercise in identifying the types of (R) problems that beginners may encounter.

### Contributing

Input welcome!

-   **New Examples**:  Add other real-world examples into the appropriate R/python/shell folder. One way to hunt for examples is to use [Stack Overflow advanced search](http://stackoverflow.com/help/searching) to find "bad" questions.  For instance, here's a 
[search for low-voted, closed questions about R](http://stackoverflow.com/search?q=%5Br%5D+score%3A..0+closed%3Ayes). Questions gathered in person in workshops/classes would be great, too. 
-   **Discussion**:  Please give your feedback on the best way to teach/use any particular problem in its associated issue.

A broader issue is how to classify the problems (by pathway to solution? Type of object/data being handled?).  Thoughts on that welcome [here](https://github.com/noamross/zero-dependency-problems/issues/3).


