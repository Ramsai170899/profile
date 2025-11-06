## **Project Challenges and Next Steps**

### **A. Scenario Management**

1. The codebase was originally built (around March 2025) to handle multiple assumptions within a single run. Since then, requirements have shifted, which means parts of the structure now need to be reworked and tested again to stay flexible for future changes.

2. It would really help to have a proper **requirement document** that clearly lays out the expected inputs, outputs, and business logic for each scenario — especially for areas like Stress Testing, ALM, and RBC. That kind of clarity upfront would save a lot of time later in testing and debugging.

3. Right now, the code is quite tied to the current assumption format. A more **modular setup** would make it easier to adapt when new assumption structures are introduced.

4. There isn’t a defined **module or architecture** for scenario management yet, so things have been built as and when needed. Having a proper structure would make it easier to scale and maintain.

5. A **long-term design view** could help guide short-term development decisions, so that quick fixes don’t conflict with the bigger vision for the framework.

6. The link between new scenario requirements and the existing core calculations could use more clarity — especially around how each scenario should plug into the current engine.

7. Finally, the **scenario execution framework** could benefit from a clearer structure. With defined layers for logging, debugging, and testing, we could make the whole process more consistent and efficient.

---

### **B. Aggregation Logic**

1. At the moment, the aggregation process starts from a fixed valuation date. It would be more flexible if this starting point could be a **configurable cutoff date**, so new business data can be added dynamically each month.

2. There’s no standard way yet to **merge new business cashflows** with the existing ones — whether that’s inception-based, year-to-date, or monthly. A clear approach here would simplify both execution and validation.

3. We also need logic to track how far each new business entry sits from the cutoff date — basically the **offset in months** — to keep the cashflow timeline accurate.

4. The parallel processing currently speeds up reserve calculations, but the same design doesn’t yet extend well to aggregation. Integrating the two could improve performance and reduce redundancy.

5. As the portfolio grows, the **aggregation code** will need to handle more data fields and columns. Expanding the technical design a bit now could save future effort.

6. Finally, it would help to have a setup that makes **testing and comparison of aggregation results** simpler — especially when adding incremental new business cashflows.

---

### **C. Summary**

Overall, preparing a **Software Requirements Specification (SRS)** that clearly documents input/output structures, key logic, dependencies, and design constraints will help align development efforts and make the system easier to maintain as it scales.

This would bring everyone on the same page about what’s expected — and give us a strong foundation for handling new requirements down the line.

---

Would you like me to make a **shorter version (1-page email summary)** of this — something you could send *directly to your manager* with a calm, collaborative tone (“Here’s a quick summary of the main challenges and improvement ideas I’ve noted”)?
