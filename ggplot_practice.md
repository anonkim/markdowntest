ggplot practice
===============

    library(ggplot2)
    library(datasets)
    head(diamonds,3)

    ##   carat     cut color clarity depth table price    x    y    z
    ## 1  0.23   Ideal     E     SI2  61.5    55   326 3.95 3.98 2.43
    ## 2  0.21 Premium     E     SI1  59.8    61   326 3.89 3.84 2.31
    ## 3  0.23    Good     E     VS1  56.9    65   327 4.05 4.07 2.31

    head(cars,3)

    ##   speed dist
    ## 1     4    2
    ## 2     4   10
    ## 3     7    4

    ## qplot
    qplot(clarity,data=diamonds,fill=cut,geom="bar")

![](ggplot_practice_files/figure-markdown_strict/unnamed-chunk-2-1.png)  

    ## ggplot histogram
    ggplot(diamonds,aes(clarity,fill=cut))+geom_bar()

![](ggplot_practice_files/figure-markdown_strict/unnamed-chunk-2-2.png)  

    qplot(wt,mpg,data=mtcars)

![](ggplot_practice_files/figure-markdown_strict/qplot-1.png)  

    qplot(log(wt),mpg-10,data=mtcars)

![](ggplot_practice_files/figure-markdown_strict/qplot-2.png)  

    qplot(wt,mpg,data=mtcars,color=qsec)

![](ggplot_practice_files/figure-markdown_strict/qplot-3.png)
