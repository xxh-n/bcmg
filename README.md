# CSEC Lab 信息安全基础能力训练

学号后六位： **303754** 

本仓库为《信息安全基础能力训练》课堂实验代码，包含两个 Python 示例：

-  **示例一** ：网页单词提取器（爬取网页、提取单词、统计词频、输出 Top 10、生成常见密码变形）
-  **示例二** ：Bind Shell（监听端口的远程命令 shell，仅用于授权实验环境）

> 注意：所有代码仅用于课程实验与授权环境。
> 示例二严禁用于任何你未拥有或未获授权测试的主机。

## 仓库结构

csec-lab/
├── example1/
│ └── wordextractor.py # 网页单词提取器
├── example2/
│ └── bindshell.py # Bind Shell（单线程与多线程版本）
├── requirements.txt
├── .gitignore
└── README.md


## 环境要求

- 操作系统：Ubuntu 24.04.5 LTS（虚拟机）
- Python：3.12+
- IDE：VSCode 或 PyCharm（开启 PEP8 检查）
- 第三方库：`requests`、`beautifulsoup4`、`click`
- 检查工具：`flake8`（最大行宽 79）
- 网络测试工具：`netcat`（`nc`）

## 环境搭建

```bash
# 1. 创建并激活虚拟环境
python3 -m venv env
source env/bin/activate

# 2. 安装依赖
pip install -r requirements.txt

# 3.（可选）安装代码检查工具
pip install flake8
