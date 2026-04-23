# Capstone_Project
This project is my first step toward combining chemistry + computation + AI in drug discovery, and I’m excited to keep building in this direction.  #ComputationalChemistry #DrugDiscovery #CADD #Bioinformatics #MolecularDocking #ADMET #ChemistryStudents #AIinScience #OpenScience
# 🧬 In Silico Drug Discovery Analysis of Ligands Against 7SFB

## 📌 Overview
This project presents a complete in silico drug discovery workflow to evaluate the binding affinity and pharmacokinetic properties of selected ligands against the target protein **7SFB**. The study integrates drug-likeness screening, ADMET prediction, binding site identification, and molecular docking.

---

## 🎯 Objective
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

## 🖼️ Key Visualizations

### 🔹 Docking Interaction (Best Ligand)
![Docking Metformin](figures/docking/docking_metformin.png)

*Metformin showing strong interaction within the active site of 7SFB.*

---

### 🔹 Binding Site Identification
![Binding Site](figures/structure/binding_site.png)

*Predicted active binding pocket of the protein.*

---

### 🔹 ADMET Analysis
![ADMET](figures/analysis/admet_summary.png)

*Predicted pharmacokinetic properties of selected ligands.*

---

## 🧠 Tools & Technologies
- PyMOL  
- PyRx / AutoDock Vina  
- SwissADME  
- ADMETlab  
- AlphaFold  
- Open Babel  

---

## 📁 Project Structure
