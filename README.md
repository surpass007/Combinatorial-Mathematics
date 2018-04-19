计算从 <a href="https://www.codecogs.com/eqnedit.php?latex=$$(0,&space;0)$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$(0,&space;0)$$" title="$$(0, 0)$$" /></a> 
点到 $(n,n)$ 点的不穿过直线 $y = x$ 的非降路径数。
	ax^{2} + by^{2} + c = 0
首先我们有 $$\binom{r}{r}+\binom{r+1}{r}+\cdots+\binom{n}{r}=\binom{n+1}{r+1}$$

令从点 $(0,0)$ 到点 $(i,j) $ 的路径数为 $a[i,j]$，先考虑右下三角形 $(i > j)$，与左上三角形 $(i < j)$ 对称， 则有$$a[i,j]=\left\{\begin{array}{cc} 
		a[i-1,j]+a[i,j-1], & i>j\ge1\\ 
		a[i,j-1], & i=j \\
		1, & j = 0
	\end{array}\right.$$
	可知 $a[n,1]=a[n-1,1]+a[n,0]=a[n-1,1]+1=a[1,1]+n-1=n=\binom{n}{1}$，而 $a[n,2]=a[n-2,2]+a[n-1,1]=a[2,1]+a[3,1]+\cdots+a[n-1,1]+a[n,1]=\binom{2}{1}+\binom{3}{1}+\binom{n-1}{1}+\binom{n}{1}=\binom{n+1}{2}-\binom{n+1}{0}$；同理 $a[n，3]=\binom{n+2}{3}-\binom{n+2}{1}$；
	于是有 $a[n,n]=\binom{2n-1}{n}-\binom{2n-1}{n-2}=\frac{(2n-1)
	!}{n!(n-1)!}-\frac{(2n-1)!}{(n-2)!(n+1)!}=\frac{(2n-1)!}{(n-2)!n!}(\frac{1}{n-1}+\frac{1}{n+1})=\frac{(2n)!}{n!n!(n+1)}=\binom{2n}{n}\frac{1}{n+1}$

<img src="https://latex.codecogs.com/gif.latex?ax^{2}&space;&plus;&space;by^{2}&space;&plus;&space;c&space;=&space;0" title="ax^{2} + by^{2} + c = 0" />
