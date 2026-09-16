# DSC2001 · Python for Data Science

DSC2001 课程的学习笔记、中文讲解与代码练习仓库。按 `WEEK1`、`WEEK2`、`WEEK3`、`WEEK4`……逐周整理，将课堂材料转化为便于理解、运行和复习的学习笔记。

每周目录下的 **`source/` 保存笔记原件、原始讲义和课堂演示**；基于原件整理的讲解、练习 Notebook 和配套代码放在对应的 `WEEK*/` 目录下。当前已收录 **WEEK2**，其他周次随课程进度补充。

## 课程概览

以下课程信息依据根目录的 [DSC2001.pdf](DSC2001.pdf) 整理，该文件为课程大纲。

| 项目 | 内容 |
| --- | --- |
| 课程名称 | Python for Data Science |
| 课程编号 | DSC2001 |
| 大纲适用学期 | Semester A 2026/27 |
| 开课单位 | Data Science（DS），College of Computing（CC） |
| 学分与学制 | 4 学分，一个学期 |
| 授课与考核语言 | 英语；本仓库以中文辅助讲解 |
| 每周教学活动 | Lecture 3 小时，Tutorial 1 小时 |

课程注重使用 Python 独立完成数据处理、分析和初步建模，通过实际代码和案例培养数据科学编程能力。学习内容包括：

- **Python 基础与开发工具**：环境配置、IPython/Jupyter、数据结构、文件操作、函数、面向对象编程、性能计时，以及 GitHub 版本控制。
- **科学计算与数据分析**：NumPy 多维数组、索引与切片、数组运算和随机数；Pandas 的 Series、DataFrame、筛选、排序等操作；Matplotlib 可视化。
- **基础机器学习**：使用 Scikit-learn 进行预处理、特征提取、线性回归、二分类、决策树、随机森林、K 近邻与模型选择。
- **综合应用**：通过探索性数据分析与案例练习解决实际问题。

这些是大纲覆盖的内容，不代表所有主题的笔记都已上传，也不预设各主题对应的教学周次。

## 目录结构

当前文件结构：

```text
DSC2001/
├── README.md
├── .gitignore
├── DSC2001.pdf                         # 课程大纲
└── WEEK2/
    ├── Lec2_Jupyter_学习与练习.ipynb    # Jupyter 讲解、示例与练习
    ├── OOP_学习与练习.ipynb             # 面向对象编程讲解与练习
    ├── lec2_hello_demo.py              # Jupyter 配套脚本
    └── source/                        # 笔记原件与课堂资料
        ├── Lec 2.docx
        ├── OOP approach.docx
        ├── Tutorial 02 Ver2.docx
        └── demo.ipynb
```

后续按相同结构新增 `WEEK1/`、`WEEK3/`、`WEEK4/` 等目录，每周将原件放入自己的 `source/`。目录名统一使用大写 `WEEK` 加周次；原件目录沿用当前的小写 `source`，以确保跨平台路径一致。

## 每周学习索引

| 周次 | 当前内容 | 入口 |
| --- | --- | --- |
| WEEK1 | 待补充 | — |
| WEEK2 | Jupyter Notebook/Lab、OOP；另含 Python Basics II 原始 Tutorial | [查看 WEEK2](WEEK2/) |
| WEEK3 | 待补充 | — |
| WEEK4 | 待补充 | — |

### WEEK2：Jupyter 与面向对象编程

| 学习资料 | 主要内容 |
| --- | --- |
| [Jupyter 学习与练习](WEEK2/Lec2_Jupyter_学习与练习.ipynb) | Notebook 与 Kernel、执行顺序、Magic Commands、对象查询、Tab 补全、工作目录、Console、Markdown、绘图与易错点 |
| [OOP 学习与练习](WEEK2/OOP_学习与练习.ipynb) | 从过程式编程到类与对象，封装、继承、抽象、多态，`ABC`、`Protocol`，动手练习与自动检查 |
| [配套 Python 脚本](WEEK2/lec2_hello_demo.py) | 供 Jupyter 中的 `%run`、`%load` 示例使用 |

原始资料：

- [Lec 2.docx](WEEK2/source/Lec%202.docx)：Jupyter Notebook/Lab 与 IPython 常用功能。
- [OOP approach.docx](WEEK2/source/OOP%20approach.docx)：过程式编程到 OOP 的思路与核心概念。
- [Tutorial 02 Ver2.docx](WEEK2/source/Tutorial%2002%20Ver2.docx)：列表、元组、集合、字典、函数参数、类与对象、多态、模块和异常处理。目前仅收录原件，尚无独立的 Tutorial 讲解 Notebook。
- [demo.ipynb](WEEK2/source/demo.ipynb)：原始课堂演示。

## 如何学习与运行

1. 先阅读 [课程大纲](DSC2001.pdf)，了解课程目标和知识范围。
2. 进入对应周次，结合 `source/` 原件阅读整理后的中文讲解。
3. 在 Jupyter 中从上到下运行 Notebook，观察结果，再独立完成练习。
4. 复习时重启 Kernel 并重新运行全部单元格，检查是否依赖之前遗留的变量状态；交互操作部分按文中步骤手动完成。

### 本地启动

将仓库克隆到本地：

```bash
git clone https://github.com/Dorian1729/DSC2001.git
cd DSC2001
```

使用 Python 3 环境安装当前 WEEK2 所需的 JupyterLab 和绘图库：

```bash
python -m pip install jupyterlab matplotlib
python -m jupyterlab
```

也可以使用已有的 Anaconda/Jupyter 环境。启动后进入 `WEEK2/`，打开对应的 `.ipynb`，选择 Python 3 Kernel。OOP 练习使用 Python 标准库；Matplotlib 用于 Jupyter 笔记中的绘图示例。后续周次如需额外依赖，将随笔记补充。

在 GitHub 上可以直接预览 Notebook；实际执行代码和完成交互练习需要本地 Jupyter 环境。

### 阅读现有资料时的说明

- 原始讲义包含伪代码及部分拼写、语法问题，整理后的 Notebook 对相关概念和易错点做了说明。
- 原始 `demo.ipynb` 引用了当前未收录的 `python_anaconda.jpg`，相应图片无法显示。
- Jupyter 学习 Notebook 开头的原件链接仍使用旧的相对路径；查阅原件时可使用本 README 上方的链接，或进入 `WEEK2/source/`。
- 部分现有示例保留了 `DS2004` 字样；本仓库的课程编号以根目录大纲中的 **DSC2001** 为准。

## 考核信息

根据 [课程大纲](DSC2001.pdf) 第 3–4 页：

| 考核项目 | 占比 |
| --- | --- |
| Assignments | 25% |
| Course Project | 25% |
| Examination | 50% |

考试时长为 **2 小时**。通过课程需总评达到 **40%**，且持续评核与考试两部分分别达到 **30%**。大纲中 Assignments 与 Course Project 的 “Allow Use of GenAI?” 均标为 **No**。具体安排以任课教师通知为准。

## 参考阅读

根目录课程大纲列出的阅读材料：

- **必读**：Jake VanderPlas，*Python Data Science Handbook: Essential Tools for Working with Data*，2016。
- **补充**：Wes McKinney，*Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython*，第 2 版，2017。
- **补充**：Peter Morgan，*Data Analysis from Scratch with Python*，第 2 版，2018。

本仓库用于课程学习与复习；原始课程资料与个人整理内容通过 `source/` 目录区分。
