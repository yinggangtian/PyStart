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
cd my_python_project
# On macOS and Linux.
# install uv
curl -LsSf https://astral.sh/uv/install.sh | sh
# 初始化项目（如果还未执行过）
uv init
# 安装虚拟环境
uv venv
# 安装运行时依赖
uv pip install -e .

# 安装开发依赖
uv pip install --dev


# 运行测试
uv pytest

# 代码检查与格式化
uv ruff . --fix