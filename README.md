# Capstone_Project
This project is my first step toward combining chemistry + computation + AI in drug discovery, and I’m excited to keep building in this direction.  #ComputationalChemistry #DrugDiscovery #CADD #Bioinformatics #MolecularDocking #ADMET #ChemistryStudents #AIinScience #OpenScience
# 🧬 In Silico Drug Discovery Analysis of Ligands Against 7SFB

##  Overview
This project presents a complete in silico drug discovery workflow to evaluate the binding affinity and pharmacokinetic properties of selected ligands against the target protein **7SFB**. The study integrates drug-likeness screening, ADMET prediction, binding site identification, and molecular docking.

---

##  Objective
To identify potential drug candidates by analyzing ligand–protein interactions and evaluating pharmacokinetic properties using computational tools.

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

## ⚙️ Methodology (Workflow)

1. Protein Preparation (PyMOL)  
2. Ligand Preparation (PubChem + Open Babel)  
3. Drug-Likeness Screening (Lipinski Rule via SwissADME)  
4. ADMET Prediction (ADMETlab)  
5. Binding Site Prediction  
6. Molecular Docking (PyRx / AutoDock Vina)  
7. Visualization of interactions (PyMOL)  
8. Structure Prediction & Comparison (AlphaFold)

---

## 📊 Docking Results

| Ligand | Binding Energy (kcal/mol) |
|--------|--------------------------|
| 🟢 **Metformin** | **-6.7** |
| Diclofenac | -6.5 |
| Artemether | -6.3 |
| Lumefantrine | -6.1 |
| Caffeine | -6.0 |
| Ibuprofen | -5.6 |
| Naproxen | -5.5 |
| Acetaminophen | -5.3 |
| Aspirin | -4.8 |
| Theophylline | -4.7 |

---

## 🏆 Key Findings
- **Metformin** showed the strongest binding affinity (**−6.7 kcal/mol**)  
- Diclofenac and Artemether demonstrated strong interactions  
- Aspirin and Theophylline showed weaker binding  
- **9 out of 10 compounds satisfied Lipinski’s Rule of Five**  
- Lumefantrine showed 2 violations (potential bioavailability issues)

---


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

### 🔹Amino acid Residues in Binding Site 
<img width="1103" height="620" alt="image" src="https://github.com/user-attachments/assets/e334c799-7adf-426c-94c4-7990852aa361" />

*sequence of aminoacids detei=rmined by DoGSiteScorer*
---

### 🔹Alphafold3 AI prediction of the protein, and comparison with the cleaned protein
<img width="1236" height="695" alt="image" src="https://github.com/user-attachments/assets/65f8b9f3-5949-4e1e-ad87-8d5c079b3c33" />

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

## 📁 Project Structure


