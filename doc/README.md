# Cache-Coherent-and-A-Quantitative-Approach（高速缓存一致性和量化分析）

建立这个仓库的初衷是通过学习和总结计算机体系结构中的高速缓存子系统，将其归纳总结；同时为了更好的将其应用在计算机芯片架构的设计中，针对比较重要的缓存方法通过建模的方式进行量化分析。所以仓库最终呈现出来的是一份关于高速缓存系统的文档以及在此基础上的建模和量化分析的系统。
## 文档介绍
关于文档，首先有一下说明：

1、为了内容及必要公式的严谨性，文档的排版采用Latex的格式，采用的是中国科学技术大学的学位论文LaTeX模板[ustcthesis](https://github.com/ustctug/ustcthesis/releases)，在此基础上进行相应的修改。

2、写文档是一个繁重的任务，不仅需要表达的准确性，同时要进行校准、更新。Doc目录下是完整的可编译的Latex项目，如果你对高速缓存一致性感兴趣，欢迎一起合作。

## 编译文档

- 编译模板的使用说明文档 `ustcthesis-doc.pdf`，这是关于整个模版的说明文档：
   ```
   latexmk -xelatex ustcthesis-doc.tex
   ```
- 编译文档 `缓存一致性和量化分析.pdf`：
   ```
   latexmk -xelatex 缓存一致性和量化分析.tex
   ```
- 如需清理文档编译过程中的临时文件，可以：
   ```
   latexmk -c
   ```

- 以上编译过程也可以用 `make` 工具：
   ```
   make doc        # 编译生成 ustcthesis-doc.pdf
   make            # 编译生成论文 缓存一致性和量化分析.pdf
   make clean      # 删除编译过程中生成的临时文件
   ```

## 更多资料

- [LaTeX 新手入门指南](https://github.com/ustctug/ustcthesis/wiki/新手指南)
- [常见问题 FAQ](https://github.com/ustctug/ustcthesis/wiki/常见问题)
- [参与开发](https://github.com/ustctug/ustcthesis/wiki/参与开发)
