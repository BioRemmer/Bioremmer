# BioremDatabase report: functional profile for plastic microbial biodegradation

## Introduction

To address the identification of a bacterial functional profile capable of degrading a specific plastic, we developed a pipeline named BioremDatabase.  Making use of a bioinformatic workflow, consisting of a pipeline that takes high-throughput sequencing data sets as input to perform a complete analysis that reports the biological capacity to participate in the biodegradation processes of plastics, identifying and classifying the bacterial abundance, as well as assessing the functional profile and locating the enzymes that degrade the different plastics. Users can generate insights by analyzing their data sets for the presence of potential plastic-degrading bacteria and enzymes, and thus design strategies to improve bioremediation of environments contaminated by different plastic waste.

![](https://drive.google.com/open?id=1pJl56dglmbe9iMpZPmsVWsTghidClJU2&usp=drive_copy)

## Installation of BioremDatabase
### Virtual machine
* Download VM [gdrive](https://drive.google.com/file/d/1z9mKT0Hhn0fSt_tcEsnuSFEelc6FSERV/view?usp=drive_link)

* Require
  * Virtual Box 7.0.8 [Platform packages] (https://www.virtualbox.org/wiki/Downloads)
  * Password: BioremDatabase

### Manual instalation
#### Databases
2003 COGs [COG](https://www.ncbi.nlm.nih.gov/research/cog-project/):
Tatusov, R. L., Galperin, M. Y., Natale, D. A. & Koonin, E. V. The COG database: A tool for genome-scale analysis of protein functions and evolution. Nucleic Acids Res. 28, 33–36 (2000).
There is copy in database folder

#### Mandatory
* __BLAST__
Camacho, C., Coulouris, G., Avagyan, V. et al. BLAST+: architecture and applications. BMC Bioinformatics 10, 421 (2009). 

* __FastQC 0.11.9__
Andrews, S. FastQC: a quality control tool for high throughput sequence data. (2010).

* __HMMER3 3.3.2__
Mistry, J., Finn, R. D., Eddy, S. R., Bateman, A. & Punta, M. Challenges in homology search: HMMER3 and convergent evolution of coiled-coil regions. Nucleic Acids Res. 41, (2013).

* __MEGA X__
Kumar S, Stecher G, Li M, Knyaz C, Tamura K. MEGA X: Molecular Evolutionary Genetics Analysis across Computing Platforms. Mol Biol Evol. 2018 Jun 1;35(6):1547-1549. doi: 10.1093/molbev/msy096. PMID: 29722887; PMCID: PMC5967553.

* __Metabat2 2.15__
Kang, D. D. et al. MetaBAT 2: An adaptive binning algorithm for robust and efficient genome reconstruction from metagenome assemblies. PeerJ 2019, 1–13 (2019)

* __METAXA2 2.2.3__
Bengtsson-Palme, J. et al. metaxa2: Improved identification and taxonomic classification of small and large subunit rRNA in metagenomic data. Mol. Ecol. Resour. 15, 1403–1414 (2015).

* __R programming__
R, C. T. R: A language and environment for statistical computing. R Found. Stat. Comput. Vienna, Au, (2021).

* __SPAdes 3.15.4__
Prjibelski, A., Antipov, D., Meleshko, D., Lapidus, A. & Korobeynikov, A. Using SPAdes De Novo Assembler. Curr. Protoc. Bioinforma. 70, 1–29 (2020).

* __Perl__
_Stajich et al, The Bioperl toolkit: Perl modules for the life sciences. Genome Res. 2002 Oct;12(10):1611-8._

* __Prokka 1.14.6__
Seemann, T. Prokka: Rapid prokaryotic genome annotation. Bioinformatics 30, 2068–2069 (2014).

* __Trimmomatic 0.39__
Bolger, A. M., Lohse, M. & Usadel, B. Trimmomatic: A flexible trimmer for Illumina sequence data. Bioinformatics 30, 2114–2120 (2014).

* __VAMPhyRE 1.0__
* Read theApplication Server [VAMPhyre](https://biomedbiotec.encb.ipn.mx/VAMPhyRE/)

## Workflow

## Invoking BioremDatabase
```
./pipeline_full.sh R1.fastq.gz R2.fastq.gz
```

## Output Files
| File | Description |
| --------- | ----------- |
| fastqc.html | quality control report |
| VGF_tree.nwk | Phylogenomic tree |
| rarefaction_out.level_6.txt | Detection of bacteria with 16S  |
| cog_frequencies.csv | Table of COGS frequenc |
| taxonomic_abundance.png | stacked barplot of COGS frequency|
| Orthologous_groups.png | barplot of COGs by Categories|

## Autor
* Jose Cano
*  Web: https://github.com/BioremDatabase/
