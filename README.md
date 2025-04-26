# Business_Analytics_Bootcamp_11


# 🧪 Multivariate A/B Testing - Advanced Analytics

Dive deep into the world of data-driven decision making by mastering the art and science of Multivariate A/B Testing. Learn how companies like **Google** optimize user experience with statistical rigor and machine learning.

---

## 📁 Repository Contents

| File Name                      | Description                                                        |
|-------------------------------|--------------------------------------------------------------------|
| `Multivariate_A_B_Testing.ipynb` | Interactive Python notebook exploring multivariate testing using real-world data |
| `ab_google.csv`               | Dataset simulating Google homepage variations and user engagement |
| `README.md`                   | This file – your guide to the project structure and key takeaways |

---

## 🧠 Game Plan for Multivariate A/B Testing

A/B testing is no longer about just comparing two variants.  
This project evolves your toolkit from traditional A/B testing to **Multivariate Testing (MVT)** — enabling simultaneous testing of multiple design elements and their interactions.

You’ll:
- Identify multiple variables impacting user engagement
- Use statistical modeling and machine learning to test combinations
- Derive insights from untested variants through predictive modeling

---

## 🕵️‍♂️ Case Study: Google's Homepage Experiment

We simulate and analyze an experiment similar to one Google ran on its homepage — testing changes in:

- 🔍 **Search Bar Shape**
- 🟠 **Search Button Design**
- 🎨 **Background Color**

Each user saw a unique combination. The dataset (`ab_google.csv`) helps us explore how subtle design tweaks can significantly impact **Session Duration**.

---

## 🔬 What is Multivariate A/B Testing (MVT)?

| A/B Test                        | Multivariate Test (MVT)                             |
|---------------------------------|-----------------------------------------------------|
| Tests one element at a time     | Tests multiple elements together                    |
| Simple to run                   | Complex due to interaction effects                  |
| Limited insight                 | Reveals combined impact of changes                  |

> MVT helps you find the **best-performing combination**, not just the best element.

---

## 🔧 Full Factorial & Partial Factorial Testing

- **Full Factorial**: Tests *all* possible combinations (e.g., 2×2×2 = 8 versions)
- **Partial Factorial**: Reduces testing effort using smart experimental designs (e.g., Taguchi methods)

✅ In this project, we use **full factorial design** to assess every combination of the three design elements.

---

## 📊 Exploratory Data Analysis (EDA)

We visualize and compare:

- 📈 Distribution of **Session Duration**
- 👥 Engagement across different **Search Bar**, **Button**, and **Background** styles
- 🔄 Frequency of each design combination

This helps detect outliers, skewness, and preliminary performance differences.

---

## 📈 Regression & Random Forest Modeling in Python

We use machine learning to model how design changes affect user behavior.

### Highlights:
- **Linear Regression**: Great for understanding influence of each variable
- **Random Forest**: Captures **non-linear patterns** and **interactions**

💡 *Pro Tip*: You don’t always need to add a constant to regression — especially in **tree-based models** like Random Forest!

---

## 🌲 Random Forest Parameter Tuning

We fine-tuned hyperparameters to boost model performance:

| Parameter           | Description                          |
|---------------------|--------------------------------------|
| `n_estimators`      | Number of trees                      |
| `max_depth`         | Maximum depth of each tree           |
| `min_samples_split` | Minimum samples to split a node      |
| `min_samples_leaf`  | Minimum samples at a leaf node       |

✅ Result: A **highly optimized model** to predict session durations.

---

## 🧪 Hypothesis Testing

We conducted:

- ✅ **ANOVA**: To check if combinations significantly influence session duration
- ✅ **Tukey’s HSD Test**: To identify which specific pairs differ significantly

### Result:
- **p-value = 0.000** → Statistically significant differences across design combinations  
- Many variations led to **significant improvements** in session duration

---

## 📌 Final Analysis: Inference & Visualizations

- 📊 Visualized **average session duration per variant** using bar plots
- 🔍 Compared **predicted vs. actual engagement**
- 🎯 Identified **top-performing and underperforming** combinations

---

## 🚀 Biggest Takeaway: Predicting Untested Variants

Even if a design combo wasn’t tested, ML models like **Random Forest** can **predict its performance**.

You're no longer limited to what was tested — now you can forecast the potential of unexplored variants and **prioritize smarter A/B testing**.

---

## 📸 Sneak Peek

| Combination                  | Avg. Session Duration (sec) |
|------------------------------|-----------------------------|
| Original_Original_Original   | 2990.86                     |
| Rectangle_Star_Original      | 3409.63                     |
| Rectangle_Star_Light Pink    | 3387.57                     |

---

## 🧠 Interpreting Results in Python

Use this helper function in the notebook to interpret p-values:

```python
def interpret_p_value(p):
    if p < 0.05:
        return "✔️ Reject Null Hypothesis"
    else:
        return "❌ Fail to Reject Null Hypothesis"


```

## 📚 Keywords for Discovery

  Multivariate AB Testing, Factorial Design, Google Homepage Experiment,
  Session Duration, Machine Learning, Random Forest, A/B Testing Analytics, User Behavior Modeling

## 🤝 Let’s Connect

If this repo adds value to your data science journey, consider giving it a ⭐️ or raising an issue for suggestions!

Made with 🧠 and 🐍 in Python


