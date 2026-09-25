The functionality in the tablefuctions.py file was developed by Vegard Gjerde Buset in 2019 for NTNUI Volleyball. He has been maintaining the repo since, updating with new league rules for relegation and promotion whenever they change.
The purpose of the repo is to generate more visually pleasing tables than Dataproject or TA can offer. 
The Python code generates input to a LaTeX file which contains the tables.
The code was further documented using GitHub Copilot in 2023.

## Setup

Install the Python dependencies with:

```bash
python -m pip install -r requirements.txt
```

Run the table generator from the `src` directory so that its relative paths to
the match data resolve correctly:

```bash
cd src
python tablefunctions.py
```

The dependencies are listed in `requirements.txt`. NumPy is used for numeric
values, and pandas is restricted to versions below 3 because the script uses
legacy DataFrame assignment behavior.
