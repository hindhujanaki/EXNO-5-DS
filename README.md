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
 ### Simple two lines
```python
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[1,4,1]
plt.plot(x1,y1, label="line 1", color="maroon", linewidth=2)

x2=[1,2,3]
y2=[4,1,4]
plt.plot(x2,y2, label="line 2", color="black", linewidth=2)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/b250b845-05c8-463a-9d2b-8aeab4d593d9)


### Customization of plots
```python
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='grey', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='maroon',markersize=10)

plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title("Customization of Plots")
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/8fbf634c-71ec-4314-a935-3db6a2c9857c)


### Implementation using Matplotlib
```python
yield_orange=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_orange, color='sienna', linewidth=3)
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/c2d77575-42a0-4552-811b-da62c0f41184)


```python
years= [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples, color='chocolate', linewidth=3)
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/448cbe47-adb1-41d4-adfb-a183f0dc5c79)


```python
years = range(2000, 2012) 
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896, ] 
 
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)'); 


plt.plot(years, apples)
plt.plot(years, oranges)

plt.xlabel( 'Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/e73b1e4c-c152-4795-97b4-8f8d82233e2d)

```python
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o')
plt.title("vield of Oranges (tons per hectare)") 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/e035a649-15e5-4cb2-9e1f-89a9b14d4fab)


```python
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker="x")
plt.xlabel('Year') 
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend([ 'Apples', 'Oranges']) 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/c9148eb7-1da6-45d6-ad39-b6f1061f0c00)


### Scatter Plot
```python
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter(x_values, y_values,s=30, color="blue") 
plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/bf894ceb-fa26-4d92-9fd8-fdaba27e35c7)


```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/92242267-022c-43d5-a1aa-700684282d20)


![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/58c5f0a2-8fac-4bf5-99e9-eb169922f287)


```python
plt.scatter(x,y,c="r")
plt.xlabel( 'X axis')
plt.ylabel('Y axis')
plt.title( 'Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/61bb7bce-f490-4eba-af4d-bf7a99443d7b)


![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/562016e8-5a0d-41d4-8bda-7534ea71df67)


```python
plt.plot(x,y, 'g*',linestyle='dashed' ,linewidth=2, markersize=12)
plt.xlabel( 'X axis') 
plt.ylabel( 'Y axis')
plt.title('2d Diagram') 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/f5198301-bd64-4c12-8a9b-2b2a510b2e4d)


![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/d1082743-e2e2-4e4c-ab03-4fa0f64c4799)


```python
x = np.arange(0, 4 * np.pi, 0.1) 
y= np.sin(x)
plt.title('sine wave form')
plt.plot(x, y)
plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/d86d5288-6987-4970-a56a-e21907d0b501)


### Area Chart
```python
import matplotlib.pyplot as pit
import numpy as np
x=[1,2,3,4,5]
y1=[10, 12, 14, 16, 18]
y2=[5,7,9, 11, 13]
y3=[2,4,6,8,10]
pit.fill_between(x, y1, color='maroon')
plt.fill_between(x, y2, color='orange') 
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/c2cd51f7-629c-4643-b30a-f5a1b94f8b3b)


### Bar Chart
```python
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one','two"', 'three’', 'four', 'five']

c1 =['chocolate', 'darkgreen']
c2 =['skyblue', 'blue'] 
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x - axis')

plt.ylabel('y - axis')

plt.title('Bar Chart')

plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/c6970d93-aedd-4c02-b47d-8da51b96dccb)


```python
x = [2,8,10]
y = [11,16,9]
x2 = [3,9,11]
y2 = [6,15,7] 
plt.bar(x, y,color='chocolate')
plt.bar(x2, y2, color = 'darkgreen')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/6bd7c1a5-32d1-4b60-b1c3-4e9014535d30)

### Histogram
```python
import matplotlib.pyplot as plt

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins = 10

plt.hist(ages, bins, range, color='darkgreen' , histtype='bar', rwidth=0.8)

plt.xlabel('age') 

plt.ylabel('No. of people')

plt.title('My histogram')

plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/0e96e94a-86cf-42b9-acb2-f96681bd5b0d)


### Box Plot
```python
import matplotlib.pyplot as plt
import numpy as np 

np.random.seed(0) 
data = np.random.normal(loc=0, scale=1, size=100)
data 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/c851ce2a-b33b-4571-8678-323b4a778f86)


```python
fig, ax = plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('Values')
ax.set_title('Box Plot') 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/18204047-ac14-44a2-aef3-743bb6ae6d35)


### Pie Chart
```python
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)

plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show() 
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/5806b38a-5f6b-4146-bd87-d6517c788b62)


```python
activities = ['eat', 'sleep', 'work', 'play']

slices =[3,7,8,6]

colors=['r', 'y', 'g', 'b']

plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1F%%')

plt.legend()
```
![image](https://github.com/hindhujanaki/EXNO-5-DS/assets/148514666/931db4c6-6fdd-4cfc-83f7-a7a24e297b2c)


# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
 
