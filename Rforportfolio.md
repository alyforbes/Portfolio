```
#setwd

setwd('/Users/AlyssaForbes/Forbes_PROSIT/Social_Analytics')
```


```
#Separate into the columns

colnames(mydata2)[1] = "column"

df = data.frame(do.call("rbind", strsplit(as.character(mydata2$column), "|", fixed = TRUE)))
```
