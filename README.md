# Introduction  
**UV** is a modern, minimalist Python projects and packages manager. Developed entirely in Rust, it has been designed to simplify **Dependency Management**, **virtual environment creation**, and **project organization**. UV aims to resolve common Python project issues like dependency conflicts and environment management. It offers a smoother, more intuitive experience than traditional tools such as the **pip + virtualenv** combo or the **Conda manager**. It is claimed to be **10 to 100 times faster** than traditional handlers. Whether for small personal projects or developing Python applications for production, UV is a **robust and efficient** solution for package management.  

## Starting with UV  
### Installation  
To install UV:  
- **On Windows**: `winget install --id=astral-sh.uv -e`  
- **On Mac or Linux**: `curl -fsSL https://astral.sh/uv/install.sh | sh`  
To verify the installation: `uv version`  

### Creating a New Python Project  
Run: `uv init --python x.xx project_name` (replace `x.xx` with the desired version, e.g., `python 3.12`). If missing, UV downloads it automatically. This initializes a Git repository and creates files: `.gitignore`, `.python-version`, `README.md`, `hello.py`, `pyproject.toml`, and `uv.lock`.  

### Package Installation  
Install a package: `uv add package_name`  
Uninstall a package: `uv remove package_name`  

### Running a Python Script  
Execute inside the virtual environment: `uv run hello.py`  

### Managing Python Versions  
List installed versions: `uv python list`  
Change Python version in `pyproject.toml`: `requires-python = ">=3.9"`  
Sync environment: `uv sync`  
If dependencies are missing: `uv pip install -e .`  

### Switching from Virtualenv to UV  
1. Generate `requirements.txt`: `pip freeze > requirements.txt`  
2. Initialize UV & install dependencies:  


### Using Tools in UV  
- Install a tool: `uv tool install tool_name`  
- Run a tool without installation: `uv tool run tool_name`  
- Shortcut alias: `uvx tool_name`  

## Conclusion  
UV is a **powerful and efficient** Python package manager offering **fast dependency resolution** and **installation**. It outperforms **pip** and **conda**, making it an excellent choice for managing Python projects. If you work with Python, **give UV a try—you might just adopt it for good!**  

## References  
1. [UV Documentation](https://docs.astral.sh/uv/)  
2. [UV GitHub Repository](https://github.com/astral-sh/uv)  
3. [Datacamp Article on UV](https://www.datacamp.com/tutorial/python-uv)  

