I'm trying to do something that I imagine is very simple with the paste function. Specifically, I need to paste several text strings together separated by commas. The catch is that I need each string to be surrounded by quotation marks. For instance,


`"blue" , "red" , "green"`

The function `paste("blue" , "," , "red" "," "green")` results in `"blue , red , green"`. I believe this has to do with escape characters, but I can't figure it out. 
