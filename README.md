# Lasso Regularization

This project demonstrates Lasso (L1) regularization on scikit-learn's diabetes dataset.

## Notebooks

- `Lasso.ipynb` — Lasso regression exploration.
- `lasso_key_point.ipynb` — compares model coefficients and test-set R² scores at several Lasso `alpha` values.

## Requirements

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

## Running the notebooks

Open either notebook with Jupyter and run the cells from top to bottom.

```bash
jupyter notebook
```

## Notes

The `r2_score` metric is imported with:

```python
from sklearn.metrics import r2_score
```

If you receive `TypeError: 'list' object is not callable`, the running kernel has overwritten `r2_score` with a list. Restart the kernel and run all cells, or run the import above again.

Use positive `alpha` values with `Lasso`. For an unregularized baseline (`alpha = 0`), use `LinearRegression` instead.
