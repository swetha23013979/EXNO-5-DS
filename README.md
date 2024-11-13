# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
# REG NO: 212223040222
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
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")

x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')

plt.legend()
```
![image](https://github.com/user-attachments/assets/9681fba8-5943-4ff9-a68f-82f543a9b00d)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('some cool!')
```
![image](https://github.com/user-attachments/assets/7f870fb2-eb08-4556-8710-35ff96caeb7b)

```
import matplotlib.pyplot as plt
x_values=[1,2,3,4,5]
y_values=[1,5,10,16,20]
plt.scatter(x_values,y_values,s=20,color="purple")
plt.show()
```
![image](https://github.com/user-attachments/assets/88680014-907d-4934-8e62-43bd07dc77f7)

```
x=[1,2,3,4,5,6,7,8,10]
y=[0,2,3,5,10,11,12,13,15]
plt.scatter(x,y,s=20,color="black",label="stars",marker="*")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My scatter plot!')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/8e046c22-20ca-4648-ba58-ea3d5e5c9515)

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='yellow')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/db290b74-b427-4f61-9d9b-6ae4cba2b799)

```
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]

plt.barh(names,values,color="yellowgreen")
plt.show()
```
![image](https://github.com/user-attachments/assets/d6ebb65a-3280-4f38-8a8d-ca25f48488ea)

```
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,color=c1,width=0.8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar plot!')
plt.show()
```
![image](https://github.com/user-attachments/assets/f5c0b413-f3b0-45c3-8dc0-d90b556cc140)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/25b1c777-6be8-4e32-b921-74f87602f758)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No.of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/21eca369-0e5a-4280-a8ac-4cecb19b5e4f)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/78f59ed8-48b4-408d-b8d4-dbc01a202353)

```
import matplotlib.pyplot as plt
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/c939f18b-307d-40f1-9a46-84f5886d8b28)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box plot')
```
![image](https://github.com/user-attachments/assets/fac893fe-5417-46bb-8098-2b5bdb1add19)

```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
c=['r','y','g','b']

plt.pie(slices,labels=activities,colors=c,startangle=90,shadow=True,explode=(0,0.1,0,0),autopct='%1.1f%%')
plt.show()
```
![image](https://github.com/user-attachments/assets/4ab7e759-4f69-4555-bb76-f638554c1507)

```
#Data to plot
labels ='Python', 'C++', 'Ruby', 'Java'
sizes =[215, 138, 245, 210]
colors= ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)
#Plot
plt.pie(sizes, explode=explode, labels =labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/5189738b-9b12-442f-843b-3f909a98334d)



# Result:
 Thus, the program Data Visualization using matplot python library for the given datas is been implemented.
