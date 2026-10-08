# Python Programming

A set of Python solutions covering five tasks, from algorithms to a full data-analysis case with pandas and visualisations. All in one Jupyter notebook.

## What's inside

See [`python_programming.ipynb`](python_programming.ipynb) — each task has markdown explanations before and after the code.

| Task | Topic | What it shows |
|------|-------|---------------|
| 1 | **Supernacci sequence** | An iterative (non-recursive) sequence built with list slicing |
| 2 | **Debug the dice game** | Finding and fixing 10 bugs in a broken program, each explained |
| 3 | **Dictionaries & geography** | Nearest-city/POI lookup, city boundaries, assigning and ranking POIs using `min()`/`sorted()` with lambdas |
| 4 | **NumPy trace** | Computing a matrix trace with a square-matrix guard, verified against `np.trace()` |
| 5 | **Udir grade statistics** | Loading, cleaning and analysing real Oslo high-school grade data |

## Highlight — Task 5: Oslo grade analysis

Using real grade data from Udir (Oslo, 2024-25), the notebook:

- Loads a messy UTF-16 tab-separated export, filters to Oslo, renames columns and converts Norwegian decimal commas to numeric
- Produces three visualisations: average grade by assessment type, a distribution box plot, and the top 10 schools by standpunkt grade
- Answers a research question: **do Oslo schools follow the national pattern where oral > teacher-set > written exam grades?** (they do: 4.34 > 4.09 > 3.51)
- Ranks schools by the gap between teacher-set and written-exam grades, and discusses what that gap means, with honest caveats about subject mix, sample size and single-year data

## Tech

Python · Jupyter · NumPy · pandas · matplotlib · seaborn

## Running it

```bash
pip install numpy pandas matplotlib seaborn jupyter
jupyter notebook python_programming.ipynb
```

Task 5 expects the Udir CSV in a `data/` folder next to the notebook — the download steps are described in the notebook itself.
