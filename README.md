# 18414
第几天




输入某年某月某日，判断这一天是这一年的第几天？
1、年份能被4整除；
2、年份若是 100 的整数倍的话需被400整除，否则是平年。





year=int(input('year:'))
month=int(input('month:'))
day=int(input('day:'))
d=[31,28,31,30,31,30,31,31,30,31,30,31]
if (year%4==0 and year%100!=0) or year%400==0:
    d[1]+=1
    
num=sum(d[:month-1])+day   #注意list的用中括号
print ('the day id the %dth day of the year' % num)
