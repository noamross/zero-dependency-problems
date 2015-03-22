I have one column of numbers (colA) ranging from 1.56 to 1200. I want to create a second column (colB) that incrementally increases as colA incrementally increases. 

As colA increases by 10, colB increases by 2. But this should only happen after values in colA reach 20. Before that colB equals 2. 

So,

1.56 <= colA <=20, then colB == 2

20 < colA<= 30, then colB == 4

30 < colA <= 40, then colB == 6

40 < colA <=50, then colB == 8

…all the way up to 1200 where colB should equal 238 (I believe)
 
Does anyone have any bright ideas as to how to make this happen? Perhaps a creative function using a for loop? Thanks for any thoughts that exist out there!
