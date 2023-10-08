# 论文写作规范

[TOC]

## 科学计算方向期刊

### Latex模板推荐

- amsart: 自带模板
- elsarticle: JCP 推荐模板，[下载链接](https://www.ctan.org/tex-archive/macros/latex/contrib/elsarticle)

### 结构方面

#### 标题

- 用简单的一句话将文章的主要内容、特点展现出来

#### MSC

- Mathematics Subject Classification (MSC2010) 的作用是向读者快速表明文章所研究的内容是什么，它将数学的各研究分支以相关程度进行分类，并以一个五位长的代码表示这个分类

- 论文中需要这个代码的目的是为了快速告诉读者本文所研究的数学对象，方便找到目标读者

- MSC2010:
  - [主页](https://mathscinet.ams.org/mathscinet/msc/msc2010.html)
  - 几个可以参考的选项：
    - 65M12: Stability and convergence of numerical methods for initial value and initial-boundary value problems involving PDEs
    - 65M32 Numerical methods for inverse problems for initial value and initial-boundary value problems involving PDEs
#### 关键字

#### 摘要

用以让读者快速掌握文章研究的问题、提出的方法以及取得的结果的简短介绍，通常可以由这样的五句话构成：

1. 第一句话交代研究的对象是什么，比如说研究的是在什么条件下的什么微分方程
2. 第二句话交代现有研究的局限是什么，比如说精度不够高，不适合复杂几何
3. 第三句话给出本文的方法，并概括出解决了上面提到的哪些问题
4. 第四句话给出本文方法主要内容的介绍，比方说方法包含两个特殊处理，处理一达到了什么效果，处理二达到了什么效果。特别的，理论结果可以在这里给出
5. 第五句话给出本文的数值结果

#### 引言

#### 方法

#### 数值结果

#### 总结与讨论

### 写作方面

#### 内容

- 每个段落表达一个观点

- 每个段落的第一句话表明整个段落的内容，类似于使得段落具有“总-分”结构

#### 时态

#### 从句

### 数学公式方面

#### 单行公式

- 带编号公式推荐使用
```latex
\begin{equation}
    a^{2} + b^{2} = c^{2}, \label{eqn:sec1:gougudingli}
\end{equation}
```
这里的 label 方便后续进行引用，如在后续段落中我们可以写 Eqn.~\eqref{eqn:sec1:gougudingli}，这样就会自动显示公式的编号，并可以跳转

- 不带编号的公式推荐使用
```latex
\begin{equation*}
    a^{2} + b^{2} = c^{2}
\end{equation*}
```
注意，因为公式不带编号了，所以没有办法进行引用，自然就没有 \label{...} 了

- 单行数学公式的标点符号问题：
  - 如果包含公式的这句话已经结束了，那么在尾部使用句号，如：
  ```latex
  The diffusion equation is
  \begin{equation*}
    \partial_{t} u = \partial_{xx} u.
  \end{equation*}
  ```
  - 如果包含公式的这句话没有结束，需要进行补充说明，那么在尾部使用逗号，如：
  ```latex
  The diffusion equation is
  \begin{equation*}
    \partial_{t} u = D \partial_{xx} u,
  \end{equation*}
  where $D$ is the diffusion coefficient.
  ```

#### 多行公式

#### 自定义命令

使用自定义命令可以简化写作

### 画图方面

#### 图像质量

- 推荐输出 eps 格式的图片，且 `dpi` 要求不低于 100，这样文章在印刷时可以保证图像清晰不损失信息

#### 图像内容

- 图像中如果有多条曲线，那么需要每条曲线的标签

### 表格方面

### 可供参考的优秀模板

