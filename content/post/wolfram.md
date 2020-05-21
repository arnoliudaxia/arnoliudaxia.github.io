---
author : "ArnoLiu"
title : "Wolfram"
date : "2020-04-13"
description : ""
tags : [
    "wolfram",
    "数学",
    "自然语言",
]
---

# 基础
## 输入输出
a = "中国科学技术大学现代教育技术中心";<br/>
Print["制作单位:", a]


表达式末尾有“;”表示不输出

## 变量
<pre>
清理：
Clear[变量名]
或{变量名}=.
</pre>

## 运算优先级
<pre>
1 []、{}、() 函数、列表、分隔符
2 !、!! 阶乘、双阶乘
3 ++、-- 变量自加1、自减1
4 +=、 -= 、 *= 、 /= 运算后赋值给左边变量
5 ^ 方幂
6 . 矩阵乘积或向量内积
7 *、  乘、除
8 +、- 加、减
</pre>

# 常数

## 数学常数
<pre>
关键字	含义	备注
Degree	°	
E 	e	
GoldenRatio  	1.618	西方黄金分割
Infinity	 ∞	
Pi	π	
</pre>

# 数值
## 操作函数
<pre>
整数操作：
Round[]四舍五入
Floor[]向下取整,Ceiling[]向上取整
实数操作：
N[输入,保留几位]小数输出
实数转为分数:Rationalize[输入,(误差)]
</pre>
		
## 常用初等函数
<pre>
Abs[x] 实数的绝对值或复数的模
Re[z]、Im[z]、Arg[z]、Conjugate[z] 复数的实部、虚部、幅角、共轭
Power[x, y]、Sqrt[x] 幂函数、平方根
Exp[x]、Log[x]、Log[b, x] 指数函数、自然对数函数、对数函数
Max[x1, x2, ...]、Min[x1, x2, ...] 最大值、最小值
Sign[x] 符号函数
Sin[x]、Cos[x]、Tan[x]、Csc[x]、Sec[x]、Cot[x] 三角函数
ArcSin[x]、ArcCos[x]、ArcTan[x]、ArcCsc[x]、
ArcSec[x]、ArcCot[x] 反三角函数
Sinh[x]、Cosh[x]、Tanh[x]、Csch[x]、Sech[x]、Coth[x] 双曲函数
ArcSinh[x]、ArcCosh[x]、ArcTanh[x]、ArcCsch[x]、
ArcSech[x]、ArcCoth[x] 反双曲函数
Factorial[n]、Factorial2[n] 阶乘!、双阶乘!!
FactorInteger[n] 整数分解
GCD[n1, n2, ...]、LCM[n1, n2, ...] 最大公约数、最小公倍数
Mod[m, n]、Mod[m, n, d] 余数
Prime[n]、PrimeQ[n]、PrimePi[n] 素数生成、素数检验、素数计数
</pre>
		
# 字符串
<code>
{ToLowerCase["ABCD"], ToUpperCase["abcd"]}
StringReverse["ABCD"]
</code>	
		
# 列表
## Range
Range[X]->代表从1到x的一个列表<br>
完整：Range[起始,末尾,增量]->

## Table
``Table[表达式,{（变量1），（起始），末尾，（步长）}，（{变量2}）]``

    随机数列表：RandomReal和RandomInteger
    RandomReal[]返回0-1之间的随机浮点数
    RandomInteger[x,y]返回x-y的随机整数
    RandomReal[{范围},随机数个数]
## 列表操作函数
    去除类：
    Drop[列表，放弃元素数]
    Delete[列表，删除元素索引]
    插入类：
    Insert[列表，插入元素，插入索引]
    Append[列表，元素]（值类型函数）
    AppendTo[]插入（引用类型函数）
    排序：
    Sort[]
    Reverse[]
    合并与拆分：
    Flatten[]降维打击（将多维数组降维成一位数组）
    Partition[]数组分组升维
    元素获取：
    集合[[索引]]

## 列表与列表函数
    Union[]多集合的并集
    Intersection[]交集
    Complement[父集合，子集合1，子集合2，····]去除父集合中各子集合成分

# 求取值范围
``FindMaxValue[]``<br>
例子1：├ ``FindMaxValue[{(2−2⁢y)^2+y^2,1/2<y<2/3},{y}]``



