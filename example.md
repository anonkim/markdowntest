This is a test
==============

==============

R code chunks
=============

Writing R markdown, you can insert R code chunks including plots:
=================================================================

    # quick summary and plot
    library(ggplot2)
    summary(cars)

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

    qplot(speed,dist,data=cars)+
            geom_smooth()

![](example_files/figure-markdown_strict/qplot-1.png)
