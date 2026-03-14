# NSFC 面上项目申请书写作逻辑参考模板（LaTeX）

本项目基于 `main.tex + nsfc.sty + GBT7714.bst + reference.bib + .latexmkrc` 构成一套可直接编译的国家自然科学基金（NSFC）面上项目正文示例工程。

## 项目主题

**如何撰写一份高质量的国自然申请书**

该示例不以具体学科研究内容为主，而以“申请书写作逻辑”为主线，围绕：

- 立项依据如何论证科学问题与研究价值
- 研究内容如何形成清晰、可评审的任务链条
- 研究基础如何体现前期积累与可行性
- 其他说明如何保持信息规范与一致性

给出一套具有实操性的正文示范文本。

## 文件结构

```text
.
├── main.tex
├── nsfc.sty
├── reference.bib
├── GBT7714.bst
├── .latexmkrc
└── images/
    └── fig-example.png
```

## 编译方式

推荐命令行编译：

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

也可在 TeXstudio 中配置：

```bash
latexmk -xelatex -synctex=1 %.tex
```

## 使用说明

1. 本项目保留了 `nsfc.sty` 的原始命令体系与版式逻辑；
2. `main.tex` 中使用标准 `\section / \subsection / \subsubsection`，便于 TeXstudio 左侧结构栏导航；
3. 参考文献采用数字型引用，示例文献用于说明写作逻辑，不代表 NSFC 官方参考文献清单；
4. 可直接将 `main.tex` 作为正文写作骨架，按学科领域替换具体内容。

## 版权与声明

- 本模板仅供学习、研究与写作交流使用；
- 该项目并非国家自然科学基金委员会官方模板；
- 使用者应自行核对最新年度官方申请书要求，并对最终提交版本负责。

## License

本项目采用 MIT License 发布。详见仓库中的 LICENSE 文件。
