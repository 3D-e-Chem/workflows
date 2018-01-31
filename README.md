[KNIME](http://www.knime.org) workflows developed in the
[3D-e-Chem project](https://3d-e-chem.github.io) using KNIME nodes developed in
the [3D-e-Chem project](https://3d-e-chem.github.io).

<!-- TOC -->
* [*Submitted manuscript: GPCR chemical diversity*](#GPCR-chemical-diversity)
	* [GPCR chemical diversity assessment workflow](#GPCR-chemical-diversity-workflow)
* [*3D-e-Chem: Structural Cheminformatics Workflows for Computer-Aided Drug Discovery*](#3d-e-chem-structural-cheminformatics-workflows-for-computer-aided-drug-discovery)
  * [Fig. 2: Structure-based bioactivity data mapping of kinase inhibitors](#structure-based-bioactivity-data-mapping-of-kinase-inhibitors)
  * [Fig. 3: Scaffold replacements for kinase ligand design](#scaffold-replacements-for-kinase-ligand-design)
  * [Fig. 4: Ligand-based cross-reactivity prediction](#ligand-based-cross-reactivity-prediction)
  * [Fig. 5: Sequence-based ligand repurposing within a protein family](#sequence-based-ligand-repurposing-within-a-protein-family)
  * [Fig. 6: Structure-based GPCR-kinase cross-reactivity prediction](#structure-based-gpcr-kinase-cross-reactivity-prediction)
* [*3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine* paper](#3d-e-chem-vm-structural-cheminformatics-research-infrastructure-in-a-freely-available-virtual-machine-paper)
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
has been enabled, otherwise the 3D-e-Chem KNIME nodes will not be found automatically.

The Pymol session files (\*.pse) can by opened with
[PyMol](https://github.com/NLeSC/Chemical-Analytics-Platform/wiki/Cheatsheet#applications).

# *Submitted manuscript: GPCR chemical diversity*

Below is the workflow for a submitted manuscript regarding the chemical diversity of GPCR ligands.

## GPCR chemical diversity workflow

This extensive workflow compares all co-crystallized GPCR ligands (taken from [GPCRdb](http://www.gpcrdb.org)) to the known GPCR ligands (taken from [ChEMBL](https://www.ebi.ac.uk/chembl/)) and assesses: i) the number of ligands of a specific crystallized GPCR similar to its co-crystallized ligands, ii) the number of ligands of a specific crystallized GPCR similar to co-crystallized ligands of any GPCR, iii) the number of ligands of other GPCRs that are similar to the co-crystallized ligands of a specific receptor, iv) the number of ligands of other GPCR subfamilies that are similar to the co-crystallized ligands of a specific receptor.

* [KNIME workflow archive](GPCR_chemical_diversity/GPCR_chemical_diversity.knwf)

# *3D-e-Chem: Structural Cheminformatics Workflows for Computer-Aided Drug Discovery*

Below are the workflows shown in Figures 2 - 6 of
*3D-e-Chem: Structural Cheminformatics Workflows for Computer-Aided Drug Discovery* ([doi:10.1002/cmdc.201700754](http://onlinelibrary.wiley.com/doi/10.1002/cmdc.201700754/abstract)).

## Structure-based bioactivity data mapping of kinase inhibitors

Figure 2: Structure-based bioactivity data mapping workflow using KLIFS.

* [KNIME workflow archive](chemmedchem/Fig_2_Structural_bioactivity_mapping.knwf)

## Scaffold replacements for kinase ligand design

Figure 3: A workflow for the identification of potential scaffold replacements for kinase inhibitors while maintaining the protein-ligand interaction profile by combining protein-ligand interaction fingerprint (IFP) similarity with ligand-based dissimilarity (ECFP-4) analyses.

* [KNIME workflow archive](chemmedchem/Fig_3_Kinase_scaffold_hopping.knwf)

## Ligand-based cross-reactivity prediction

Figure 4: Ligand-based GPCR cross-reactivity prediction workflow that can also be used to derive ligand-based protein-protein (PP) assocations.

* [KNIME workflow archive](chemmedchem/Fig_4_PP_GPCR_cross-reactivity.knwf)
* [Optional tables for shortcuts during execution](chemmedchem/Fig_4_PP_GPCR_tables/)

## Sequence-based ligand repurposing within a protein family

Figure 5: Workflow for the identification of ligand repurposing possibilities using a sequence-based double entropy analysis (ss-TEA).

* [KNIME workflow archive](chemmedchem/Fig_5_ss-TEA_classA_GPCRs.knwf)

## Structure-based GPCR-kinase cross-reactivity prediction

Figure 6: A structure-based ligand repurposing workflow that searches for KripoDB pharmacophore similarities between GPCRs and kinases. 

* [KNIME workflow archive](chemmedchem/Fig_6_GPCR-kinase_cross-reactivity.knwf)

# *3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine* paper

Below are the workflows mentioned in the
[3D-e-Chem-VM: Structural Cheminformatics Research Infrastructure in a Freely Available Virtual Machine](https://doi.org/10.1021/acs.jcim.6b00686)
paper.

KNIME workflow archive files ending with `_small.knwf` are workflows with most nodes
collapsed into metanodes. The files ending with `_full.knwf` are workflows
mostly without metanodes.

## Chemdb4VS

* [KNIME workflow archive](jcim/Chemdb4VS_full.knwf)

Customizable KNIME workflow to extract GPCR ligands from ChEMBL and preparation
for virtual screening.

## GPCR-kinase

* [KNIME workflow archive](jcim/GPCR_kinase.knwf)

Workflow to analyze the binding site similarity between all crystallized GPCRs
and kinases. PDB IDs are fetched through GPCRdb and KLIFS nodes, and the KRIPO
nodes are used to select similar binding pockets and to add ligand structures.

A Pymol session file called [jcim/GPCR-kinase.pse](jcim/GPCR-kinase.pse) is
stored next to this workflow.

## GCRPDB_example

* [KNIME workflow archive](jcim/GPCRDB_example_full.knwf)

This example fetches the residues, structures, protein-ligand interactions, and
mutations of the human beta-2 adrenoreceptor and its similarity to other beta-2
adrenoreceptors.

Data is fetched from http://gpcrdb.org website.

A Pymol session file called
[jcim/aminergic_alignment.pse](jcim/aminergic_alignment.pse) with an aminergic
alignment is stored next to this workflow.

## KLIFS_example

* [KNIME workflow archive](jcim/KLIFS_example_workflow_full.knwf)

Example for KLIFS nodes

This example performs interaction fingerprint analysis of human MAPK-ligand
complexes.

Data is fetched from http://klifs.vu-compmedchem.nl/

## KRIPO_bioisosteric_replacement_workflow

* [KNIME workflow archive](jcim/KRIPO_bioisosteric_replacement_full.knwf)

Bioisosteric replacement workflow using
[Kripo Knime nodes](https://github.com/3D-e-Chem/3D-e-Chem-VM/wiki/Software#kripodb).

A Pymol session file called [jcim/KRIPO_3rze_2aot.pse](jcim/KRIPO_3rze_2aot.pse)
with 3rze + 2aot Kripo fragment alignment is stored next to this workflow.

## SyGMa-example

* [KNIME workflow archive](jcim/SyGMa-example.knwf)

Example for the SyGMa metabolites node: predicting the metabolites of 5 (drug)
molecules.
