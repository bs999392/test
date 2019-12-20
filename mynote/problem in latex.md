# Latex问题以及解决方案
>1. 字体缺失\
    1) 下载对应的字体\
    2) 调用XeLatex来编译\
    3) 安装对应字体时，需要为全部用户安装
   
>2. 下标放于下方\
    解决办法：\
     1) 使用代码\$limits_{}\$位于需要的后面 例如:
      >> \$\sum \limits_{k=1}^n\$ 
      >>>  $\sum \limits_{k=1}^n$

>3. 如何自定义编号\
     解决办法：\
      1) 构造环境 gather 、align*等等
      2) 使用标签\tag\*{...}
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
