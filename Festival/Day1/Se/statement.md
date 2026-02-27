## 题目背景
:::figure
锦瑟无端五十弦，一弦一柱思华年。

庄生晓梦迷蝴蝶，望帝春心托杜鹃。

沧海月明珠有泪，蓝田日暖玉生烟。

此情可待成追忆，只是当时已惘然。
:::
## 题目描述
给定一个 $m$ 次多项式 $F(x)$ 和一个数列 $\{\varphi_n\}$ 的前 $d$ 项（数列从 $\varphi_0$ 开始）。

该数列的递推式分两种。

当 $d\le n\le d+m$ 时，$\varphi_n=[x^{n+\Omega}]\ln(F(x))+\displaystyle\sum_{i=1}^d \mu_i\varphi_{n-i}$。

当 $n>d+m$ 时，$\varphi_n=F(n)+\displaystyle\sum_{i=1}^d \nu_i\varphi_{n-i}$。

求 $\varphi_\Omega$ 的值。

$\ln(F(x))$ 由泰勒展开定义为 $\displaystyle\sum_{i=0}^{\infty}(-1)^{i+1}\displaystyle\frac{(F(x)-1)^i}{i}$。

答案对 $998,244,353$ 取模。

## 输入格式
{{s.input_file()}}
第一行有两个正整数 $\Omega,d,m$。

第二行有 $d$ 个整数，代表 $\varphi_0,\varphi_1,\cdots,\varphi_{d-1}$。

第三行有 $d$ 个整数，代表 $\mu_1,\mu_2,\cdots,\mu_d$。
	
第四行有 $d$ 个整数，代表 $\nu_1,\nu_2,\cdots,\nu_d$。
	
第五行有 $m+1$ 个整数，代表多项式 $F$ 从低往高的系数。
## 输出格式
{{s.output_file()}}
输出一行一个整数，代表询问的答案。	

严禁面向数据点编程，一经发现立即禁赛十一万四千五百一十四年并全机房通报。
## 样例 1 输入

## 样例 1 输出

## 样例 1 解释

## 数据范围
对于 $100\%$ 的数据，$d,m \le 10^5;\Omega\le 10^9$。
