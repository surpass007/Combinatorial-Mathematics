计算从 <a href="https://www.codecogs.com/eqnedit.php?latex=$$(0,&space;0)$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$(0,&space;0)$$" title="$$(0, 0)$$" /></a> 
点到 <img src="https://latex.codecogs.com/gif.latex?(n,n)" title="(n,n)" /> 点的不穿过直线 <img src="https://latex.codecogs.com/gif.latex?y&space;=&space;x" title="y = x" /> 的非降路径数。
	ax^{2} + by^{2} + c = 0
首先我们有 <img src="https://latex.codecogs.com/gif.latex?\binom{r}{r}&plus;\binom{r&plus;1}{r}&plus;\cdots&plus;\binom{n}{r}=\binom{n&plus;1}{r&plus;1}" title="\binom{r}{r}+\binom{r+1}{r}+\cdots+\binom{n}{r}=\binom{n+1}{r+1}" />

令从点 <img src="https://latex.codecogs.com/gif.latex?(0,0)" title="(0,0)" /> 到点 <img src="https://latex.codecogs.com/gif.latex?(i,j)" title="(i,j)" />  的路径数为 $a[i,j]$，先考虑右下三角形 $(i > j)$，与左上三角形 $(i < j)$ 对称， 则有 <img src="https://latex.codecogs.com/gif.latex?a[i,j]=\left\{\begin{array}{cc}&space;a[i-1,j]&plus;a[i,j-1],&space;&&space;i>j\ge1\\&space;a[i,j-1],&space;&&space;i=j&space;\\&space;1,&space;&&space;j&space;=&space;0&space;\end{array}\right." title="a[i,j]=\left\{\begin{array}{cc} a[i-1,j]+a[i,j-1], & i>j\ge1\\ a[i,j-1], & i=j \\ 1, & j = 0 \end{array}\right." />
	可知 <img src="https://latex.codecogs.com/gif.latex?a[n,1]=a[n-1,1]&plus;a[n,0]=a[n-1,1]&plus;1=a[1,1]&plus;n-1=n=\binom{n}{1}" title="a[n,1]=a[n-1,1]+a[n,0]=a[n-1,1]+1=a[1,1]+n-1=n=\binom{n}{1}" />，而 <img src="https://latex.codecogs.com/gif.latex?a[n,2]=a[n-2,2]&plus;a[n-1,1]=a[2,1]&plus;a[3,1]&plus;\cdots&plus;a[n-1,1]&plus;a[n,1]=\binom{2}{1}&plus;\binom{3}{1}&plus;\binom{n-1}{1}&plus;\binom{n}{1}=\binom{n&plus;1}{2}-\binom{n&plus;1}{0}" title="a[n,2]=a[n-2,2]+a[n-1,1]=a[2,1]+a[3,1]+\cdots+a[n-1,1]+a[n,1]=\binom{2}{1}+\binom{3}{1}+\binom{n-1}{1}+\binom{n}{1}=\binom{n+1}{2}-\binom{n+1}{0}" />；同理 <img src="https://latex.codecogs.com/gif.latex?a[n，3]=\binom{n&plus;2}{3}-\binom{n&plus;2}{1}" title="a[n，3]=\binom{n+2}{3}-\binom{n+2}{1}" />；
	于是有 <img src="https://latex.codecogs.com/gif.latex?a[n,n]=\binom{2n-1}{n}-\binom{2n-1}{n-2}=\frac{(2n-1)&space;!}{n!(n-1)!}-\frac{(2n-1)!}{(n-2)!(n&plus;1)!}=\frac{(2n-1)!}{(n-2)!n!}(\frac{1}{n-1}&plus;\frac{1}{n&plus;1})=\frac{(2n)!}{n!n!(n&plus;1)}=\binom{2n}{n}\frac{1}{n&plus;1}" title="a[n,n]=\binom{2n-1}{n}-\binom{2n-1}{n-2}=\frac{(2n-1) !}{n!(n-1)!}-\frac{(2n-1)!}{(n-2)!(n+1)!}=\frac{(2n-1)!}{(n-2)!n!}(\frac{1}{n-1}+\frac{1}{n+1})=\frac{(2n)!}{n!n!(n+1)}=\binom{2n}{n}\frac{1}{n+1}" />


