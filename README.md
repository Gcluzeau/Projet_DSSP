# Projet_DSSP

This tool parses a PDB file, identifies secondary structure elements (helices and beta strands) using hydrogen bonding criteria, and compares the prediction with the DSSP reference using MDAnalysis.


### Parses backbone atoms from a PDB file.

### Detects hydrogen bonds using electrostatic energy approximation.

### Predicts:

Alpha helices (i → i+4)

3₁₀ helices (i → i+3)

π helices (i → i+5)

Beta strands (via beta bridges: parallel & antiparallel)

### Classifies each residue as:

H → Helix

E → Strand

L → Loop (default)

```bash
Hydrogen bonds (detected beta bridges):
  Antiparallel between ('A', 5) and ('A', 22)
  Antiparallel between ('A', 8) and ('A', 20)
  ...
Final secondary structure:
A1: L
A2: L
A3: L
```

### Compares custom results to DSSP-derived secondary structures.

```bash
Comparison with DSSP:
  Residues compared: XXX
  Exact matches: XXX
  Prediction accuracy: XX%
```

# Requirements

Download the yamal file
```bash
conda activate dssp_env
```

# Reference
Kabsch, W., & Sander, C. (1983). Dictionary of protein secondary structure: Pattern recognition of hydrogen-bonded and geometrical features. Biopolymers, 22(12), 2577–2637. https://doi.org/10.1002/bip.360221211