# Targeting-calcium-signaling-in-bone-micrometastases

This repository is the code for bioinformatic analysis of the manuscript "The osteogenic niche is a calcium reservoir of breast cancer bone micrometastases and confers unexpected therapeutic vulnerability". The paper is reviewed and in revison for ***Cancer Cell***.

Codes are generated by Dr. Xiang Zhang, Dr. Lin Tian and Dr. Hai Wang.

Please contact haiw@bcm.edu if you have any questions.

## RNAseq datase normalization

* Data normalization
* Collapse to gene names

## Figure 1 and 5

* Preparation for Analysis
* Gene Set variation analysis
* Analysis on Breast cancer metastasis
* Apply the same procedures for prostate cancer
* correlation between mef2, nfat, mecp2 and Cx43(GJA1)

## Survival curve in Figure S1 and S5

* Figure S1: Metastasis-free survival curve on 8-gene NFAT signature expression
* Figure S5: Metastasis-free survival curve on Cx43 expression

## Figure 2B and 4B

* Comparison between IVBLs and orthotopic tumors

## Figure 4E

* Analysis of GSE29036 in Figure 4E

## Figure 7 and S8

* Figure 7B and Figure S8C & S8D: use heatmaps to visualize the efficacies of drug treatment in BICA

## Dataset information:
| Dataset (RData) | Objects | Description |
| --- | --- | --- |
| breast-mets-gse14020.RData (The breast cancer metastases data from GSE14020) | allmets.mn | Data matrix with each row as an Affymetrix U133 probe and each column as a metastasis sample |
| --- | allmets.clps | Data matrix derived from allmets.mn with probes mapped to the same gene averaged into one value. |
| --- | allmets.ann | Annotation of breast cancer metastases containing site of metastasis information . The order of rows (samples) is exactly the same as the order of columns in allmets.clps. |
| CRPC-mets-gse77930.RData (The castration resistance prostate cancer metastasis data from GSE77930 | gse77930 | Data matrix with each row as a probe on microarray and each column as a metastasis sample |
| * Please download all the splitted files (.zip, .z01, .z02, .z03) before unzip  | gse77930.clps | Data matrix derived from gse77930 with probes mapped to the same gene averaged into one value. |
| --- | gse77930.ann | Annotation of prostate cancer metastases containing site information . The order of rows (samples) is exactly the same as the order of columns in allmets.clps. |
| Pre-clinical-model-GSE110451.RData | gse110451.clps | Data matrix derived from gse110451 with each role as a gene and each role as a biological replicate of either in vivo bone lesion or a orthotopic tumor. |
| --- | gse110451.ann | Annotation of sample type (IVBL: in vivo bone lesion, or Ortho: orthotopic tumors). |
| Stromal-cell-with-CC-GSE29036.RData (MSC, myoepithelial cells and fibroblasts co-cultured with various cancer cells) | msc.cc | Data matrix with each row as an Affymetrix U133 probe and each column as a metastasis sample |
| * Please download all the splitted files (.zip, .z01, .z02) before unzip  | msc.cc.clps | Data matrix derived from msc.cc with probes mapped to the same gene averaged into one value. |
| --- | msc.cc.ann | Annotation of both parties of cells in each co-culture sample. The order of rows (samples) is exactly the same as the order of columns in allmets.clps. |
| mef2 signature.txt | --- | MEF2 signature obtained from Di Giorgio et al., PloS Genetics 2017. |

