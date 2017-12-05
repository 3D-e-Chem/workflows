[KNIME](http://www.knime.org) workflows developed in the
[3D-e-Chem project](https://3d-e-chem.github.io) using KNIME nodes developed in
the [3D-e-Chem project](https://3d-e-chem.github.io).

<!-- TOC -->

* ["3D-e-Chem: Structural Cheminformatics Workflows for Computer-Aided Drug Discovery"](#3d-e-chem-structural-cheminformatics-workflows-for-computer-aided-drug-discovery)
  * [Ligand-based cross-reactivity prediction](#ligand-based-cross-reactivity-prediction)
  * [Scaffold replacements for kinase ligand design](#scaffold-replacements-for-kinase-ligand-design)
  * [Sequence-based ligand repurposing within a protein family](#sequence-based-ligand-repurposing-within-a-protein-family)
  * [Structure-based bioactivity data mapping of kinase inhibitors](#structure-based-bioactivity-data-mapping-of-kinase-inhibitors)
  * [Structure-based GPCR-kinase cross-reactivity prediction](#structure-based-gpcr-kinase-cross-reactivity-prediction)
* ["3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine" paper](#3d-e-chem-vm-structural-cheminformatics-research-infrastructure-in-a-freely-available-virtual-machine-paper)
  * [Chemdb4VS](#chemdb4vs)
  * [GPCR-kinase](#gpcr-kinase)
  * [GCRPDB_example](#gcrpdb_example)
  * [KLIFS_example](#klifs_example)
  * [KRIPO_bioisosteric_replacement_workflow](#kripo_bioisosteric_replacement_workflow)
  * [SyGMa-example](#sygma-example)

<!-- /TOC -->

The 3D-e-Chem KNIME nodes are part of the
[Community contributions](https://www.knime.com/3d-e-chem-nodes-for-knime). The
community contribution software site is disabled by default, it can be enabled
by in KNIME menu going to File>Preferences>Install/Update>Available software
sites and checking the checkbox of the `Stable Community Contributions` software
site.

The workflows can be imported into KNIME by importing each KNIME archive file
(\*.knwf). Before importing make sure the community contribution software site
has been enabled, otherwise the 3D-e-Chem KNIME node will not be found.

The Pymol session files (\*.pse) can by opened with
[PyMol](https://github.com/NLeSC/Chemical-Analytics-Platform/wiki/Cheatsheet#applications).

# "3D-e-Chem: Structural Cheminformatics Workflows for Computer-Aided Drug Discovery"

## Ligand-based cross-reactivity prediction

## Scaffold replacements for kinase ligand design

## Sequence-based ligand repurposing within a protein family

## Structure-based bioactivity data mapping of kinase inhibitors

## Structure-based GPCR-kinase cross-reactivity prediction

# "3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine" paper

Below are the workflows mentioned in the
[3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine](https://doi.org/10.1021/acs.jcim.6b00686)
paper.

Workflow archive files ending with `_small.knwf` are workflows with most nodes
collapsed into metanodes. The files ending with `_full.knwf` are workflows
mostly without metanodes.

## Chemdb4VS

[Workflow archive](jcim/Chemdb4VS_full.knwf)

Customizable KNIME workflow to extract GPCR ligands from ChEMBL and preparation
for virtual screening.

## GPCR-kinase

[Workflow archive](jcim/GPCR_kinase.knwf)

Workflow to analyze the binding site similarity between all crystallized GPCRs
and kinases. PDB IDs are fetched through GPCRdb and KLIFS nodes, and the KRIPO
nodes are used to select similar binding pockets and to add ligand structures.

A Pymol session file called [jcim/GPCR-kinase.pse](jcim/GPCR-kinase.pse) is
stored next to this workflow.

## GCRPDB_example

[Workflow archive](jcim/GPCRDB_example_full.knwf)

This example fetches the residues, structures, protein-ligand interactions, and
mutations of the human beta-2 adrenoreceptor and its similarity to other beta-2
adrenoreceptors.

Data is fetched from http://gpcrdb.org website.

A Pymol session file called
[jcim/aminergic_alignment.pse](jcim/aminergic_alignment.pse) with an aminergic
alignment is stored next to this workflow.

## KLIFS_example

[Workflow archive](jcim/KLIFS_example_workflow_full.knwf)

Example for KLIFS nodes

This example performs interaction fingerprint analysis of human MAPK-ligand
complexes.

Data is fetched from http://klifs.vu-compmedchem.nl/

## KRIPO_bioisosteric_replacement_workflow

[Workflow archive](jcim/KRIPO_bioisosteric_replacement_full.knwf)

Bioisosteric replacement workflow using
[Kripo Knime nodes](https://github.com/3D-e-Chem/3D-e-Chem-VM/wiki/Software#kripodb).

A Pymol session file called [jcim/KRIPO_3rze_2aot.pse](jcim/KRIPO_3rze_2aot.pse)
with 3rze + 2aot Kripo fragment alignment is stored next to this workflow.

## SyGMa-example

[Workflow archive](jcim/SyGMa-example.knwf)

Example for the SyGMa metabolites node: predicting the metabolites of 5 (drug)
molecules.
