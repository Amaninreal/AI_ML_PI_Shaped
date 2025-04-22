# AI_ML_PI_Shaped

## Objective

Practice foundational Python functional programming concepts by working with a real-world dataset. We perform data cleaning, preprocessing, and basic analysis using pure functions, `map()`, `filter()`, and `Counter`—without mutating the original dataset.

---

## Dataset

- **Source:** [Iris Dataset (Seaborn)](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv)
- **Columns:** `sepal_length`, `sepal_width`, `petal_length`, `petal_width`, `species`
- **Format:** CSV

---

## Steps & Functional Operations

### 1. **Load the Dataset**

```python
import pandas as pd

df = pd.read_csv("https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv")
