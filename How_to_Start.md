# example

A starter Python project scaffolded with **uv**.

## 特性
- 使用 `uv` 进行依赖管理与虚拟环境管理
- 结构化项目布局
- 内置 NumPy 依赖示例
- 开发依赖：Ruff、Pytest

## 安装与使用

```bash
# 克隆仓库
git clone git@github.com:yourusername/my_python_project.git
cd PyStart
# On macOS and Linux.
# install uv
curl -LsSf https://astral.sh/uv/install.sh | sh

# download your project form githubor gitlab
git clone git@github.com:yourusername/Your_python_Project.git
# write your python packages name in pyproject.toml
dependencies = [
  "numpy==1.26.4"  # The most stable and widely compatible version of NumPy
  [packages name ]
]
cd [Your_python_Project]
# run your python files
uv run python [file_name]
# 运行测试
uv pytest

# 代码检查与格式化
uv ruff . --fix