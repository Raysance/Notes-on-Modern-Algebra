# 近世代数Latex笔记生成

## 任务目标

根据 `lec0x.txt` 中的笔记内容，在 `lec0x` 文件夹内生成一份 LaTeX 文档。

## 具体要求

- **内容完善**：补全提到但未完整记录的要点；加入对于所有定理及性质的直观理解和证明。
- **准确性**：修正笔记中不规范及错误的数学表示，笔记中提到的所有内容都需在文档中体现。
- **结构化**：分点清晰明了，保证笔记脉络连贯。
- **排版规范**：保证输出的 LaTeX 格式美观，缩进换行正确。定理/定义/性质/推论等部分请调用 `preamable.tex` 中的样式模板。

## LaTeX 模板头部

生成的 LaTeX 文档应采用以下开头格式：

```latex
\documentclass[11pt]{article}
\usepackage[utf8]{inputenc}
\usepackage{ctex}
\usepackage{amsmath, amssymb, amsthm}
\usepackage{geometry}
\geometry{a4paper, margin=1in}

\input{../preamable/preamable.tex}

\declaretheorem[style=thmgreenbox, name=定义]{cndefinition}
\declaretheorem[style=thmredbox, name=定理]{cntheorem}
\declaretheorem[style=thmbluebox, name=性质]{cnproperty}
\declaretheorem[style=thmredbox, name=引理]{cnlemma}
\declaretheorem[style=thmredbox, numbered=no, name=推论]{cncorollary}
\declaretheorem[style=thmbluebox, numbered=no, name=例]{cnexample}
\title{近世代数笔记(Lec xx)：xxxx}
\author{Raysance}
\date{}
```