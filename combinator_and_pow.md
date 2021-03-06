令 <img src="https://latex.codecogs.com/gif.latex?S&space;=&space;\{1,2,\cdots,n&plus;1\}" title="S = \{1,2,\cdots,n+1\}" />，其中 <img src="https://latex.codecogs.com/gif.latex?n\ge2" title="n\ge2" />，
<img src="https://latex.codecogs.com/gif.latex?T=\{(x,y,z)|x,y,z\in&space;S,x<z,y<z\}" title="T=\{(x,y,z)|x,y,z\in S,x<z,y<z\}" /><br>
证明:<br>
1.<br>
<img src="https://latex.codecogs.com/gif.latex?|T|=\binom{n&plus;1}{2}&plus;2\binom{n&plus;1}{3}" title="|T|=\binom{n+1}{2}+2\binom{n+1}{3}" />.<br>	 
2.<br>
<img src="https://latex.codecogs.com/gif.latex?|T|=\sum_{k=1}^nk^2" title="|T|=\sum_{k=1}^nk^2" />.<br>
>1.可以先假设<img src="https://latex.codecogs.com/gif.latex?x=y" title="x=y" />，然后从集<img src="https://latex.codecogs.com/gif.latex?A" title="A" />中取出两个不同的数字，大者为<img src="https://latex.codecogs.com/gif.latex?z" title="z" />，小者为<img src="https://latex.codecogs.com/gif.latex?x,y" title="x,y" />，易知共有<img src="https://latex.codecogs.com/gif.latex?\binom{n&plus;1}{2}" title="\binom{n+1}{2}" />种取法，当假设<img src="https://latex.codecogs.com/gif.latex?x\ne&space;y" title="x\ne y" />，从集合<img src="https://latex.codecogs.com/gif.latex?A" title="A" />中取出三个不同的数字，最大者为<img src="https://latex.codecogs.com/gif.latex?z" title="z" />，次大者为 <img src="https://latex.codecogs.com/gif.latex?x" title="x" /> 或者 <img src="https://latex.codecogs.com/gif.latex?y" title="y" />，共有<img src="https://latex.codecogs.com/gif.latex?2\cdot&space;\binom{n&plus;1}{3}" title="2\cdot \binom{n+1}{3}" />种取法，所以共有<img src="https://latex.codecogs.com/gif.latex?\binom{n&plus;1}{2}&plus;2\binom{n&plus;1}{3}" title="\binom{n+1}{2}+2\binom{n+1}{3}" />种取法。<br>
>2.假设当 <img src="https://latex.codecogs.com/gif.latex?z=2" title="z=2" /> 时，<img src="https://latex.codecogs.com/gif.latex?x" title="x" />，<img src="https://latex.codecogs.com/gif.latex?y" title="y" /> 共有 <img src="https://latex.codecogs.com/gif.latex?1\cdot&space;1" title="1\cdot 1" /> 种取法；<br>
>当 <img src="https://latex.codecogs.com/gif.latex?z=3" title="z=3" /> 时，<img src="https://latex.codecogs.com/gif.latex?x" title="x" />，<img src="https://latex.codecogs.com/gif.latex?y" title="y" /> 共有 <img src="https://latex.codecogs.com/gif.latex?2\cdot&space;2" title="2\cdot 2" /> 种取法；<br>
	   <img src="https://latex.codecogs.com/gif.latex?\cdots" title="\cdots" /><br>
>当 <img src="https://latex.codecogs.com/gif.latex?z=n&plus;1" title="z=n+1" /> 时，<img src="https://latex.codecogs.com/gif.latex?x" title="x" />，<img src="https://latex.codecogs.com/gif.latex?y" title="y" /> 共有 <img src="https://latex.codecogs.com/gif.latex?n\cdot&space;n" title="n\cdot n" /> 种取法；<br>
>故 <img src="https://latex.codecogs.com/gif.latex?|T|=\sum_{i=1}^ni^2" title="|T|=\sum_{i=1}^ni^2" />。<br>
>>推论：当 
	   <img src="https://latex.codecogs.com/gif.latex?T=\{(x_1,x_2,\cdots,x_k,z)|x_1,x_2,\cdots,x_k,z\in&space;A,x_1,x_2,\cdots,x_k<z\}" title="T=\{(x_1,x_2,\cdots,x_k,z)|x_1,x_2,\cdots,x_k,z\in A,x_1,x_2,\cdots,x_k<z\}" />
>有<br>
	  <img src="https://latex.codecogs.com/gif.latex?|T|=\sum_{i=1}^ni^k=\sum_{j=1}^k\binom{n&plus;1}{j&plus;1}\cdot&space;S(k,j)\cdot&space;j!" title="|T|=\sum_{i=1}^ni^k=\sum_{j=1}^k\binom{n+1}{j+1}\cdot S(k,j)\cdot j!" /><br>
>注:<img src="https://latex.codecogs.com/gif.latex?S(n,k)" title="S(n,k)" /> 为第二类Stirling数，满足递推关系:<br>
	  <img src="https://latex.codecogs.com/gif.latex?S(n&plus;1,k)=S(n,k-1)&plus;kS(n,k)\quad&space;(1\le&space;k\le&space;n)." title="S(n+1,k)=S(n,k-1)+kS(n,k)\quad (1\le k\le n)." />




