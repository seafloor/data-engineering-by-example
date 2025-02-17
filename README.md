# Data Engineering by Example

A collection of small, focused data engineering examples using Python, SQL, and Bash. The goal is to explore different data processing methods without getting bogged down in tooling or project structures, which are all important but not the focus here.  

- 🚀 **Methods-first examples** → deliberately side-steps tooling, abstract ideas, and broader parts of the pipeline
- 🚀 **Minimal Setup** → No global environments, each script defines its own deps.  
- 🚀 **Easy to Run** → Each example is **self-contained** and runs using **PEP 723 + `uv`**, keeping dependencies lightweight.

---

## How to Run Examples

1. **Install `uv` (if not already installed):**  
   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```
   
2. **Run any example using `uv`:**  
   ```bash
   uv run example_dir/script.py
   ```

Each script defines its own dependencies at the top using [PEP 723](https://peps.python.org/pep-0723/), so there's no need to manually install anything.  

Each directory contains **an independent example**, focusing on a specific data engineering problem.

---

## Development & Testing (Optional)

For testing, linting, or contributions, there's an **optional root development environment**:  

1. **Create a dev environment** (only if needed):  
   ```bash
   uv venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\activate
   uv pip install -r dev-requirements.txt
   ```
   
2. **Run tests:**  
   ```bash
   pytest tests/
   ```

This environment is **not required to run examples**—it's just for **development, testing, and consistency**.

---

## License etc.
This project is licensed under the **MIT License**. Contributions are welcome!
