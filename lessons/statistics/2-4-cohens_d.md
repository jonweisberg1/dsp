[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)


```{python}
firsts = live[live.birthord == 1]
others = live[live.birthord != 1]

first_weight = firsts.totalwgt_lb
others_weight = others.totalwgt_lb
first_weight.mean(),others_weight.mean(),first_weight.mean()-others_weight.mean()

```

The above code yields the result:
```
(7.201094430437772, 7.325855614973262, -0.12476118453549034)
```
This shows a very close mean weight for both first time births and non-first time births. We use the Cohen's D statistic to measure how many pooled standard deviations theses means are away from each other.

```{python}
Cohen_D_for_weights = CohenEffectSize(first_weight,others_weight)
Cohen_D_for_weights
```
Which yields:
```
-0.088672927072602
```

It is negative because the first mean is less than the second mean for the data being compared. The difference in means for the pregnancy lengths of these two groups and the Cohen's D for that question is (respectively:
```
(0.07803726677754952, 0.028879044654449883)
```
Comparing these statistics indicates that there is a larger difference in the average weights for first vs. non-first borns than there is for weeks of pregnancy. 
