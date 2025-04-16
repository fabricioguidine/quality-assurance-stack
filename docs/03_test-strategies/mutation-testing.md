Thanks for flagging that! Here's a **clean and properly formatted markdown version** of `mutation-testing.md` with **no nested code blocks**, making it safe for copy-paste into any `.md` file or markdown renderer:

---

# Mutation Testing

**Mutation Testing** is a technique used to evaluate the **effectiveness of your test suite** by introducing small changes (called _mutants_) into the code and checking whether the tests catch them.

If your tests **fail** when a mutant is introduced → ✅ The test is effective.  
If your tests **pass** despite the mutant → ❌ The test is weak or missing.

---

## 🎯 Purpose

- Measure the **quality and completeness** of your unit tests.
- Identify **untested logic paths** or false positives.
- Encourage writing **stronger, more meaningful tests**.

---

## 🧬 How Mutation Testing Works

1. A mutation tool makes small changes to your code.
2. It runs your existing test suite against the modified code.
3. If a test fails → the mutant is "killed".
4. If no test fails → the mutant "survives".

---

## 🧪 Example

### Original code:
```python
def is_even(n):
    return n % 2 == 0
```

### Mutated version:
```python
def is_even(n):
    return n % 2 != 0  # Mutant introduced
```

If your tests don't fail when this logic is reversed, then they didn’t catch the mutant — meaning the test suite is inadequate.

---

## 📊 Mutation Score

Mutation testing tools often report a **mutation score**:

```
Mutation Score = (Killed Mutants / Total Mutants) × 100%
```

- **High score** → strong test coverage and logic validation
- **Low score** → potential gaps in test quality

---

## 🛠 Tools

- **Python:** MutPy, Cosmic Ray
- **Java:** PIT (Pitest)
- **JavaScript:** Stryker
- **.NET:** Stryker.NET

---

## ✅ Benefits

- Reveals weak or missing test cases
- Improves test suite robustness
- Encourages better unit testing practices

---

## ⚠️ Limitations

- Can be **slow** on large codebases
- May produce **equivalent mutants** (which don’t affect behavior but are hard to detect)
- Requires a solid test environment setup

---

## 🧠 Best Practices

- Use mutation testing **alongside** code coverage tools (not as a replacement)
- Focus mutation testing on **critical or high-risk modules**
- Run in **CI pipelines or pre-release gates** for test quality audits

---

## ✅ Summary

| Metric             | Description                                 |
|--------------------|---------------------------------------------|
| Mutant             | Small code change used to challenge tests   |
| Killed Mutant      | Detected and failed by a test               |
| Survived Mutant    | Undetected and passed as normal             |
| Mutation Score     | % of mutants caught by the test suite       |

> 🧪 Mutation testing doesn’t just ask “do you test?” — it asks “do your tests matter?”