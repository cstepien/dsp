[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
from __future__ import print_function, division
import numpy as np
import thinkstats2
import thinkplot

t = np.random.random(1000)
pmf = thinkstats2.Pmf(t)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='Random variate', ylabel='PMF')

cdf = thinkstats2.Cdf(t)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random variate', ylabel='CDF')
```

![PMF of random variate](4-2_PMF.png)

It's hard to determine the distribution with the PMF because of the large number of values.

![CDF of random variate](4-2_CDF.png)

The CDF is pretty much a straight line, so the distribution is uniform.
