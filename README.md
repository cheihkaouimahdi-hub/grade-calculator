# Student Grade Calculator

A simple Python application that calculates the average grade of a student
and determines whether the student passes.

## Installation

```bash
pip install -r requirements.txt
```

## Usage

Import the functions in Python:

```python
from calculator import calculate_average, get_grade_category, is_passing

average = calculate_average([10, 12, 14])

print(average)                      # 12.0
print(is_passing(average))          # True
print(get_grade_category(average))  # Good
```

- `calculate_average` raises a `ValueError` if the list is empty.
- `is_passing` returns `True` for an average of 10 or higher.
- `get_grade_category` returns `Excellent` (16 or higher), `Good` (12 or higher), `Average` (10 or higher), or `Fail` (below 10).

## Run Tests

```bash
pytest -v
```

## Run Linting

```bash
flake8 .
```
