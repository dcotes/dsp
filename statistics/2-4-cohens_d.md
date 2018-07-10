[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

import nsfg
import math

preg = nsfg.ReadFemPreg()
live = preg[preg.outcome == 1]
firsts = live[live.birthord ==1]
others = live[live.birthord != 1]

mean_difference = firsts.totalwgt_lb.mean() - others.totalwgt_lb.mean()

var_firsts = firsts.totalwgt_lb.var()
var_others = others.totalwgt_lb.var()
var_both = (len(firsts) * var_firsts + len(others) * var_others) / (len(firsts) + len(others))

mean_difference / math.sqrt(var_both)