# Power BI Report with Python Visuals

This report visualizes regional sales data using Python integration in Power BI.

## Tools Used
- Power BI Desktop
- Python 3.13
- Libraries: seaborn, matplotlib, pandas

## How It Works
- Dragged `Region` and `Sales` columns into the Python visual.
- Used seaborn to create a bar plot of sales by region.

## Sample Python Code
```python
import seaborn as sns
import matplotlib.pyplot as plt

dataset.columns = dataset.columns.str.replace('value.', '', regex=False)
sns.barplot(x=dataset['Region'], y=dataset['Sales'])
plt.xticks(rotation=45)
plt.title("Sales by Region")
plt.tight_layout()
plt.show()
