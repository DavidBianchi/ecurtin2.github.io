---
layout: post
title: Testing what happens with two posts
---

Maybe something more complex this time:

{% highlight python linenos=table %}
#Number of randomly generated pairs
import numpy as np
import matplotlib.pyplot as plt
N_array = [10**2, 10**4, 10**6, 10**8]
pi_estimate = []

for N in N_array:
    x, y = np.random.rand(2, N)
    x_squared = np.square(x)
    y_squared = np.square(y)
    #Determine the number of times x**2 + y**2 < 1 and divide by N
    accept = len(np.where(x_squared + y_squared < 1.0)[0]) / float(N)
    pi_estimate.append( 4.0 * accept )
{% endhighlight %}

Whoa that was kinda neat!

Does youtube embedding work? align
<iframe align="middle" width="560" height="315" src="https://www.youtube.com/embed/2ovhbT-Iulc" frameborder="0" allowfullscreen></iframe>
