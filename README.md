# 💫 BIOINFORMATICS for Drug Development

### Name: [Jay Arre Talosig](https://github.com/flexycode)  
### Subject & Section: [BIOF-101 COM231](https://www.geeksforgeeks.org/computer-organization-and-architecture-tutorials/)
### Professor: [Senku Ishigami](https://dr-stone.fandom.com/wiki/Senku_Ishigami)    
### No. of Units: [3 Units](https://www.youtube.com/watch?v=CKZdGfOdaUw)
### Prerequisite: [COMPUTER SCIENCE 2nd Year Level](https://www.pornhub.com/pornstar/lexi-lore)

## 🧠 Overview

Bioinformatics for Drug Development is a Python package that provides a simple pipeline for drug development using bioinformatics tools. This package includes tools for loading molecules, generating 2D drawings, calculating molecular descriptors, and performing virtual screening using a simple docking algorithm.

## 📋 Table of Contents

- [Introduction](#-introduction)
- [Installation](#-installation)
- [Usage](#-usage)
- [Functions](#-function)
- [Example](#-example) 
- [Documentation](#-documentation)
- [Acknowledgements](#-acknowledgements) 
- [License](#-license)
- [Changelogs](#-changelogs)

## 🛸 Introduction

<!-- Background github cover with short introduction down below -->
<img src="https://github.com/flexycode/CCOMPORG/blob/main/assets/asset2.jpg" />

Bioinformatics for drug development is an interdisciplinary field that combines biology, computer science, and data analysis to accelerate the discovery and optimization of new therapeutic agents. By leveraging large-scale biological data, such as genomic, proteomic, and metabolomic information, bioinformatics tools enable researchers to identify potential drug targets, understand disease mechanisms, and predict drug interactions and efficacy. This approach not only enhances the efficiency of the drug development process but also reduces costs and time, ultimately leading to more effective and personalized treatments for patients.

## Bioinformatics for Drug Development Course Outline

This 3-month course is designed to provide a comprehensive introduction to bioinformatics for drug development. The course will cover the basics of bioinformatics, molecular modeling, and virtual screening, as well as more advanced topics such as machine learning and data analysis.

#### Month 1: Introduction to Bioinformatics and Molecular Modeling

- Week 1: Introduction to bioinformatics and its role in drug development
- Week 2: Molecular modeling basics: atom types, bond orders, and molecular descriptors
- Week 3: Introduction to molecular modeling software: RDKit and PyMOL
- Week 4: Building and visualizing molecular models: SMILES, SDF, and PDB files

#### Month 2: Virtual Screening and Molecular Docking

- Week 5: Introduction to virtual screening and molecular docking
- Week 6: Molecular docking algorithms: DOCK, AutoDock, and Glide
- Week 7: Virtual screening workflows: preparing ligands and receptors
- Week 8: Analyzing molecular docking results: binding energies and docking scores

#### Month 3: Machine Learning and Data Analysis in Bioinformatics

- Week 9: Introduction to machine learning in bioinformatics
- Week 10: Supervised and unsupervised learning methods: regression, classification, and clustering
- Week 11: Data analysis and visualization: Matplotlib, Seaborn, and Plotly
- Week 12: Final project presentations: applying bioinformatics to drug development

### 🛸 Course Syllabus Table

| Week | Topic                                   | Description                                               | Assignments                                   |
|------|-----------------------------------------|-----------------------------------------------------------|-----------------------------------------------|
| 1    | Introduction to Bioinformatics          | Overview of bioinformatics and its role in drug development | Read chapters 1-2, complete assignment 1     |
| 2    | Molecular Modeling Basics               | Atom types, bond orders, and molecular descriptors        | Complete assignment 2, build a molecular model |
| 3    | Molecular Modeling Software             | Introduction to RDKit and PyMOL                           | Complete assignment 3, visualize a molecular model |
| 4    | Building and Visualizing Molecular Models| SMILES, SDF, and PDB files                                | Complete assignment 4, build and visualize a molecular model |
| 5    | Introduction to Virtual Screening       | Overview of virtual screening and molecular docking        | Read chapters 5-6, complete assignment 5     |
| 6    | Molecular Docking Algorithms            | DOCK, AutoDock, and Glide                                 | Complete assignment 6, dock a ligand to a receptor |
| 7    | Virtual Screening Workflows             | Preparing ligands and receptors                            | Complete assignment 7, prepare a virtual screening workflow |
| 8    | Analyzing Molecular Docking Results     | Binding energies and docking scores                        | Complete assignment 8, analyze molecular docking results |
| 9    | Introduction to Machine Learning        | Supervised and unsupervised learning methods              | Read chapters 9-10, complete assignment 9    |
| 10   | Data Analysis and Visualization         | Matplotlib, Seaborn, and Plotly                           | Complete assignment 10, visualize data       |
| 11   | Final Project Preparation               | Applying bioinformatics to drug development               | Complete assignment 11, prepare final project |
| 12   | Final Project Presentations             | Final project presentations                                | Present final project                         |


### 🛸 Current versions of the dependencies:

| Dependency      | Version   | Description                                   |
|------------------|-----------|-----------------------------------------------|
| RDKit            | 2022.03.1 | Molecular modeling and cheminformatics library |
| PyMOL           | 2.4.0    | Molecular visualization software               |
| Matplotlib       | 3.5.1    | Data visualization library                     |
| Seaborn          | 0.11.2   | Data visualization library                     |
| Plotly           | 5.6.0    | Data visualization library                     |
| Scikit-learn     | 1.0.2    | Machine learning library                       |
| Pandas           | 1.4.1    | Data analysis library                          |
| NumPy            | 1.22.3   | Numerical computing library                    |


## 💻 Installation

To install the package, run the following command:
```
pip install -r requirements.txt
```

This will install the required dependencies, including RDKit and Matplotlib.

## 👷 Usage

The package can be used to load molecules, generate 2D drawings, calculate molecular descriptors, and perform virtual screening. Here is an example of how to use the package:

##### Python
```
from bioinformatics import load_molecule, generate_drawing, calculate_descriptors, dock_molecule

# Load a sample molecule
smiles = 'CC(=O)Nc1ccc(cc1)S(=O)(=O)N'
mol = load_molecule(smiles)

# Generate a 2D drawing of the molecule
drawing = generate_drawing(mol)

# Calculate molecular descriptors
descriptors = calculate_descriptors(mol)

# Perform virtual screening using a simple docking algorithm
target_smiles = 'CN(c1ccc(cc1)C(=O)N)S(=O)(=O)=O'
target_mol = load_molecule(target_smiles)
score = dock_molecule(mol, target_mol)
```

## ✨ Function

The package includes the following functions:
- load_molecule(smiles): Loads a molecule from a SMILES string.
- generate_drawing(mol): Generates a 2D drawing of a molecule.
- calculate_descriptors(mol): Calculates molecular descriptors for a molecule.
- dock_molecule(mol, target): Performs virtual screening using a simple docking algorithm.

## 🧊 Example

The package includes an example script that demonstrates how to use the functions:

##### Python
```
# example.py
from bioinformatics import load_molecule, generate_drawing, calculate_descriptors, dock_molecule

# Load a sample molecule
smiles = 'CC(=O)Nc1ccc(cc1)S(=O)(=O)N'
mol = load_molecule(smiles)

# Generate a 2D drawing of the molecule
drawing = generate_drawing(mol)

# Calculate molecular descriptors
descriptors = calculate_descriptors(mol)

# Perform virtual screening using a simple docking algorithm
target_smiles = 'CN(c1ccc(cc1)C(=O)N)S(=O)(=O)=O'
target_mol = load_molecule(target_smiles)
score = dock_molecule(mol, target_mol)

print('Molecular weight:', descriptors['mol_wt'])
print('Docking score:', score)
```

## 📜 Documentation

The package includes documentation for each function, including usage examples and descriptions of the parameters and return values.

```
Coming Soon
```

## 💻 Technology Stacks

#### ✨ Tools
- VSCode
- Pycharm
- GoogleColab
- Python
- Common sense
- Datashit set
- Kaggle

#### ✨ dependencies

- rdkit
- matplotlib

## 🔑 License   

The package is licensed under the MIT license. See the LICENSE file for details.

[Artificial Ledger Technology](https://github.com/Artificial-Ledger-Technology) grants permission to students of the National University of Manila to use, modify, and distribute this project for educational purposes within the scope of their coursework and assignments.

### Usage 

- You may use this project as a reference or learning material for your studies at the National University of Manila.
- You may modify the project to suit your educational needs and requirements.
- You may share the project with your fellow students or instructors for educational purposes.

### Restrictions

- You may not use this project for commercial purposes.
- You may not redistribute or publish this project outside the National University of Manila without explicit permission.

## Disclaimer

This project is provided "as is" without warranty of any kind, express or implied. The National University of Manila and the project contributors disclaim any liability or responsibility for any direct, indirect, incidental, special, exemplary, or consequential damages arising out of the use or misuse of this project.

# 🔭 Acknowledgements   

### ✨ Youtube University 

#### ✨ Youtube Channel: 
- [BioTech Whisperer](https://www.youtube.com/watch?v=CKZdGfOdaUw)
- Comming Soon
- [Johnny Sins](https://www.pornhub.com/pornstar/johnny-sins)

# 📫 Changelogs
```
## [0.0.0] - 2025-02-25     
### Added  
- ✨ Create Repository for BioInformatics for Drug Development
- ✨ Create Documentation
- ✨ Create Course Table Syllabus

## [0.0.1] - 2025-02-TBA     
### Added  
- ✨ Coming Soon
- ✨ Coming Soon

## [0.0.1] - 2025-03-TBA     
### Added  
- ✨ Coming Soon
- ✨ Coming Soon

🧊 BIOINFORMATICS 101
```

<!-- Introduction Pannel button link, it will redirect to the top -->
#### [Back to Table of Content](#-introduction)

<!-- End point line insert Thanks for visiting enjoy your day, feel free to modify this  -->
---
<p align="center">
<img src="https://readme-typing-svg.demolab.com/?lines=Thanks+For+Visiting+Enjoy+Your+Day+~!;" alt="mystreak"/>
</p>

<!-- Genshin Impact -->
<div align="center">
<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZnkxNDgzYjhwNTNwZnltNnltZXM5ZnFwNWl3M2VuYmJtdXY0YTlvayZlcD12MV9zdGlja2Vyc19zZWFyY2gmY3Q9cw/rMelA7MZWTeGoJCi0f/giphy.gif" width="300">
</div>

<!-- End point line insert Comeback again next time, feel free to modify this  -->
<p align="center">
<img src="https://readme-typing-svg.demolab.com/?lines=💎💎Come+Back+Again+next+time💎💎" alt="mystreak"/>
</p>

</p>
    
<br>
<!-- End point insert background effect line of sight color red -->

