## **Summary of Current Challenges and Next Steps**

### **A. Scenario Management**

1. The codebase was first built to run multiple assumptions in one go, but with new requirements coming in, it now needs some restructuring and retesting to stay flexible.

2. We could really use a clear **requirement document** outlining inputs, outputs, and logic for each scenario type — it would make future work more consistent.

3. The code is quite tied to the current assumption format. Making it more **modular** would help adapt faster when the structure changes.

4. There’s no dedicated module yet for managing scenarios, so most updates are done on demand. A defined structure would make things smoother and easier to maintain.

5. Having a **long-term design view** for scalability would help guide short-term fixes in a more structured way.

6. The way new scenarios plug into the **core calculations** could be clearer — documenting this link would prevent confusion later.

7. The scenario framework could also use a better structure for **testing and debugging**, so we can trace issues more easily.

---

### **B. Aggregation Logic**

1. Aggregation currently starts from a fixed valuation date. Making it a **configurable cutoff** would add flexibility for monthly updates.

2. There’s no standard process yet to **combine new and existing cashflows** — setting this up would help with accuracy and automation.

3. We need a way to calculate the **offset (in months)** for new business entries, to keep the cashflow alignment correct.

4. Parallel processing works well for reserve runs, but aggregation doesn’t fully use it yet. Integrating the two could save time.

5. The aggregation code will need to support more **fields and data volume** as the portfolio grows.

6. A setup for easier **testing and comparison** of aggregation results with incremental data would be helpful.

---

### **C. Overall**

Preparing a **Software Requirements Specification (SRS)** that clearly defines inputs, outputs, core logic, and dependencies would help align everyone on the same page. It’ll make development smoother now and more scalable later on.
