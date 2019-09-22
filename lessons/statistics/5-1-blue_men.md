[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

The following code yields the answer.

```{python}
mu = 178
sigma = 7.7
min_height = (10+5*12)*2.54
max_height = (1+6*12)*2.54
answer = scipy.stats.norm.cdf(max_height,mu,sigma)-scipy.stats.norm.cdf(min_height,mu,sigma)
print('Percentage of men between 5\'10" and 6\'1" is : ', answer*100)
```
Output:
```
Percentage of men between 5'10" and 6'1" is :  34.27468376314746
```
