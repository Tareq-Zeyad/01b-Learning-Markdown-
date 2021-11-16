# Data Visualization


### What is Data Visualization ?

Data visualization is the discipline of trying to understand data by placing it in a visual context so that patterns, trends and correlations that might not otherwise be detected can be exposed. Python offers multiple great graphing libraries that come packed with lots of different features.


### How can we Visualize Data in Python ?

We can visualize Data in python using a library called Seaborn which is a Python data visualization library based on Matplotlib.


### What are the available Data Visualization Types in matplotplib ?

1. Line Chart
2. Histogram
3. Bar Chart
4. Box plots
5. Heatmap
6. Scatter Chart


### Code Examples:

```Python
import seaborn as sns
sns.set_theme(style="darkgrid")

# Load an example dataset with long-form data
fmri = sns.load_dataset("fmri")

# Plot the responses for different events and regions
sns.lineplot(x="timepoint", y="signal",
             hue="region", style="event",
             data=fmri)
```

![image](https://seaborn.pydata.org/_images/errorband_lineplots.png)

```Python
import seaborn as sns
sns.set_theme(style="whitegrid")

penguins = sns.load_dataset("penguins")

# Draw a nested barplot by species and sex
g = sns.catplot(
    data=penguins, kind="bar",
    x="species", y="body_mass_g", hue="sex",
    ci="sd", palette="dark", alpha=.6, height=6
)
g.despine(left=True)
g.set_axis_labels("", "Body mass (g)")
g.legend.set_title("")
```

![chart](https://seaborn.pydata.org/_images/grouped_barplot.png)

```Python
import numpy as np
import seaborn as sns
sns.set_theme(style="ticks")

rs = np.random.RandomState(11)
x = rs.gamma(2, size=1000)
y = -.5 * x + rs.normal(size=1000)

sns.jointplot(x=x, y=y, kind="hex", color="#4CB391")
```
