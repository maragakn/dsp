[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> ```python
>> import numpy as np
>> import pandas as pd
>> import matplotlib.pyplot as plt
>> from collections import Counter as cnt
>> %matplotlib inline
>> 
>> def gen_CDF(input_list):
>>   cdf={}
>>   input_list.sort()
>>   for x in input_list: 
>>     c=0
>>     for y in input_list:
>>         if x >= y:
>>             c+=1
>>     cdf[x]=c/len(input_list)
>> return(cdf)
>> 
>> def gen_PMF(input_list):
>>  pmf={}
>>  list_cnt=cnt(input_list)
>>  for x in list_cnt:
>>      pmf[x]=x/len(input_list)
>>  return(pmf)
>> 
>> inp_arr=np.random.random(1000)
>> cdf=gen_CDF(inp_arr)
>> pmf=gen_PMF(inp_arr)
>> plt.plot(pmf.keys(),pmf.values() , drawstyle='steps', linestyle='-', alpha=0.5,c='r')
>> plt.plot(cdf.keys(),cdf.values() , drawstyle='steps', linestyle='-', alpha=0.5,c='b')
>> ```
[[img/commit_file.png]]
![edit](img/edit_file.png)
