# Biobank-scale genetic characterization of Alzheimer’s disease and related dementias across diverse populations
## Summary
This is the online repository for the original article titled "Biobank-scale genetic characterization of Alzheimer’s disease and related dementias across diverse populations." This study aims to conduct genetic characterization of key genes associated with dementia across different ancestry populations using the largest biobank-scale datasets, including AllofUs, UK Biobank, ADSP, AMP PDRD, and 100KGP.
### Data Statement 
* The All of Us genomic data are available under restricted access for human subject data. Access can be obtained by following the instructions under the All of Us workbench
* Primary data from the 100KGP, which are held in a secure Research Environment, are available to registered users. Please see https://www.genomicsengland.co.uk/about-gecip/for-gecip-members/data-and-data-access for further information

  # Repository Orientation 
- The `analyses/` directory includes all analyses discussed in the manuscript
  
```
THIS_REPO
├── README.md
└── analyses
    ├── UKB
    │   └── 00_UKB.ipynb
    ├── AMP PDRD
    │   └── 00_AMP PDRD.ipynb
    │   └── 01_AMP PDRD.ipynb
    │   └── 02_AMP PDRD.ipynb
    ├── AllOfUs
    │   ├── 00_AoU.ipynb
    │   └── 01_AoU.ipynb
    │   └── 02_AoU.ipynb
    │   └── 03_AoU.ipynb
    └── ADSP
        ├── 00_ADSP.ipynb
        └── 01_ADSP.ipynb
        └── 02_ADSP.ipynb
        
```

### Analysis Notebooks
* Languages: Python and bash

| **Directory** | Notebooks        | Description                        |
|---------------|------------------|------------------------------------|
| UKB/          | 00_UKB.ipynb |   |
|
| AMP PDRD/     | 00_AMP PDRD | Querying AMP PDRD to check for variants of interest |
|               | 01_AMP PDRD | Querying AMP PDRD for APOE genotyping |
|               | 02_AMP PDRD | Querying AMP PDRD to define cases and controls in each ancestry and to obtain demographic and phenotype data |
|
| AllOfUs/      | 00_AoU | Query AllofUs to create three cohorts (AD, Dementia, and Control), and characterize the genes of interest  |
|               | 01_AoU | Querying All of Us to prepare data for Genotools, applying Genotools, and calculating allele frequency   |
|               | 02_AoU | Querying AllofUs for APOE genotyping and defining ancestry for each genotype  |
|               | 03_AoU | Querying AllofUs for demographic and phenotype data |
|
| ADSP/         | 00_ADSP  | Querying ADSP to check for variants of interest, allele frequency, and to calculate missingness |
|               | 01_ADSP  | Querying ADSP for APOE genotyping |
|               | 02_ADSP  | Querying ADSP for demographic and phenotype data |


# Software 
|               Software              |  Version(s) |                              Resource URL                              |       RRID      |                                               Notes                                               |   |
|:-----------------------------------:|:-----------:|:----------------------------------------------------------------------:|:---------------:|:-------------------------------------------------------------------------------------------------:|:-:|
|     Python Programming Language     | 3.8 and 3.9 |                         http://www.python.org/                         | RRID:SCR_008394 | pandas; numpy; seaborn; matplotlib; statsmodel; used for general data wrangling/plotting/analyses |   |

|                PLINK                | 1.9 and 2.0 |                   http://www.nitrc.org/projects/plink                  | RRID:SCR_001757 |                                     used for genetic analyses                                     |   |
|         samtools (bcftools)         |     1.9     |                         https://www.htslib.org/                        | RRID:SCR_002105 |                                          VCF manipulation                                         |   |


