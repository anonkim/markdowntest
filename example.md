R code chunks
=============

Writing R markdown, you can insert R code chunks including plots:

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
 Table

    fit<-lm(speed~dist,data=cars)
    summary(fit)$coef

    ##              Estimate Std. Error  t value     Pr(>|t|)
    ## (Intercept) 8.2839056 0.87438449 9.473985 1.440974e-12
    ## dist        0.1655676 0.01749448 9.463990 1.489836e-12

this is a table manually constructed
------------------------------------

<table>
<thead>
<tr class="header">
<th align="right">alpha</th>
<th align="left">beta</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="right">11</td>
<td align="left">aa</td>
</tr>
<tr class="even">
<td align="right">22</td>
<td align="left">bb</td>
</tr>
<tr class="odd">
<td align="right">33</td>
<td align="left">cc</td>
</tr>
</tbody>
</table>
