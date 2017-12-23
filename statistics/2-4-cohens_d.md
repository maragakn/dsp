[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> ```python
>> def Cohen(group1,group2):
>> >> mean1=group1.mean()
>> >> mean2=group2.mean()
>> >> var1=group1.var()
>> >> var2=group2.var()
>> >> pooled_var=(len(group1)*var1+len(group2)*var2)/ (len(group1)+len(group2))
>> >> return((mean1-mean2)/np.sqrt(pooled_var))
>> 
>> firsts = live[live.birthord == 1]
>> others = live[live.birthord != 1]
>> Cohen(firsts.totalwgt_lb,others.totalwgt_lb)
>> Cohen(firsts['prglngth'],others['prglngth'])
>> ```
