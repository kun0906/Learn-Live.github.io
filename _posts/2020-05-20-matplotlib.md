---
title: "matplotlib"
preview: "matplotlib" 
permalink: "/blog/misc/matplotlib" 
layout: post
 
categories: 
    - "pycharm"
    - "matplotlib"
    - "visual"
---

# Pycharm matplotlib in interactive mode
## Solution:
```python3
import matplotlib as mpl
import matplotlib.pyplot as plt
mpl.use('macosx')

plt.plot(range(10))
```
+ or 

```
Disable Settings | Tools | Python Scientific | Show plots in tool window.
```

## Refs:

<!-- comments
<sup>[1]</sup>
1. [1]: https://stackoverflow.com/questions/49844189/how-to-get-interactive-plot-of-pyplot-when-using-pycharm
[inline link](in reference[1])  

[inline link](in reference[1])  
[1] [interactive plot in pycharm](https://stackoverflow.com/questions/49844189/how-to-get-interactive-plot-of-pyplot-when-using-pycharm)
-->

* https://stackoverflow.com/questions/49844189/how-to-get-interactive-plot-of-pyplot-when-using-pycharm

# plt.savefig() should stay before plt.show() 

* [https://stackoverflow.com/questions/21875356/saving-a-figure-after-invoking-pyplot-show-results-in-an-empty-file](https://stackoverflow.com/questions/21875356/saving-a-figure-after-invoking-pyplot-show-results-in-an-empty-file)

# plt.draw() and plt.show() 
* [https://stackoverflow.com/questions/23141452/difference-between-plt-draw-and-plt-show-in-matplotlib#:~:text=show()%20will%20display%20the,the%20graph%20itself%20to%20change.](https://stackoverflow.com/questions/23141452/difference-between-plt-draw-and-plt-show-in-matplotlib#:~:text=show()%20will%20display%20the,the%20graph%20itself%20to%20change.)


# Rotate axis text in python matplotlib and get_xticklabels() contains empty text instances
 
```
# Unfortunately you need to draw your figure first to assign the labels,
# otherwise get_xticklabels() will return empty strings.
plt.draw()
ax.set_xticklabels(ax.get_xticklabels(), rotation=45, ha='right')
```

* [https://stackoverflow.com/questions/32700935/get-xticklabels-contains-empty-text-instances](https://stackoverflow.com/questions/32700935/get-xticklabels-contains-empty-text-instances)





