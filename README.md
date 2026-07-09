# protein-homology-modeller
Automated MODELLER 10.8 script pipeline for 3D protein structure prediction of query sequence qseq1 via homology modeling. Features rigorous structural fold validation (GA341: 1.00000, DOPE: -41978.76) followed by global thermodynamic optimization via overall molecular energy minimization to resolve steric clashes.

In Silico Protein Structure Prediction and Optimization of qseq1
An automated, script-based computational biology pipeline for the 3D structure prediction, validation, and thermodynamic optimization of an uncharacterized query sequence (qseq1).  

**Project Overview**
The objective of this project is to model a raw primary amino acid sequence into a stable, native-like 3D conformation. By leveraging homology modeling pipelines and subsequent energy minimization, this workflow establishes a structurally sound model suitable for downstream bioinformatics applications, including Computer-Aided Drug Design (CADD), virtual screening, and molecular docking. 

**Methodology & Workflow**
1. Sequence AlignmentThe target query sequence (qseq1.ali) was aligned against a high-identity structural template (tseq1). The target-template alignment revealed an exceptional sequence identity of 99.703%, making it an ideal candidate for high-accuracy comparative modeling. 
2. Homology ModelingComparative 3D modeling was executed using python automation scripts via MODELLER 10.8. The backbone and side-chain coordinates were generated, outputting the final 3D structural file (qseq1.B99990005.pdb).  
3. Structural Validation & EvaluationThe generated theoretical model was rigorously evaluated using standard statistical potential scoring functions:  GA341 Score: 1.00000 (indicates a reliable fold topology with 100% confidence).  DOPE Score: -41978.76172 (Discrete Optimized Protein Energy potental).  Modeller Objective Function: 1465.5603. 
4. Energy MinimizationTo transition the theoretical model closer to its stable biological conformation, the structure underwent overall energy minimization. This critical optimization step relieved steric hindrances, eliminated atomic overlaps, relaxed side-chain clashes, and stabilized the global thermodynamic profile of the protein.
