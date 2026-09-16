# DSC2001 · Python for Data Science

DSC2001 课程的学习笔记、中文讲解与代码练习仓库，随课程进度逐周更新，帮助理解课堂知识并进行实践与复习。

课程涵盖 Python 基础、数据处理与可视化，以及基础机器学习。完整课程介绍与考核要求见根目录的 [课程大纲](DSC2001.pdf)。

## 统一结构

- 按 `WEEK1`、`WEEK2`、`WEEK3`、`WEEK4`……组织各周学习资料。
- 每周的 `source/` 保存笔记原件、原始讲义及课堂演示。
- 对应周目录下保存整理后的中文讲解、练习 Notebook 和配套代码，方便与原件对照学习。

## 使用方法

1. 进入对应周次，先阅读 `source/` 中的原始资料，再结合整理后的笔记理解知识点。
2. 打开 Notebook，从上到下运行代码，观察输出并完成练习。
3. 复习时尝试独立重写示例，再重启 Kernel 并运行全部单元格，检查理解与运行结果。

GitHub 可直接预览笔记；运行代码和完成交互练习需要本地 Python 3 与 Jupyter 环境。

### 本地运行

克隆仓库：

```bash
git clone https://github.com/Dorian1729/DSC2001.git
cd DSC2001
```

安装 JupyterLab 和绘图库并启动：

```bash
python -m pip install jupyterlab matplotlib
python -m jupyterlab
```

也可使用已有的 Anaconda/Jupyter 环境。启动后进入相应周目录，打开 `.ipynb` 文件并选择 Python 3 Kernel；其他依赖按对应笔记中的说明安装。
