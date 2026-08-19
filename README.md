# evaluation

Short description of what this project does.

## Requirements

- **Python 3.12**
- [**uv**](https://docs.astral.sh/uv/) — package & environment manager

### Installing uv

```bash
# Windows (PowerShell)
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"

# macOS / Linux
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Setup

### 1. Check the Python versions available

```bash
uv python list
```

If 3.12 isn't listed, install it:

```bash
uv python install 3.12
```

### 2. Create the virtual environment

```bash
uv venv env --python 3.12
```

### 3. Activate it

```bash
env\Scripts\activate        # Windows (PowerShell / CMD)
source env/bin/activate     # macOS / Linux
```

### 4. Install the dependencies

```bash
uv pip install -r requirements.txt
```

## Usage

```bash
python main.py
```

## Managing dependencies

```bash
uv pip install <package>              # add a package
uv pip freeze > requirements.txt      # lock the current environment
uv pip list                           # show what's installed
```

## Project structure

```
evaluation/
├── env/               # virtual environment (git-ignored)
├── requirements.txt   # Python dependencies
├── .env               # local secrets (git-ignored)
├── .gitignore
└── README.md
```

## License

TBD

