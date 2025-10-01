# 使用 Miniconda 进行包管理

---

## miniconda 的用法与普通虚拟环境的区别

ꔷ 特性 普通虚拟环境 (venv) |———————————— Miniconda (使用 conda)

ꔷ 核心功能 隔离项目的 Python 包 |———————————— 隔离整个环境，包括 Python 版本和其他软件

ꔷ 管理对象 仅 Python 包 (如 requests, Django) |———————————— Python 包、Python 解释器本身、C/C++库、CUDA、R 语言等任何软件

ꔷ 来源 是 Python 3.3+ 内置，无需安装 |———————————— 需独立安装

ꔷ 大小 非常轻量，只在项目目录创建文件夹 |———————————— 较重，需要独立安装几十 MB 的程序

ꔷ 包来源 来自于 PyPI (Python Package Index) |———————————— Anaconda/Conda-Forge 源 (通常是预编译好的二进制包)

ꔷ 典型命令 python -m venv venv source venv/bin/activate pip install ... |————— conda create -n myenv python=3.9 conda activate myenv conda install ...

---

_选择 Miniconda，如果：_

ꔷ1.你从事数据科学、机器学习、生物信息学等领域。

ꔷ2.你需要轻松切换不同的 Python 版本。

ꔷ3.你的项目依赖于复杂的、难以编译的库 (如 PyTorch, TensorFlow, GDAL)。

ꔷ4.你希望在不同操作系统间获得高度一致的开发环境。

```bash
#  下载miniconda安装包
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh

#  安装miniconda(一路确认加enter加yes)
bash Miniconda3-latest-Linux-x86_64.sh

#  conda环境查看
conda env list

#  conda查看已经安装的包
conda list
```

**这个时候关闭当前终端开启多一个终端**

```bash
#  确认是否成功安装conda
conda --version

#  创建conda环境，可以在特定路径下创建
conda create --name condaEnv python=3.10

#  激活conda环境
conda activate condaEnv

#  在conda虚拟环境下安装需要的包, 这里只是一个实例
#  conda install numpy pandas matplotlib

#  关闭虚拟环境
conda deactivate condaEnv
```
