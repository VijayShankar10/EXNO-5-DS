# EXNO-5:
DATA VISUALIZATION USING MATPLOT LIBRARY

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
 Include the necessary coding and corresponding screenshots
 import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=np.arange(0,10)
y=np.arange(11,21)
x
y

![image](https://github.com/user-attachments/assets/ad59bb06-8e24-4676-a7f6-f2f019a98b1b)

![image](https://github.com/user-attachments/assets/dd5ef830-c4d0-4381-80c4-e9e67d73150f)

x=np.arange(40,50)
y=np.arange(50,60)
x
y
![image](https://github.com/user-attachments/assets/14e9a9f2-d2dc-4b25-9387-574192d5629f)

![image](https://github.com/user-attachments/assets/20108c59-ab09-4311-a7e6-fc4ae61f012b)

#Scatterplot

plt.scatter(x,y,c='r')

plt.xlabel('X axis')

plt.ylabel('Y axis')

plt.title('Graph in 2D')

plt.savefig('Test.png')

![image](https://github.com/user-attachments/assets/1c58a096-3910-45e5-8087-3fd0d2c01d00)

y=x*x

y

![image](https://github.com/user-attachments/assets/cda00958-1d57-419c-8889-486688498361)

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)

plt.xlabel('X axis')

plt.ylabel('Y axis')

plt.title('2D Diagram')

![image](https://github.com/user-attachments/assets/b2f80edc-6728-443c-9229-efa5880ded26)

plt.subplot(2,2,1)

plt.plot(x,y,'r--')
plt.subplot(2,2,2)

plt.plot(x,y,'g*--')

plt.subplot(2,2,3)

plt.plot(x,y,'bo')

plt.subplot(2,2,4)

plt.plot(x,y,'go')

![image](https://github.com/user-attachments/assets/39dccf92-1f83-45bf-80c9-0187fe84387e)

# Compute the x and y coordinates for points on a

x=np.arange(0,4*np.pi,0.1)

y=np.sin(x)

plt.title("sine wave form")

#Plot the points using matplotlib

plt.plot(x,y)

plt.show()

![image](https://github.com/user-attachments/assets/41038e67-cf29-4519-84e2-a1b5fdfafe43)

#BAR Chart

x=[2,8,10]

y=[11,16,9]

x2=[3,9,11]

y2=[6,15,7]

plt.bar(x,y,color='r')

plt.bar(x2,y2,color='g')

plt.title('Bar graph')

plt.xlabel('X axis')

plt.ylabel('Y axis')

plt.show()

![image](https://github.com/user-attachments/assets/a45d36f3-0ba3-4756-9ce2-7bf15239a1dc)

x=np.arange(1,11)

y=3*x+5

plt.title("Matplotlib demo")

plt.xlabel("x axis caption")

plt.ylabel("y axis caption")

plt.plot(x,y)

plt.show()

![image](https://github.com/user-attachments/assets/a76a8a29-a032-40fc-871c-29fbe4dbd1d4)

x=np.arange(0,5 *np.pi,0.1)

y_sin=np.sin(x)

y_cos=np.cos(x)

plt.subplot(2,1,1)

plt.plot(x,y_sin,'r--')

plt.title('Sine')

plt.subplot(2,1,2)

plt.plot(x,y_cos,'g--')

plt.title('Cosine')

plt.show()

![image](https://github.com/user-attachments/assets/9242a3aa-4797-40c9-b601-c3592760138f)

a=np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27])

plt.hist(a,color='g')

plt.title("histogram")

plt.show()

![image](https://github.com/user-attachments/assets/c282362b-ee0a-4075-8711-e9d50a578063)

labels=['A','B','C']

values=[1,4,2]

plt.figure(figsize=(5,3),dpi=100)

bars=plt.bar(labels,values,color='green')
patterns=['-','*','+']

for bar in bars:

  bar.set_hatch(patterns.pop(0))
  
plt.savefig('barchat.png',dpi=100)

plt.show()

![image](https://github.com/user-attachments/assets/a9120416-6c9c-4790-a91c-4a500be4a346)

import matplotlib.pyplot as plt

x_values = [0,1,2,3,4,5]

y_values = [0,1,4,9,16,25]

plt.plot(x_values,y_values)

plt.show()

![image](https://github.com/user-attachments/assets/6e3114f3-144d-43a6-8d3a-3227f411792f)

import matplotlib.pyplot as plt

x=[1,2,3]

y=[2,4,1]

plt.plot(x,y)

plt.xlabel('x-axis')

plt.ylabel('y-axis')

plt.title('My first graph!')

plt.show()

![image](https://github.com/user-attachments/assets/42903830-2af8-4abb-89f6-2052297d89fa)

import matplotlib.pyplot as plt

x1=[1,2,3]

y1=[2,4,1]

plt.plot(x1,y1,label="line 1")

x2=[1,2,3]

y2=[4,1,3]

plt.plot(x2,y2,label="line2")

plt.xlabel('x-axis')

plt.ylabel('y-axis')

plt.title('Two lines on same graph')

plt.legend()

plt.show()

![image](https://github.com/user-attachments/assets/f069300a-b3ca-4f10-9637-f16ce92e2f48)

import matplotlib.pyplot as plt

x = [1,2,3,4,5,6]

y = [2,4,1,5,2,6]

plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,

         marker='o',markerfacecolor='blue',markersize=12)
         
plt.ylim(1,8)

plt.xlim(1,8)

plt.xlabel('x-axis')

plt.ylabel('y-axis')

plt.title('Some cool customization')

plt.show()

![image](https://github.com/user-attachments/assets/aab2caae-6653-4fd7-a549-6df938ddc6ee)

yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]

plt.plot(yield_apples)

![image](https://github.com/user-attachments/assets/10aa052f-f3a7-4ed2-9331-d486a3a7ea55)

years=[2010,2011,2012,2013,2014,2015]

yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]

plt.plot(years,yield_apples)

![image](https://github.com/user-attachments/assets/8f9b0d87-c3bc-4f99-892d-3f5a19886d1f)

years=range(2000,2012)

apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]

oranges=[0.962,0.941,0.930,0.923,0.918,0.900,0.907,0.904,0.901,0.898,0.9,0.896]

plt.plot(years,apples)

plt.plot(years,oranges)

plt.xlabel("year")

plt.ylabel("Yield(toes per hectare)");

![image](https://github.com/user-attachments/assets/39c289fa-8aec-4080-8bca-10db95df3c5a)

plt.figure(figsize=(12,6))

plt.plot(years,oranges,marker='o')

plt.title("Yield of oranges (toes per hectare)");

![image](https://github.com/user-attachments/assets/238e2e29-93fc-4a81-8ff4-2b4ea474665f)

plt.plot(years,apples,marker='o')

plt.plot(years,oranges,marker='x')

plt.xlabel('Year')

plt.ylabel('Yield (tons per hectare)')

plt.title("Crop Yeilds in Kanto")

plt.legend(['Apples','Oranges'])

![image](https://github.com/user-attachments/assets/57c6579b-69ab-413c-95d7-571eccc20c63)

import matplotlib.pyplot as plt

x_values = [1,2,3,4,5,6,7,8,9,10]

y_values = [2,4,5,7,6,8,9,11,12,12]

plt.scatter(x,y,label="stars",color="blue",marker="*",s=30)

plt.xlabel('x-axis')

plt.ylabel('y-axis')

plt.title("My scatter plot!")

plt.legend()

plt.show()

![image](https://github.com/user-attachments/assets/81f5ae38-5733-4f4b-a366-ba6032b907ce)

AREA CHART

import matplotlib.pyplot as plt

import numpy as np

x=[1,2,3,4,5]

y1=[10,12,14,16,18]

y2=[5,7,9,11,13]

y3=[2,4,6,8,10]

plt.fill_between(x,y1,color="blue")

plt.fill_between(x,y2,color="green")

plt.plot(x,y1,color='red')

plt.plot(x,y2,color='black')

plt.legend(['y1','y2'])

plt.show()

![image](https://github.com/user-attachments/assets/4ae72eac-d831-4ba6-922f-95e4889f3071)


x=[1,2,3,4,5]

y1=[10,12,14,16,18]

y2=[5,7,9,11,13]

y3=[2,4,6,8,10]

plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2','Line3'])

plt.legend(loc='upper left')

plt.title('Stacked Line Chart')

plt.xlabel("X-axis")

plt.ylabel("Y-axis")

plt.show()

![image](https://github.com/user-attachments/assets/f2acfe42-76eb-46ee-a44d-057b33d10975)

SPLINE CHART

import numpy as np

import matplotlib.pyplot as plt

from scipy.interpolate import make_interp_spline

x = np.array([1,2,3,4,5,6,7,8,9,10])

y = np.array([2,4,5,6,7,8,8,10,11,12])

spl=make_interp_spline(x,y)

x_smooth=np.linspace(x.min(),x.max(),100)

y_smooth=spl(x_smooth)

plt.plot(x,y,'o',label='data')

plt.plot(x_smooth,y_smooth,'-',label='spline')

plt.legend()

plt.show()

![image](https://github.com/user-attachments/assets/faac8127-9783-4d11-a49f-34670fef6c4b)

# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
