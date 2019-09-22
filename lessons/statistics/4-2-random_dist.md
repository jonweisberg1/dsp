[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```{python}
numbers = np.random.random(1000)
pmf = thinkstats2.Pmf(numbers)
cdf = thinkstats2.Cdf(numbers)

```

```{python}
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Random Number', ylabel='PMF')

```
![pmf](https://github.com/jonweisberg1/dsp/blob/JonWeisberg/images/pmf_random.png 'pmf')
```{python}
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random Number', ylabel='CDF')
```
![cdf](https://github.com/jonweisberg1/dsp/blob/JonWeisberg/images/cdf_random.png 'cdf')
