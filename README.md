![](https://img.shields.io/badge/language-R_and_Python-orange.svg) ![version](https://img.shields.io/badge/GiHub_version-1.1.0-519dd9) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/viktormiok/AstrocytesHeterogenityARC) ![GitHub issues](https://img.shields.io/github/issues/viktormiok/AstrocytesHeterogenityARC)

![dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-orange)  	![commit](https://img.shields.io/github/last-commit/viktormiok/AstrocytesHeterogenityARC) ![GitHub](https://img.shields.io/github/license/viktormiok/AstrocytesHeterogenityARC)

[![Edit with Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/viktormiok/AstrocytesHeterogenityARC) 



- [Introduction](#introduction)
  * [Summary of main findings](#summary-of-main-findings)
  * [Overview](#overview)
- [Data and analysis](#data-and-analysis)
- [License](#license)
- [References](#references)

## Introduction
We provide a detailed multi-omics view of the spatial and
temporal changes of different astrocyte populations in response to a high-fat
high-sugar diet. Using a combination of proteomics, RNAseq, and scRNAseq data
and their integrated analysis, together with in vivo labeling of astrocyte-specific
molecular markers, we show that the anatomical location of astrocytes
determines the cellular response to exposure to a high-caloric diet. Specifically,
our results identify a high sensitivity and strong molecular response of astrocytes
located in the arcuate nucleus of the hypothalamus upon exposure to a
hypercaloric diet.

<img src="https://github.com/viktormiok/AstrocytesHeterogenityARC/blob/main/GLIA_Graphical%20abstract_IGG.jpeg" align="center" height="540" width="730">

### Summary of main findings
- Long-term exposure to a hypercaloric diet differently affects the
the transcriptional pattern of astrocytes located in the cortex, hippocampus, and
hypothalamus, with the most prominent changes in the proteomic profile
of hypothalamic astrocytes.
- Unlike other cell types in the ARC, astrocytes rapidly respond to
a hypercaloric diet with a remarkable, yet transient, transcriptional
activation.
- The number of astrocytes expressing the astrocytic markers Aldh1L1 and
GFAP increases upon a high-fat high-sugar (HFHS) diet feeding in a
intraregional- and time-dependent manner.
- The spatial location of Aldh1L1- and GFAP- expressing astrocytes in the
ARC undergoes a dynamic reorganization in response to hypercaloric
diet. 

### Overview
Given that the CNS control of metabolism highly depends on functional hypothalamic astrocyte-neuron interactions we find our insights into the rapid and selective changes in astrocytes in response to a hypercaloric diet, before significant changes in body weight, inflammation, and insulin sensitivity, of particular interest. We provide a comprehensive multi-omics data collection on astrocytes and other cell types during different time points of the initial adaptation to a high
caloric diet to better understand the cellular circuitries acting in the ARC and their rearrangements in response to the HFHS diet. Of note, our spatial point pattern analysis method in itself provides an advancement to cell analysis in various disciplines and experimental setups, helping to describe the anatomy at a cellular level. 

## Data and analysis
All the data required for performing the analysis and publisch in the reference articles will be soon deposited in the National Center for Biotechnology Information Gene Expression Omnibus (GEO) and are accessible through the GEO Series accession numbers:
| Data type     | Link to the data | Notebook |
| ------------- | ------------- | ------------- |
| Transcriptomics  | [__`GSE205313`__](https://0-www-ncbi-nlm-nih-gov.brum.beds.ac.uk/geo/query/acc.cgi?acc=GSE205313)  | [transcriptomics_analysis_v1.ipynb](https://github.com/viktormiok/AstrocytesHeterogenityARC/blob/main/transcriptomics_analysis_v1.ipynb) |
| Proteomics  | [__`ProtData`__](https://www.biorxiv.org/content/10.1101/2022.03.30.486358v1.abstract) | [proteomics_analysis_v1.ipynb](https://github.com/viktormiok/AstrocytesHeterogenityARC/blob/main/proteomics_analysis_v1.ipynb) |
| Singel-Cell RNA-Seq  | [__`GSE205667`__](https://0-www-ncbi-nlm-nih-gov.brum.beds.ac.uk/geo/query/acc.cgi?acc=GSE205667)| [astrocyte_scRNAseq_cluster_approach.ipynb](https://github.com/viktormiok/AstrocytesHeterogenityARC/blob/main/astrocyte_scRNAseq_cluster_approach.ipynb)  |
| Astrocyte spatial point patterns  | [__`ASPP_data`__](https://github.com/viktormiok/AstrocytesHeterogenityARC/blob/main/SPP_data_all.csv)| [Csppa_analysis.ipynb](https://github.com/viktormiok/AstrocytesHeterogenityARC/blob/main/Csppa_analysis.ipynb)  |

In order to access one of the data set for instance GSE78279 you need to run the code bellow. Unpacking the data requires tar and gunzip, which should already be available on most systems.

```
cd ../  #To get to the main GitHub repo folder
mkdir -p data/AstrocytesHeterogenityARC/
cd data/AstrocytesHeterogenityARC/
wget ftp://ftp.ncbi.nlm.nih.gov/geo/series/GSE78nnn/GSE78279/suppl/GSE78279_RAW.tar
mkdir GSE78279_RAW
tar -C GSE78279_RAW -xvf GSE78279_RAW.tar
gunzip GSE78279_RAW/*_Regional_*
```
## License

__`AstrocytesHeterogenityARC`__ is distributed under the MIT license. Please read the license before using __`AstrocytesHeterogenityARC`__, which it is distributed in the `LICENSE` file.

## References

Publications related to __`AstrocytesHeterogenityARC`__ include:

- Lutomska, L.M., Miok, V., Krahmer, N., González García, I., Gruber, T., Le Thuc, O., De Bernardis Murat, C., Legutko, B., Sterr, M., Saher, G., Lickert, H., Ussar, S., Tschöp, M., Lutter, D., García-Cáceres, C. (2022), [Diet triggers specific responses of hypothalamic astrocytes in time and region dependent manner](https://onlinelibrary.wiley.com/doi/full/10.1002/glia.24237), *Glia 70 (10), 1795-2008*.
  
- Lutomska, L.M., Miok, V., Krahmer, N., González García, I., Gruber, T., Le Thuc, O., De Bernardis Murat, C., Legutko, B., Sterr, M., Saher, G., Lickert, H., Ussar, S., Tschöp, M., Lutter, D., García-Cáceres, C.(2021), [Hypercaloric diet selectively triggers a transient molecular rearrangement of astrocytes in the arcuate nucleus]( https://www.biorxiv.org/content/10.1101/2022.03.30.486358v1.abstract), bioRxiv, 4(1).

Please cite the publication if you use __`AstrocytesHeterogenityARC`__.


