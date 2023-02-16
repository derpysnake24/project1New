## Locally Weighted Regression

Locally weighted regression, or lowess, is the concept that when a dataset does not fit a linear regression, such as with a since wave, you can take each observation and apply a linear regression to it and and it's neighbors, going through each observation until the trend line for the data is made up of multiple linear regressions, rather than a sine wave or a normal linear regression. 

The first step of the process is to assign distances between all the points. This will help determine the cutoffs for where the data is split into to sepeate linear regressions. Each observation becomes a matrix with the number of rows/columns equal to the number of observations, with each vector representing the distance between each other observation.

The next step is to pick a kernel for the locally weighted regression. Given my current level of understanding, a kernel determines how the locally wieghted regression actually determines the correltions. Each kernel function will make a slightly different output.

$$\sqrt2$$

Here is a diagram representing the process:
<figure>
<center>
<img src='https://drive.google.com/uc?id=1rWcjflTXOfPsuKa71dr_ruqgqklfcSO_' 
width='500px' />
<figcaption></figcaption></center>
</figure>

The oval is the area of points around which the linear relationship is calculated, and the kernel is represented by the normal curve at the bottom. 

![horse.avif](horse.avif)

https://www.youtube.com/watch?v=het9HFqo1TQ
