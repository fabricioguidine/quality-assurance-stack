# Principles of Testing

The **Principles of Software Testing** are foundational guidelines that help ensure testing is efficient, effective, and purposeful. These principles are recognized by ISTQB and widely used in QA practices.

---

## 1. Testing Shows Presence of Defects
Testing can reveal that defects exist, but it can **never prove that there are no defects**. The goal is to reduce the risk of issues, not to confirm perfection.

> 💡 "Absence of evidence is not evidence of absence."

---

## 2. Exhaustive Testing is Impossible
It’s impractical to test every possible input and path. Instead, testing should be **risk-based and prioritized**, using techniques like boundary-value analysis and equivalence partitioning.

---

## 3. Early Testing Saves Time and Money
Testing activities should start **as early as possible** in the SDLC to catch defects when they are cheaper to fix (e.g., during requirements or design phases).

---

## 4. Defect Clustering
A small number of modules often contain the majority of defects. Identifying and focusing on these **high-risk areas** improves testing effectiveness.

> 📊 80/20 Rule (Pareto Principle): ~80% of bugs are found in ~20% of the code.

---

## 5. Pesticide Paradox
Running the **same set of tests repeatedly** will eventually stop finding new bugs. To continue being effective, tests must be **regularly reviewed and updated**.

---

## 6. Testing is Context-Dependent
Testing strategies and approaches depend on the **type of application**, **domain**, and **business risks** involved. What works for a banking app may not suit a game or an IoT device.

---

## 7. Absence-of-Errors Fallacy
Just because a system has **no known defects** does **not** mean it is usable or meets business needs. Testing must validate **correctness, completeness, and user expectations**.

---

## Summary Table

| Principle                       | Key Idea                                         |
|--------------------------------|--------------------------------------------------|
| 1. Defects are always possible | Testing proves bugs exist, not that they don’t  |
| 2. Not everything can be tested| Use smart, focused testing                       |
| 3. Start early                 | Catch issues before they get expensive           |
| 4. Defects cluster             | Focus on high-risk areas                         |
| 5. Update your tests           | Avoid the pesticide paradox                      |
| 6. Adapt to context            | No one-size-fits-all strategy                    |
| 7. More than no bugs           | Ensure the system actually meets the needs       |

---

**References**  
- ISTQB Foundation Level Syllabus  
- IEEE 829 Standard  
- ISO/IEC/IEEE 29119