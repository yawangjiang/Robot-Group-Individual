# LAB3 个人交付

- [deliverable_1.txt](deliverable_1.txt)：个人题1的五项代码答案及所需头文件。
- [deliverable_2.pdf](deliverable_2.pdf)：个人题2的矩阵秩分析和指定二次阻力补偿推导，共2页。
- [source/](source/)：PDF的LaTeX主文件及样式。
- [verification.txt](verification.txt)：矩阵行列式、秩、行相关关系与阻力方向核算。

## 编译

在安装常规 TeX Live 包的环境中：

```bash
cd source
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=.. deliverable_2.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=.. deliverable_2.tex
```

矩阵使用报告中明确写出的上向z坐标系及电机编号。讨论的是改装后的旋翼继续产生正向升力、偏航反力矩符号发生变化的情形。阻力模型为题目指定的速度平方模型，不是线性阻力。

题目来源：[MIT VNAV LAB3](https://vnav.mit.edu/labs_2023/lab3/exercises.html)。
