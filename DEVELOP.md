# Initial Setup

Create a Python virtual environment:

```
python3 -m venv mkdocs-material-venv/ 
```

Activate the Python virtual environment:

```
source mkdocs-material-venv/bin/activate
```

Install `mkdocs-material`:

```
pip install mkdocs-material
```

# Start Local Server

Activate the Python virtual environment:

```
source mkdocs-material-venv/bin/activate
```

Run the following from the repository root directory:

```
mkdocs serve
```

Open: http://127.0.0.1:8000

The server rebuilds the pages whenever a source file changes and automatically reloads the browser.
