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
NAME: SRIRAM.S

REG.NO: 212225240155
```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
<img width="714" height="533" alt="image" src="https://github.com/user-attachments/assets/649bee81-f813-46b2-b21d-d425443337b5" />

```
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/dc473831-dc8b-4bf1-b744-e699d1e0eb7c" />

```
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
plt.show()
```
<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/ad855f41-65c7-4374-8d1f-f184ad530e8b" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue') # Added closing quote and a color 'blue'
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations')
plt.show()
```
<img width="558" height="453" alt="image" src="https://github.com/user-attachments/assets/e4d62da1-2c80-4187-8e20-5f06693532b8" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
<img width="764" height="568" alt="image" src="https://github.com/user-attachments/assets/3da1aa6e-c2d4-42ca-bb02-3262e8e020d1" />

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9375,0.895] 
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.895] 
plt.plot(years , apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)');
```
<img width="576" height="432" alt="image" src="https://github.com/user-attachments/assets/9304ab75-9d42-4319-abe2-32a72d9d8b92" />

```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
plt.title("Crop yield in Kanto")
plt.legend(['Apples','Oranges'])
```
<img width="766" height="610" alt="image" src="https://github.com/user-attachments/assets/6cdb89a8-0cf2-4b75-a8b5-8265ad5dfeb4" />

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)');
```
<img width="585" height="432" alt="image" src="https://github.com/user-attachments/assets/5be290f7-03fc-473f-984b-ebd82608dc75" />

```
plt.figure(figsize=(12,6))
years=range(2000,2012)
plt.plot(years,oranges,marker='o')
plt.title("Yield of oranges (tons per hectare)");
```
<img width="990" height="526" alt="image" src="https://github.com/user-attachments/assets/88e721d8-6bc7-449c-bd9e-0091fba2dec0" />

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in kanto")
plt.legend(['Apples','Oranges'])
```
<img width="760" height="605" alt="image" src="https://github.com/user-attachments/assets/b60c9045-9037-4597-b38d-ac60b2c45819" />

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="red")
plt.show()
```
<img width="543" height="413" alt="image" src="https://github.com/user-attachments/assets/4c127358-8335-46d6-a35c-a3874375584f" />

```
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
<img width="690" height="572" alt="image" src="https://github.com/user-attachments/assets/2e914408-24cb-417d-b43c-68694cadbd8b" />

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
<img width="724" height="603" alt="image" src="https://github.com/user-attachments/assets/7bed8cd0-4096-4998-a4bf-bb19be634eb9" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="709" height="569" alt="image" src="https://github.com/user-attachments/assets/7976a356-bac8-445e-be6b-c7c98390fe43" />

```
import numpy as np
np.pi
```
<img width="182" height="39" alt="image" src="https://github.com/user-attachments/assets/ec0d339e-4e1d-4ed7-92e5-d2983a72d84b" />

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
<img width="568" height="433" alt="image" src="https://github.com/user-attachments/assets/3bd22ed6-f937-4aab-a783-69b047355ef7" />

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="556" height="413" alt="image" src="https://github.com/user-attachments/assets/cc029e61-9bc2-40fb-b6c6-388c509645f2" />

```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='Spline')
plt.legend()
plt.show()
```
<img width="543" height="413" alt="image" src="https://github.com/user-attachments/assets/8f55ba8b-e5e9-46b2-be41-06d71a7550df" />

```
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color="green")
plt.show()
```
<img width="534" height="413" alt="image" src="https://github.com/user-attachments/assets/d8be1fbc-8ac5-4b4d-a52f-41099fb1e431" />

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
<img width="563" height="453" alt="image" src="https://github.com/user-attachments/assets/0e60648b-fd7c-4555-9e78-350ed8a70f13" />

```
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
<img width="534" height="413" alt="image" src="https://github.com/user-attachments/assets/1eec3d0a-6050-418a-949a-023d836b52d6" />

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
