# Capstone_Project
This project is my first step toward combining chemistry + computation + AI in drug discovery, and I’m excited to keep building in this direction.  #ComputationalChemistry #DrugDiscovery #CADD #Bioinformatics #MolecularDocking #ADMET #ChemistryStudents #AIinScience #OpenScience
# 🧬 In Silico Drug Discovery Analysis of Ligands Against 7SFB


## 🏆 Key Result
**Metformin showed the highest binding affinity (-6.7 kcal/mol), supported by strong hydrogen bonding with key active site residues.**
## 🔬 Key Interaction
  
<p align="center">
   <img width="1536" height="1024" alt="metformin2" src="https://github.com/user-attachments/assets/bcae0a8a-fbb3-4c9f-b4a5-1c4c7f49c90a" />
</p>


----- 

## 📌 Project Overview
This project implements a **complete computational drug discovery pipeline** to evaluate ligand–protein interactions against the target protein **7SFB**.

The workflow integrates:
- Drug-likeness screening  
- ADMET profiling  
- Binding site identification  
- Molecular docking  
- Structural validation  

The objective is to identify **potential drug candidates based on both binding affinity and pharmacokinetic suitability**, rather than relying on docking alone.


<img width="1536" height="1024" alt="overview" src="https://github.com/user-attachments/assets/cab4ef3d-92ac-45fd-a2d4-50e0b651f7d7" />


---


## 🎯 Objectives
- Evaluate ligand binding affinity using molecular docking  
- Assess drug-likeness using Lipinski’s Rule of Five  
- Predict pharmacokinetic properties (ADMET)  
- Identify the most promising compound for further study  


---

## 🧪 Selected Ligands
- Aspirin  
- Ibuprofen  
- Acetaminophen  
- Naproxen  
- Diclofenac  
- Caffeine  
- Theophylline  
- Metformin  
- Artemether  
- Lumefantrine  

---


## ⚙️ Computational Workflow

| Step | Description | Tools |
|------|------------|------|
| Protein Preparation | Structure cleaning, hydrogen addition | PyMOL |
| Ligand Preparation | Format conversion & optimization | PubChem, Open Babel |
| Drug-Likeness | Lipinski Rule evaluation | SwissADME |
| ADMET Prediction | Pharmacokinetic profiling | ADMETlab |
| Binding Site | Active pocket identification | CASTp / PrankWeb |
| Docking | Binding affinity calculation | PyRx (AutoDock Vina) |
| Visualization | Interaction analysis | PyMOL |
| Structure Validation | Predicted vs experimental comparison | AlphaFold |

---


---
## 📊 Docking Results

| Rank | Ligand | Binding Energy (kcal/mol) |
|------|--------|--------------------------|
| 🥇 | **Metformin** | **-6.7** |
| 🥈 | Diclofenac | -6.5 |
| 🥉 | Artemether | -6.3 |
| 4 | Lumefantrine | -6.1 |
| 5 | Caffeine | -6.0 |
| 6 | Ibuprofen | -5.6 |
| 7 | Naproxen | -5.5 |
| 8 | Acetaminophen | -5.3 |
| 9 | Aspirin | -4.8 |
| 10 | Theophylline | -4.7 |


---

## 🧠 Key Insights

- **Metformin achieved the strongest interaction**, likely due to efficient hydrogen bonding within the active site  
- Diclofenac and Artemether showed **stable binding via hydrophobic and polar interactions**  
- Weak binders (Aspirin, Theophylline) indicate limited interaction capability  
- **9/10 compounds satisfied Lipinski’s Rule**, indicating good oral drug potential  
- Lumefantrine showed strong binding but **failed drug-likeness criteria**, highlighting the importance of multi-step evaluation  

-----


### 🔹 Docking Interaction (Best Ligand)
<img width="906" height="476" alt="image" src="https://github.com/user-attachments/assets/c7902bbd-f45e-42ee-851c-2b2e75484d7f" />
<img width="471" height="667" alt="image" src="https://github.com/user-attachments/assets/869b1348-1f66-40b6-b4ed-ecd5ec45b806" />

*Metformin shows a strong interaction within the active site of 7SFB.*

---

### 🔹 Binding Site Identification

<img width="624" height="702" alt="image" src="https://github.com/user-attachments/assets/ebe98ce2-28ce-475e-b3e7-1be5207ece92" />

*Predicted active binding pocket of the protein.*

---

### 🔹Docking: Binding site prediction 
<img width="674" height="379" alt="image" src="https://github.com/user-attachments/assets/74a1887d-86a1-4650-ad91-57d4b4020b26" />

*docking the targeted protein with selective ligands*

---

### 🔹Alphafold3 AI prediction of the protein, and comparison with the cleaned protein

*AI predicted protein structure aligned on the cleaned protein*

  ------

### 🔹Results


### Summary of Ligand Screening and Final Approval Status

| Compound Name | PubChem CID | Drug-likeliness (Lipinski) | Binding Energy (kcal/mol) | Safety & ADMET Balance | Final Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Diclofenac** | 3033 | Yes; 0 violation | -6.5 | High (Most balanced profile) | **Approved** |
| **Metformin** | 4091 | Yes; 0 violation | -6.7 | High (Strongest binding affinity) | **Approved** |
| **Acetaminophen** | 1983 | Yes; 0 violation | -5.3 | High (Very safe long-term use) | **Approved** |
| **Caffeine** | 2519 | Yes; 0 violation | -6.0 | Moderate (Excellent BBB access) | **Approved** |
| **Naproxen** | 156391 | Yes; 0 violation | -5.5 | Moderate (Stable profile) | **Approved** |
| **Ibuprofen** | 3672 | Yes; 0 violation | -5.6 | Moderate (High skin sensitization) | **Approved** |
| **Artemether** | 68911 | Yes; 0 violation | -6.3 | Low (Dangerously high skin risk) | **Not Approved** |
| **Lumefantrine** | 6437380 | No; 2 violations | -6.1 | Low (High skin risk/Poor absorption) | **Not Approved** |
| **Aspirin** | 2244 | Yes; 0 violation | -4.8 | Low (High eye corrosion risk) | **Not Approved** |
| **Theophylline** | 2153 | Yes; 0 violation | -4.7 | Low (High drug interaction risk) | **Not Approved** |

***

-----


#### Selection Criteria Notes:
* **Approved**: Compounds that passed the Lipinski Rule of Five and showed a favorable balance between binding affinity and ADMET safety profiles.
* **Not Approved**: Compounds excluded due to either multiple Lipinski violations (Lumefantrine) or critical safety concerns, such as high toxicity markers or significant drug-drug interaction risks.

---------

## 🧠 Tools & Technologies
- RCSB PDB
- PubCHEM
- PyMOL
- DoGSiteScorer  
- PyRx / AutoDock Vina  
- SwissADME  
- ADMETlab3.0
- Discovery Studio  
- AlphaFold  
- Open Babel  

---

## 📁 Repository Structure

Capstone-CADD-Project/
├── README.md
├── report/
│ └── report.pdf
├── methods/
│ └── methodology.md
├── data/
├── results/
├── figures/




---

## 📄 Detailed Report
A complete scientific report including methodology, results, and discussion is available:
report.pdf

---

## 🔬 Conclusion
This study demonstrates that **integrating docking with pharmacokinetic and drug-likeness analysis provides a more reliable framework for candidate selection**.

Among all compounds, **Metformin stands out as the most promising candidate**, balancing strong binding affinity with favorable drug-like properties.

---

## 📌 Author
**Rubab Fawad**  
BS Chemistry at QAU | Computational Drug Discovery | CADD Enthusiast



