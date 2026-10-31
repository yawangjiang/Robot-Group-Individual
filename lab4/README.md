# LAB4 个人交付

- [deliverables_1_2.pdf](deliverables_1_2.pdf)：两项个人题合并PDF，共3页。
- [source/](source/)：PDF的LaTeX主文件及样式。
- [verification.txt](verification.txt)：五个有限维QP的精确解、目标值及多段约束计数恒等式。

PDF第1页给出一次、二次、三次多项式的最小速度轨迹；第2页加入末端速度约束并求解；第3页给出多段minimum-snap以及一般r阶问题的系数与约束计数。

## 编译

```bash
cd source
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=.. deliverables_1_2.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=.. deliverables_1_2.tex
```

约束计数按单个标量坐标、固定正段时长、外端0至r−1阶导数固定、内部非位置导数自由的假设给出。区分几何航点数量与左右段位置方程数量，避免重复计数。

题目来源：[MIT VNAV LAB4](https://vnav.mit.edu/labs_2023/lab4/exercises.html)。
