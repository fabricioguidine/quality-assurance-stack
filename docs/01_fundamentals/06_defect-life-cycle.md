# Defect Life Cycle

The **Defect Life Cycle**, also known as the **Bug Life Cycle**, defines the various stages a defect goes through from the moment it is identified to its final closure. Understanding this cycle is essential for ensuring clear communication, effective resolution, and high software quality.

---

## 🐞 What is a Defect?

A **defect** is any deviation from the expected behavior of the software product. It may arise due to incorrect logic, missing requirements, or flaws in code implementation, design, or requirements.

---

## 🔄 Stages of the Defect Life Cycle

Below is a typical flow of stages in the defect life cycle:

1. **New**  
   The defect is discovered and logged by the tester. It awaits review and validation.

2. **Assigned**  
   The defect is reviewed and assigned to a developer or team for investigation.

3. **Open**  
   The developer has acknowledged the defect and started working on a fix.

4. **Fixed**  
   The developer resolves the defect by applying a fix and marks it as fixed.

5. **Retest**  
   The tester retests the application to confirm if the defect has been resolved correctly.

6. **Verified**  
   The tester verifies the fix and confirms the issue is resolved.

7. **Closed**  
   The defect is formally closed after successful verification.

8. **Reopened** *(optional)*  
   If the issue persists after the fix, the tester reopens the defect for further investigation.

9. **Rejected / Not a Defect / Duplicate / Deferred** *(alternate closures)*  
   Special statuses when a defect is invalid, already reported, or postponed.

---

## 🗂 Common Defect Statuses

| Status          | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| New             | Initial state when the defect is logged                                     |
| Assigned        | Assigned to a developer for resolution                                      |
| Open            | Developer is actively working on the issue                                 |
| Fixed           | Developer has implemented a fix                                             |
| Retest          | Awaiting tester to validate the fix                                         |
| Verified        | Tester confirms the defect is resolved                                      |
| Closed          | Final state when the defect is resolved and verified                        |
| Reopened        | The defect reoccurs even after a fix                                        |
| Rejected        | The defect is invalid or not reproducible                                   |
| Duplicate       | The defect is a duplicate of an existing issue                              |
| Deferred        | The defect is postponed for future releases (e.g., low priority)            |

---

## 🧠 Key Takeaways

- The **defect life cycle ensures traceability** and clarity in the resolution process.
- **Accurate status updates** are crucial for managing defects effectively.
- A well-defined defect life cycle supports **prioritization, triaging, and closure tracking**.
- **Collaboration between testers, developers, and project managers** ensures smooth defect resolution.

---

## 🧩 Best Practices

- Use a **centralized defect tracking tool** (e.g., JIRA, Bugzilla, Azure DevOps).
- **Clearly define severity and priority** to guide fix urgency.
- Attach **logs, screenshots, and steps to reproduce** for clarity.
- Keep the defect **status updated in real time** for accurate reporting.
- Perform **root cause analysis** on critical or recurring defects.

---

## 📊 Sample Workflow Diagram

```text
       +------+
       | New  |
       +--+---+
          |
          v
    +-----------+
    | Assigned  |
    +-----+-----+
          |
          v
       +------+
       | Open |
       +--+---+
          |
          v
       +-------+
       | Fixed |
       +---+---+
           |
           v
        +--------+
        | Retest |
        +---+----+
            |
   +--------+--------+
   |                 |
   v                 v
+--------+     +-----------+
| Verified|     | Reopened |
+----+---+     +-----+-----+
     |               |
     v               v
  +------+       +--------+
  | Closed|<---->| Fixed  |
  +------+       +--------+

Alternate paths:
  - Rejected
  - Duplicate
  - Deferred