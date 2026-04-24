# Capstone_Project
This project is my first step toward combining chemistry, computation, and AI in drug discovery, and I’m excited to keep building in this direction.  #ComputationalChemistry #DrugDiscovery #CADD #Bioinformatics #MolecularDocking #ADMET #ChemistryStudents #AIinScience #OpenScience

---
# 🧬 In Silico Drug Discovery Analysis of Ligands Against 7SFB
Protein 7SFB, also known as Main Protease, is an essential constructive part of the COVID-19 virus without which the virus is rendered replication-incompetent. This protein is the master key to the virus's survival. The selection of 7SFB is a strategic choice because it represents the Main Protease (Mpro/3CLpro) of the SARS-CoV-2 virus. It is a proven, high-impact target where computational modeling can yield fast, life-saving results without the immediate need for a high-containment wet lab.

## 🏆 Key Finding
**Metformin exhibited the highest binding affinity (-6.7 kcal/mol), driven by strong hydrogen bonding with active site residues.**

## 🔬Metformin Docking
  <p align="center">
    <img width="1536" height="1024" alt="metformin2" src="https://github.com/user-attachments/assets/bcae0a8a-fbb3-4c9f-b4a5-1c4c7f49c90a" />

</p>

## 🔬 Binding Interaction Insights

Metformin exhibits strong binding within the active site through multiple hydrogen bonds and polar interactions:

- Hydrogen bonding with ASN A:151 and THR A:111 stabilizes ligand positioning  
- ASP A:295 contributes to the electrostatic interaction  
- Polar functional groups enhance binding affinity  
- A minor unfavorable donor interaction is observed, but does not significantly impact overall stability  

These interactions explain the superior docking score observed for Metformin.

  
----- 

## 📌 Project Overview
This project aims to implement a **complete computational drug discovery pipeline** to evaluate ligand–protein interactions against the target protein **7SFB**.

The workflow integrates:

**Ligand Selection → Druglikeness Screening → Protein Preparation → Docking → ADMET → AI Structure Validation**

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

## Docking Results

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

## 🧠 Key Insights

- **Metformin achieved the strongest interaction**, likely due to efficient hydrogen bonding within the active site  
- Diclofenac and Artemether showed **stable binding via hydrophobic and polar interactions**  
- Weak binders (Aspirin, Theophylline) indicate limited interaction capability  
- **9/10 compounds satisfied Lipinski’s Rule**, indicating good oral drug potential  
- Lumefantrine showed strong binding but **failed drug-likeness criteria**, highlighting the importance of multi-step evaluation  

-----


### 🔹 Docking Interaction (Best Ligand)

<img width="471" height="667" alt="image" src="https://github.com/user-attachments/assets/869b1348-1f66-40b6-b4ed-ecd5ec45b806" />

*Metformin shows a strong interaction within the active site of 7SFB. The figure shows the bonding of the ligand with the amino acids, showing the interactions of Metformin to the amino acids ASN151, THR111, ASP295, and GLN110 of the protein.*

<img width="906" height="476" alt="image" src="https://github.com/user-attachments/assets/83313845-5807-4b07-bc89-b1886560df29" />

- Metformin forms multiple hydrogen bonds with ASN A:151 and THR A:111
- ASP A:295 contributes to electrostatic stabilization
- Polar interactions enhance binding affinity
- Minor unfavorable donor interaction observed, but it does not significantly affect stability
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
| **Artemether** | 68911 | Yes; 0 violation | -6.3 | Low 🚩(Dangerously high skin risk) | **Not Approved** |
| **Lumefantrine** | 6437380 | No; 2 violations 🚫| -6.1 | Low 🚩(High skin risk/Poor absorption)| **Not Approved** |
| **Aspirin** | 2244 | Yes; 0 violation | -4.8 | Low 🚩(High eye corrosion risk)| **Not Approved** |
| **Theophylline** | 2153 | Yes; 0 violation | -4.7 | Low 🚩(High drug interaction risk) | **Not Approved** |

***

-----


#### Selection Criteria Notes:
* **Approved**: Compounds that passed the Lipinski Rule of Five and showed a favorable balance between binding affinity and ADMET safety profiles.
* **Not Approved**: Compounds excluded due to either multiple Lipinski violations (Lumefantrine) or critical safety concerns, such as high toxicity markers or significant drug-drug interaction risks.

---------


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

📄 Full Report: report.pdf
---


---

## 🧠 Tools & Technologies
- RCSB PDB
- PubCHEM
- PyMOL
- DoGSiteScorer  
- PyRx / AutoDock Vina / Open Babel 
- SwissADME  
- ADMETlab3.0
- Discovery Studio  
- AlphaFold  
   
---
## ⚙️ Workflow

Ligand Selection → Druglikeness Screening → Protein Preparation → Docking → ADMET → AI Structure Validation
| Step | Description | Tools |
|------|------------|------|
| Protein Preparation | Structure cleaning, hydrogen addition | PyMOL |
| Ligand Preparation | Format conversion & optimization | PubChem, Open Babel |
| Drug-Likeness | Lipinski Rule evaluation | SwissADME |
| ADMET Prediction | Pharmacokinetic profiling | ADMETlab |
| Binding Site | Active pocket identification | DoGSiteScorer |
| Docking | Binding affinity calculation | PyRx (AutoDock Vina) |
| Visualization | Interaction analysis | PyMOL |
| Structure Validation | Predicted vs experimental comparison | AlphaFold |

-----


## Conclusion

Metformin emerged as the most promising candidate due to its strong binding affinity and stable interactions with key residues at the active site. This study demonstrates the importance of integrating docking, drug-likeness, and ADMET analysis for reliable candidate selection.

---

## 📌 Author
**Rubab Fawad**  
BS Chemistry at QAU | Computational Drug Discovery | CADD Enthusiast



