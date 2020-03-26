# ISA-Tab annotation for the  "SARS-CoV-2 infected host cell proteomics reveal potential therapy targets" publication

This is part of an effort to (re-)annotate

https://dx.doi.org/10.21203/rs.3.rs-17218/v1

## Proteomics data

Available from PRIDE at [https://www.ebi.ac.uk/pride/archive/projects/PXD017710](https://www.ebi.ac.uk/pride/archive/projects/PXD017710)
and [MassIVE/CCMS Maestro+MSstats reanalysis of MSV000085096 / PXD017710](https://massive.ucsd.edu/ProteoSAFe/result.jsp?task=334df9b4f1af4501bca0a2aa63278a7d&view=display_metadata_results&file=f.RMSV000000308%2F2020-03-22_nuno_334df9b4%2Fmetadata%2FMSV000085096_SARS-CoV-2_proteome_translatome.csv#%7B%22table_sort_history%22%3A%22_dyn_%23Condition_asc%22%7D)

## ISA-Tab


The formatting and reannotation are based on information extracted from:
- the original publication
- the supplementary tables available from the publishers site
- the 'filtered-results.csv' helper file as supplied to @sneumann during the [HUPO-PSI]()


The default ISA configuration from https://isa-tools.org/format/configurations/index.html was used for validation.

### Task performed:

* initial structure of the study design in ISA format:

* linkage of Proteome and Translatome data (supplementary material) to ISA assay tables (via Derived Data File)

* ontology markup for:
	* declaration of independant variables as ISA Study Factors:{biological agent, dose, timepoint,replicate} ->OBI
	* Taxonomic information (host cells and virus) -> NCBITaxonomy
	* Cell line: CaCo-2 cells -> Cell Line Ontology
	* Disease: Colon Cancer -> Human Phenotype Ontology
	* MS specific aspect (TMT reagent, instrument ... ) -> PSI-MS


### unresolved curatorial issues:
 1. ambiguities related to Tandem Mass Tag labeling protococol
    - the publication mentions TMT11 (see Figure 2 in https://www.researchsquare.com/article/rs-17218/v1)
    - the information available from PRIDE mentions TMT6 (https://www.ebi.ac.uk/pride/archive/projects/PXD017710)
    This may require another round of annotation on the TMT agents and fractions in the ISA a_assay representation


 2. SARS-Cov2 isolate: no clear NCBI Taxonomic anchoring and unclear origin.



----

## FAIRification Objectives, Inputs and Outputs

| Actions.Objectives.Tasks  | Input | Output  |
| :------------- | :------------- | :------------- |
| [validation](http://edamontology.org/operation_2428)  | [Investigation Study Assay (ISA)](https://fairsharing.org/FAIRsharing.53gp75)  | [report](http://edamontology.org/data_2048)  |
| [formatting](http://edamontology.org/operation_0335)  | [tab delimited file]() |[Investigation Study Assay (ISA)](https://fairsharing.org/FAIRsharing.53gp75)|
| [formatting](http://edamontology.org/operation_3438)  | [Waters MS format]()  | [mzML](https://fairsharing.org/FAIRsharing.26dmba)  |
| [text annotation](http://edamontology.org/operation_3778)  | [CLO](https://fairsharing.org/FAIRsharing.4dvtcz)  | [annotated text](http://edamontology.org/data_3779)  |
| [text annotation](http://edamontology.org/operation_3778)  | [OBI](https://fairsharing.org/FAIRsharing.284e1z)  | [annotated text](http://edamontology.org/data_3779)  |
| [text annotation](http://edamontology.org/operation_3778)  | [NCBI taxonomy](https://fairsharing.org/FAIRsharing.fj07xj)  | [annotated text](http://edamontology.org/data_3779)  |
| [text annotation](http://edamontology.org/operation_3778)  | [HP](https://fairsharing.org/FAIRsharing.kbtt7f)  | [annotated text](http://edamontology.org/data_3779)  |
| [text annotation](http://edamontology.org/operation_3778)  | [MS](https://fairsharing.org/FAIRsharing.sxh2dp)  | [annotated text](http://edamontology.org/data_3779)  |


## Table of Data Standards

| Data Formats  | Terminologies | Models  |
| :------------- | :------------- | :------------- |
| [Investigation Study Assay (ISA)](https://fairsharing.org/FAIRsharing.53gp75)   | [CLO](https://fairsharing.org/FAIRsharing.4dvtcz) |   |
| [mzML](https://fairsharing.org/FAIRsharing.26dmba)  | [OBI](https://fairsharing.org/FAIRsharing.284e1z)  |   |
| | [NCBI taxonomy](https://fairsharing.org/FAIRsharing.fj07xj) |  |
| | [HP](https://fairsharing.org/FAIRsharing.kbtt7f)  |   |
| | [MS](https://fairsharing.org/FAIRsharing.sxh2dp)  |   |



## Authors:

| Name | Affiliation  | orcid | CrediT role  |
| :------------- | :------------- | :------------- |:------------- |
| Steffen Neumann |  IPB-Halle | [0000-0002-7899-7192](https://orcid.org/orcid.org/0000-0002-7899-7192)|  Writing - First Draft|
| Philippe Rocca-Serra | Data Readiness Group, Department of Engineering Science, University of Oxford, | [0000-0001-9853-5668](https://orcid.org/orcid.org/0000-0001-9853-5668) | Writing - Review|

___


## License:

<a href="https://creativecommons.org/licenses/by/4.0/"><img src="https://mirrors.creativecommons.org/presskit/buttons/80x15/png/by-sa.png" height="20"/></a>
