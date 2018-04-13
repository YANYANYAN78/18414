# 18414
第几天




输入某年某月某日，判断这一天是这一年的第几天？
1、年份能被4整除；
2、年份若是 100 的整数倍的话需被400整除，否则是平年。

year = int(raw_input('year:\n'))
month = int(raw_input('month:\n'))
day = int(raw_input('day:\n'))
days = [31,28,31,30,31,30,31,31,30,31,30,31]
if year % 400 == 0 or (year % 4 == 0 and year % 100 != 0):
	days[2] += 1

now = sum(days[0:month-1])+day
print （'it is the %dth day.' %now）
