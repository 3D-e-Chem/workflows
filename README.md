# KNIME workflows

<!-- TOC -->

* [KNIME workflows](#knime-workflows)
* ["3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine" paper](#3d-e-chem-vm-structural-cheminformatics-research-infrastructure-in-a-freely-available-virtual-machine-paper)
  * [Chemdb4VS](#chemdb4vs)
  * [GPCR-kinase](#gpcr-kinase)
  * [GCRPDB_example](#gcrpdb_example)
  * [KLIFS_example](#klifs_example)
  * [KRIPO_bioisosteric_replacement_workflow](#kripo_bioisosteric_replacement_workflow)
  * [SyGMa-example](#sygma-example)

<!-- /TOC -->

[KNIME](http://www.knime.org) workflows developed in the
[3D-e-Chem project](https://3d-e-chem.github.io) using
[KNIME](http://www.knime.org) nodes developed in the
[3D-e-Chem project](https://3d-e-chem.github.io).

The workflows can be imported into KNIME by importing each \*knwf file.

The Pymol session files (\*.pse) can by opened with
[PyMol](https://github.com/NLeSC/Chemical-Analytics-Platform/wiki/Cheatsheet#applications).

# "3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine" paper

Below are the workflows mentioned in the
[3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine](https://doi.org/10.1021/acs.jcim.6b00686)
paper.

## Chemdb4VS

Customizable KNIME workflow to extract GPCR ligands from ChEMBL and preparation
for virtual screening.

## GPCR-kinase

Workflow to analyze the binding site similarity between all crystallized GPCRs
and kinases. PDB IDs are fetched through GPCRdb and KLIFS nodes, and the KRIPO
nodes are used to select similar binding pockets and to add ligand structures.

A Pymol session file called 'GPCR-kinase.pse' is stored next to this workflow.

## GCRPDB_example

This example fetches the residues, structures, protein-ligand interactions, and
mutations of the human beta-2 adrenoreceptor and its similarity to other beta-2
adrenoreceptors.

Data is fetched from http://gpcrdb.org website.

A Pymol session file called `aminergic_alignment.pse` with an aminergic
alignment is stored next to this workflow.

## KLIFS_example

Example for KLIFS nodes

This example performs interaction fingerprint analysis of human MAPK-ligand
complexes.

Data is fetched from http://klifs.vu-compmedchem.nl/

## KRIPO_bioisosteric_replacement_workflow

Bioisosteric replacement workflow using
[Kripo Knime nodes](https://github.com/3D-e-Chem/3D-e-Chem-VM/wiki/Software#kripodb).

## SyGMa-example

Example for the SyGMa metabolites node: predicting the metabolites of 5 (drug)
molecules.

A Pymol session file called `KRIPO_3rze_2aot.pse` with 3rze + 2aot Kripo
fragment alignment is stored next to this workflow.
