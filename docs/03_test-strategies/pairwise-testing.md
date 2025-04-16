Absolutely! Here's the clean, markdown-compliant version of **`pairwise-testing.md`**, ready for direct use in documentation, wikis, or any `.md` file without formatting issues.

---

# Pairwise Testing (All-Pairs Testing)

**Pairwise Testing** is a **black-box test design technique** that focuses on testing **all possible discrete combinations of input parameter pairs**. It helps reduce the number of test cases while still covering the most critical combinations.

> 🧠 Instead of testing all combinations, test every **pair** of input values at least once.

---

## 🎯 Purpose

- To minimize test cases while maximizing defect detection
- To uncover interaction bugs between input pairs
- To balance **test coverage and execution time**

---

## 📋 Why It Works

Most bugs are caused by **interactions between pairs of inputs**, not full combinations. Pairwise testing ensures that **each pair of values** is covered **at least once**, catching the majority of interaction defects.

---

## 🧪 Example

### Inputs:
- **OS:** Windows, macOS, Linux  
- **Browser:** Chrome, Firefox, Safari  
- **User Type:** Admin, Guest

**Full combinations:** 3 × 3 × 2 = **18 test cases**  
**Pairwise testing:** Can reduce to **~9 test cases** while still testing all pairs.

---

## ✅ Benefits

- Efficient: Reduces test case volume significantly
- Effective: Detects most defects caused by input interactions
- Scalable: Ideal for large input matrices

---

## ⚠️ Limitations

- Doesn’t cover **triplet or higher-level combinations**
- May miss bugs caused by **specific input sequences**
- Not suitable for **state-dependent systems**

---

## 🛠 Tools

| Tool           | Language       | Use Case                     |
|----------------|----------------|------------------------------|
| **PICT**       | Windows/CMD    | Pairwise input combination   |
| **AllPairs**   | Perl/Python    | CLI tool for all-pairs tests |
| **Pairwiser**  | Web            | Online test generator        |
| **TestersDesk**| Web            | Generate test cases visually |

---

## 🧠 Best Practices

- Identify **critical parameters** and their value sets
- Use pairwise as a **baseline**, not a replacement for other techniques
- Combine with **Boundary Value Analysis** for numeric inputs
- Track parameter combinations in a matrix to ensure pair coverage

---

## 📌 Summary

| Attribute           | Description                              |
|----------------------|------------------------------------------|
| Technique Type       | Black-box testing                        |
| Focus                | Input pair combinations                  |
| Ideal For            | Configurations, compatibility, scenarios |
| Reduces Test Cases   | While maintaining high fault detection   |

> “Don’t test everything — test every pair.”