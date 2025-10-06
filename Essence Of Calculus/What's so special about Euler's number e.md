 
So let's just take $2^t$ for instance 

assumming that 
$$ M(t) = {2^t}$$
from day3 to day4
it grows from 8 to 16

but what we want to find the difference is how does change when we change the $t$ a little bit or some smaller number 

as $dt$,

$$\frac{dM}{dt}(t)=\frac{2^{t+dt}-2^{t}}{dt}$$$$ \frac{dM}{dt}(t)=2^t(\frac{2^{dt}-1}{dt}) $$as $dt \to 0$,the expression will equal to 

$$\frac{dM}{dt}(t)=\frac{d(2^t)}{dt} = 2^t(0.6931...),when\space dt =0.001 $$
and as $dt \to 0$,the constant expression is approaching to a specific number ,which is around **0.6931**.


**and when the f(t)= $8^t$ ,the relevant proportionality constant is around 2.079**

And you maybe find that 2.079 is seemingly 3 times 0.6931

So what does 2 have to do with the numeber 0.6931?
And what does 8 have to do with the number 2.079?

**The second Q is whether there's some base where that proportionality constant is 1?**

where the derivative of a to the power t is not just proportional to itself,but actually equal to itself?

It's **e**!

which means $$\frac{dM}{dt}(t)=e^t(\frac{e^{dt}-1}{dt})
\space,as\space dt \to 0
$$
and this is how **e** is defined,when $dt$ is small enough,the revelent proportionality constant is exactly 1.

when we add some number on e,

for instance,$M(t)=e^{3t}$

$$ \frac{dM}{dt}(t)=e^{3t}(\frac{e^{3dt}-1}{dt})$$

But there is a easier way to get it ,$e^{3t}=e^3\cdot e^t$
put the constant in front of the expression.

