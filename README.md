# NAME:KISHORE G
# REGISTER NO: 212223040099

# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=[2018,2019,2020,2021,2022]
y=[15000,20000,25000,30000,35000]
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```
<img width="746" height="475" alt="image" src="https://github.com/user-attachments/assets/eb1072a4-af64-42fc-8c51-5ec0198f5bd7" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```

<img width="937" height="445" alt="image" src="https://github.com/user-attachments/assets/24288908-008a-4d74-b2a9-319c78b05146" />


```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```

<img width="699" height="428" alt="image" src="https://github.com/user-attachments/assets/465e0599-43f9-4e04-bbe6-5f152f62178d" />

```
x=[2,8,10]
y=[11,16,9]
x1=[3,9,11]
y1=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x1,y1,color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="788" height="446" alt="image" src="https://github.com/user-attachments/assets/6c6b342c-f474-4667-87b6-44377324b656" />

```
x=[1,2,3]
y=[7,3,9]

plt.plot(x,y,color='g')
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="698" height="437" alt="image" src="https://github.com/user-attachments/assets/ae50b3e8-ccb8-4f0d-8d68-1dc8f503baca" />

```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.title("multiline graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="923" height="486" alt="image" src="https://github.com/user-attachments/assets/c5a3dd94-95f6-4a79-b57a-a29933d460ab" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='red',markersize=12,label='spices')
plt.ylim(1,8)
plt.xlim(1,8)
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="760" height="454" alt="image" src="https://github.com/user-attachments/assets/b07c1c08-1fa4-4a43-94d1-10a7bdce1f0b" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples,linestyle='dashed',linewidth=3,marker='*',markersize=12,color='g')
plt.show()
```
<img width="750" height="417" alt="image" src="https://github.com/user-attachments/assets/d3311af6-0edf-4ad3-a58d-bca814a7bf0d" />

```
oranges=[2,4,6,7,8,12,45]
apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022,2023,2024,2025]
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='*')
plt.title("crop yields in kanto")
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
plt.legend(['apples','oranges'])
plt.show()
```

<img width="563" height="453" alt="Untitled" src="https://github.com/user-attachments/assets/0ce6137e-ceb0-4147-a241-334503c42133" />

```
oranges=[2,4,6,7,8,12]
apples=[2,4,5,6,8,23]
years=[2019,2020,2021,2022,2023,2024]
plt.bar(oranges,apples)
plt.plot(years,apples,label='apples',marker='*')
plt.plot(years,oranges,label='oranges',marker='o')
plt.title("Fruit sales")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="826" height="488" alt="image" src="https://github.com/user-attachments/assets/e55708f8-4260-463a-81fc-23e02256480b" />

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o',label='oranges')
plt.title("Yield of oranges(tons per hectare)")
plt.legend()
```

<img width="1071" height="552" alt="image" src="https://github.com/user-attachments/assets/652f58d6-dfa1-4337-b716-f2dc43e86a4c" />

```
print("scatter plot is:")
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,6,7,8,9,11,12,12]
plt.scatter(x,y,label='star',color='green',marker='*',s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="767" height="488" alt="image" src="https://github.com/user-attachments/assets/3cc5a287-6aef-4453-8be7-db229be2d243" />

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='green',label='y1')
plt.fill_between(x,y2,color='blue',label='y2')
plt.fill_between(x,y3,color='red',label='y3')
plt.title("fill between is")
plt.legend()
plt.show()
```
<img width="752" height="432" alt="image" src="https://github.com/user-attachments/assets/9ffb1a89-0103-4160-bfdb-ebe06609d044" />


```
plt.stackplot(x,y1,y2,y3, labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="850" height="456" alt="497083265-3433126c-a7c5-48ea-8fb0-d792332f173d" src="https://github.com/user-attachments/assets/761b067f-4082-4e86-97cf-c645342db1bb" />

```
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,9,10,11,12,13])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='spline')
plt.legend()
plt.show()
```
<img width="723" height="423" alt="image" src="https://github.com/user-attachments/assets/2e1b124b-4dcd-45d1-861f-dc442d5de20d" />

```
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```
<img width="595" height="406" alt="image" src="https://github.com/user-attachments/assets/1a119785-18e3-4a45-80c4-1c56d0b44465" />

```
ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range1=(0,100)
bins=10
plt.hist(ages,bins,range1,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no of people')
plt.title('my histogram')
plt.show()
```
<img width="774" height="472" alt="image" src="https://github.com/user-attachments/assets/b0b75f3b-1b3a-43a6-a099-40a84eeafcbb" />

```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='green',alpha=0.5)
plt.show()
```
<img width="724" height="404" alt="image" src="https://github.com/user-attachments/assets/b4f93fdb-a014-49bc-9fd2-68f59dc2ca67" />

```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
<img width="968" height="359" alt="image" src="https://github.com/user-attachments/assets/14072f23-c5bc-47b8-ac84-e0bdaf04f250" />

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box_plot')
```
<img width="855" height="495" alt="image" src="https://github.com/user-attachments/assets/0332dd3d-615e-4371-a713-1566fb60d59e" />

```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct="X1.1")
plt.legend()
plt.show()
```
<img width="720" height="441" alt="image" src="https://github.com/user-attachments/assets/e92aea43-7c46-4b8c-b420-b9c28ec0f4b6" />

```
labels='python','C+','ruby','java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,colors=colors,labels=labels, autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

<img width="627" height="364" alt="image" src="https://github.com/user-attachments/assets/f33442a6-723c-4351-92d3-997ce14aa4f0" />

# Result:
 Thus all the data visualization technique of matplotlib has been implemented
 
