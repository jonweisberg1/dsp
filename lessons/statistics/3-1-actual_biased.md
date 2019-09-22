[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```{python}
resp = nsfg.ReadFemResp()
pmf_actual = thinkstats2.Pmf(resp.numkdhh,label='actual')
pmf_biased = BiasPmf(pmf_actual, label='observed')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf_actual, pmf_biased])
thinkplot.Config(xlabel='Number of Children', ylabel='PMF')
```
![pmf]
(/dsp/images/pmf_children.png)
