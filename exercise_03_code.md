#  case 1
```
from scipy.integrate import odeint
import numpy as N
import matplotlib.pyplot as plt
def f(y,t):
    return 10*y-3*y #定义常微分方程组的形式
y0=100 #规定初始人数
a=0 #规定起始年份
b=3#规定终止的年份
t=N.arange(a,b,0.00001)#规定计算的步长
y=odeint(f,y0,t)    #使用obeint函数求解微分方程
plt.plot(t,y,'b')   #将结果的numpy数组绘制为曲线
plt.xlabel('time year') #x轴名称
plt.title('Increasing population') #y轴名称
plt.ylim([0,200]) #y轴的显示范围
plt.show #绘制曲线图
```

# case 2
```
from scipy.integrate import odeint
import numpy as N
import matplotlib.pyplot as plt
def f(y,t):
    return 10*y-0.01*y #定义常微分方程组的形式
y0=10000 #规定初始人数
a=0 #规定起始年份
b=3#规定终止的年份
t=N.arange(a,b,0.00001)#规定计算的步长
y=odeint(f,y0,t)    #使用obeint函数求解微分方程
plt.plot(t,y,'b')   #将结果的numpy数组绘制为曲线
plt.xlabel('time year') #x轴名称
plt.title('Increasing population') #y轴名称
plt.ylim([0,20000]) #y轴的显示范围
plt.show #绘制曲线图
