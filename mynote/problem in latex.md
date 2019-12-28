# Latex问题以及解决方案
>1. 字体缺失\
    1) 下载对应的字体\
    2) 调用XeLatex来编译\
    3) 安装对应字体时，需要为全部用户安装
   
>2. 下标放于下方\
    解决办法：\
     1) 使用代码\$limits_{}\$位于需要的后面 但只能对公式这么做.例如:
     2) 使用\underset。注意\underset 尽量一个嵌套，多个嵌套会出错. 
     3) \inf \sup 其使用\inf_n时，n会位于下方（latex语法与markdown中不同）
      >> \$\sum \limits_{k=1}^n\$ \
      >> \$ \inf _n \$
      >>>  $\sum \limits_{k=1}^n$ \
      >>> $\inf \limits_{n}$
>3. 如何自定义编号\
     解决办法：\
      1) 构造环境 gather 、align*等等
      2) 使用标签\tag\*{...}
      3) \notag 可以去除该行编号
      4) align 环境下，不要空行
       >>  \begin{align}\
       \big(\sum \limits_{k=1}^n a_k b_k \big)^2 \leqslant \sum \limits_{k=1}^n a_k^2 \cdot \sum \limits_{k=1}^n b_k^2 \
    \end{align}
    >>> 
>4. 处理公式中的文字问题\
     解决办法：\
      1) 使用\textbf{} 强调
      2) 使用\mbox{} 插入
       >> \$ a \mbox{是1}\$
       >>> $a 是1$
>5. 积分中的求导符
     解决办法：\
      1） 使用\dif
      2） 使用\mathrm
      >> \DeclareMathOperator\dif{d\!}
      >>  \$\dif x\$
       >>> $\mathrm{d} x$
>6. 反斜杠
     解决办法：\
      1) \backslash
        >> \$ \backslash\$
        >>> $\backslash$

>7. 交叉引用问题

>8. 冒号问题：\
    在数学环境下的冒号会自动表示比值符号，比值符号两侧等距，而赋值符号，右边空间更大.需要注意.疑惑而colon则是左小右大\
    1） 数学冒号： \$:\$\
    2)  赋值号: \$ \colon \$
        >> \$x:2\$\
        >>\$ x \colon 2\$
        >>> $x:2$ \
        >>> $x \colon 2$

>9. 顶部线偏移\
    解决办法：注意\bar 和\overline 的运用

>10. 空集符号\
    解决办法：使用\emptyset,不过长得不好看
     >>\$\emptyset\$
     >>>$\emptyset$

>11. 大括号多行公式\
    解决办法：使用\begin{case}环境
    >>   \$D(x)=\
         \begin{cases}  \
           1\\\\\
           0   
         \end{cases}\$
    >>> $D(x)=
      \begin{cases}  
        1 \\
        0   
      \end{cases}$

    