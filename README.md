# Projet_DSSP

This tool parses a PDB file, identifies secondary structure elements (helices and beta strands) using hydrogen bonding criteria, and compares the prediction with the DSSP reference using MDAnalysis.

## Parses backbone atoms from a PDB file.

## Detects hydrogen bonds using electrostatic energy approximation.

## Predicts:

Alpha helices (i → i+4)

3₁₀ helices (i → i+3)

π helices (i → i+5)

Beta strands (via beta bridges: parallel & antiparallel)

## Classifies each residue as:

H → Helix

E → Strand

L → Loop (default)

## Compares custom results to DSSP-derived secondary structures.