# python-10-
python学习笔记(10)
# p35 pass语句
#pass语句什么都不做，只是一个占位符，用在语法需要语句的地方
#先搭建语法结构，还没想好代码怎么写的时候使用
answer=input('请输入您是会员吗?y/n')
#判断是否为会员
if answer=='y':
    pass
else:
    pass
#目的是让语法不报错

age=int(input('请输入您的年龄'))
if age:
    print(age)
else:
    print('年龄为:',age)
#这也是布尔值的作用，可以直接放在条件表达式中去使用



# p36 range函数的使用
#range的三种创建方式
‘’‘1.只有一个参数(小括号中只给了1个数)’‘’
r=range(10) #0,1,2,3,4,5,6,7,8,9。默认从0开始，默认相差1的步长
print(r) #range(0,10)
print(list(r)) #用于查看range对象中的整数序列

‘’‘2.给了两个参数(小括号中给了两个数)’‘’
r=range(1,10) #指定起始值，从1开始，到10结束(不包含10),默认步长为1
print(list(r)) #[1,2,3,4,5,6,7,8,9]

‘’‘3.给了三个参数’‘’
r=range(1,10,2)
print(list(r)) #[1,3,5,7,9]

'''判断指定的整数 在序列中是否存在in,not in'''
print(10 in r) #False, 10不在当前的r这个整数序列中
print(9 in r) #True

print(10 not in r) #True
print(9 not in r) #False

print(range(1,20,1)) #[1...19]
print(range(1,101,1)) #[1...100]
#注：range不论范围有多长，只有用到才会计算具体的内存空间，不用的时候都是一个内存空间大小



# p37 while循环
a=1
#判断条件表达式
while a<10:
  #执行条件执行体
  print(a)
  a+=1

#计算0到14之间的累加和
a=0
sum=0
while a<5:
sum+=a
a+=1
print('和为',sum)
