---
layout: post
# nav_order: 3
title: Sigmoid
permalink: /blog/sigmoid
parent: Blog
---

Let's plot a sigmoid function. 
{: .fs-7 }


TODO: Implement using tensorflow.
{: .fs-6 }


```python
import numpy as np
from matplotlib import pyplot as plt
```
{: .fs-5 }

```python
x = np.arange(-6,6,.5)
x
```




    array([-6. , -5.5, -5. , -4.5, -4. , -3.5, -3. , -2.5, -2. , -1.5, -1. ,
           -0.5,  0. ,  0.5,  1. ,  1.5,  2. ,  2.5,  3. ,  3.5,  4. ,  4.5,
            5. ,  5.5])




```python
y = (1/(1+np.exp(-x)))
y
```




    array([0.00247262, 0.00407014, 0.00669285, 0.01098694, 0.01798621,
           0.02931223, 0.04742587, 0.07585818, 0.11920292, 0.18242552,
           0.26894142, 0.37754067, 0.5       , 0.62245933, 0.73105858,
           0.81757448, 0.88079708, 0.92414182, 0.95257413, 0.97068777,
           0.98201379, 0.98901306, 0.99330715, 0.99592986])




```python
plt.plot(x,y)
plt.show()
```


    
![image](/img/blog/np_sigmoid_4_0.png)
    


Packages: numpy
