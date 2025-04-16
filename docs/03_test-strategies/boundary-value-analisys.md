Absolutely! Here's the clean and ready-to-use markdown content for **`boundary-value-analysis.md`**, designed to be copy-pasted directly into your `.md` file with no formatting issues.

---

# Boundary Value Analysis (BVA)

**Boundary Value Analysis (BVA)** is a **black-box test design technique** that focuses on testing the **edges or boundaries** of input ranges, where defects are more likely to occur.

> 🧠 Most bugs live at the boundaries, not in the middle.

---

## 🎯 Purpose

- To identify errors that occur at the **minimum, maximum, just inside, and just outside** input boundaries.
- To reduce the number of test cases while maintaining high effectiveness.

---

## 📦 How It Works

For any input range **[min, max]**, test cases are designed for:

- Minimum value
- Just above minimum (min + 1)
- Just below minimum (min - 1)
- Maximum value
- Just below maximum (max - 1)
- Just above maximum (max + 1)

---

## 🧪 Example

Suppose a form accepts age between **18 and 60**:

| Test Input   | Reason                   |
|--------------|--------------------------|
| 17           | Just below minimum       |
| 18           | Minimum valid            |
| 19           | Just above minimum       |
| 59           | Just below maximum       |
| 60           | Maximum valid            |
| 61           | Just above maximum       |

---

## ✅ Benefits

- High defect detection rate at a low cost
- Simple to understand and apply
- Works well for **numeric** and **range-based inputs**

---

## ⚠️ Limitations

- Not effective for complex input conditions or logical rules
- Only focuses on **boundaries**, may miss errors in mid-range values
- Less applicable for **non-continuous** input types

---

## 🔁 When to Use BVA

| Scenario                            | Apply BVA? |
|-------------------------------------|------------|
| Numeric range validation            | ✅          |
| Date, time, age fields              | ✅          |
| Dropdown menus or discrete options  | ❌          |
| Text format or regex validation     | ❌          |

---

## 🧠 Best Practices

- Use BVA **alongside** Equivalence Partitioning
- Always test **invalid boundaries** (e.g., min-1, max+1)
- Include **edge cases** in your regression suite

---

## 📌 Summary

| Aspect              | Value                                  |
|---------------------|----------------------------------------|
| Technique type      | Black-box                              |
| Focus               | Input boundaries                       |
| Test cases          | min, min±1, max, max±1                  |
| Best for            | Numerical and input field validation   |

> “If you’re not testing the edges, you’re missing where most bugs hide.”