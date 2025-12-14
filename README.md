# Persuasive or Deceptive Visualization?
### DSC 106 Project @ UCSD

**Highlights the thin line between persuasive and deceptive visualizations by analyzing the relationship between race and police allegations.**

🔗 **[View Live Project Here](./notebooks/project2.ipynb)**

---

## 📊 Project Overview
Data doesn't lie, but charts can. This project investigates the thin line between **persuasion** (earnest storytelling) and **deception** (manipulative design). 

Using a dataset of civilian complaints against NYC police officers, we attempted to visualize two contradictory arguments:

1.  **For the Proposition (Earnest):** <br>
    *Argument:* Black individuals are disproportionately targeted by police misconduct.
    * *Technique:* We used **2020 Census Benchmarking** to show that while Black residents make up ~24% of NYC, they account for over 50% of complaints.
    * *Design Score:* Earnest (+2).

2.  **Against the Proposition (Deceptive):** <br>
    *Argument:* The system is fair; complaints are sustained at similar rates across all races.
    * *Technique:* We employed **Axis Truncation** (zooming the Y-axis to 70-78%) to exaggerate minor differences and suggest that White complainants actually see higher sustained rates than Black complainants.
    * *Design Score:* Mildly Deceptive (-1.5).

---

## ⚙️ Methodology & Design
The analysis focused on the "Ethical Visualization" framework, scoring design decisions based on their honesty.

* **Data Processing:** <br>Filtered ProPublica's dataset to remove "Unknown/Refused" ethnicities for accurate calculating.

* **Visual Rhetoric:**
    * *Normalization:* Comparing counts vs. proportions (Population Baseline).
    * *Scale Manipulation:* Using narrow axes to fabricate contrast.
    * *Ordering:* Sorting bars to subconsciously guide the viewer's conclusion.

---

## 🛠️ Tech Stack
* **Language:** Python 3
* **Libraries:**
    * `Pandas`: Data manipulation and cleaning.
    * `Matplotlib` / `Seaborn`: Visualization of demographic distributions and outcome rates.
    * `NumPy`: Statistical operations.

---

## 📂 Data Sources
| Dataset | Source | Description |
| :--- | :--- | :--- |
| **Civilian Complaints Against NYC Police Officers** | [ProPublica Datastore](https://projects.propublica.org/datastore/#civilian-complaints-against-new-york-city-police-officers) | Records of complaints filed with the Civilian Complaint Review Board (CCRB) from 1985 to 2020, including officer details, complainant demographics, and board dispositions. |
| **NYC Demographics** | [US Census Bureau](https://www.census.gov/) | Population benchmarks used to assess disproportionality in the complaint data. |