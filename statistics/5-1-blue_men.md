[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>>  Around 34.2% of the US male population are between 5'10'' and 6'1'' height.
>> 
>> ```python
>> import scipy.stats as st
>> mu   = 178
>> std  = 7.7
>> low  = ((5*12)+10)
>> high = ((6*12)+1)
>> dist = st.norm(loc=mu,scale=std)
>> (dist.cdf(high)-dist.cdf(low)) * 100.0)
>> ```
