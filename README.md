# KNIME workflows

<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [KNIME workflows](#knime-workflows)
	- [Chemdb4VS](#chemdb4vs)
	- [GPCR-kinase](#gpcr-kinase)
	- [GCRPDB_example](#gcrpdbexample)
	- [KLIFS_example](#klifsexample)
	- [KRIPO_bioisosteric_replacement_workflow](#kripobioisostericreplacementworkflow)

<!-- /TOC -->

[KNIME](http://www.knime.org) workflows developed in the [3D-e-Chem project](https://3d-e-chem.github.io) using [KNIME](http://www.knime.org) nodes developed in the [3D-e-Chem project](https://3d-e-chem.github.io).

The workflows can be imported into KNIME by importing this repository as a KNIME workflow group.

The Pymol session files (*.pse) can by opened with [PyMol](https://github.com/NLeSC/Chemical-Analytics-Platform/wiki/Cheatsheet#applications).

The following workflows are available:

## Chemdb4VS

Customizable KNIME workflow to extract GPCR ligands from ChEMBL and preparation for virtual screening.

## GPCR-kinase

TODO

A Pymol session file called 'GPCR-kinase.pse' is stored next to this workflow.

## GCRPDB_example

This example fetches the residues, structures, protein-ligand interactions, and mutations of the human beta-2 adrenoreceptor and its similarity to other beta-2 adrenoreceptors.

Data is fetched from http://gpcrdb.org website.

A Pymol session file called `aminergic_alignment.pse` with an aminergic alignment is stored next to this workflow.

## KLIFS_example

Example for KLIFS nodes

This example performs interaction fingerprint analysis of human MAPK-ligand complexes.

Data is fetched from http://klifs.vu-compmedchem.nl/

## KRIPO_bioisosteric_replacement_workflow

Bioisosteric replacement workflow using [Kripo Knime nodes](https://github.com/3D-e-Chem/3D-e-Chem-VM/wiki/Software#kripodb).

A Pymol session file called `KRIPO_3rze_2aot.pse` with 3rze + 2aot Kripo fragment alignment is stored next to this workflow.
