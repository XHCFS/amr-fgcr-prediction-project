# Dataset
The data was obtained from previously published studies that aligned with our research and were downloaded from [NCBI](https://www.ncbi.nlm.nih.gov/) and [PATRIC](https://www.patricbrc.org/)

Notebook for downloading datasets: [Notebook](https://colab.research.google.com/drive/1zF_EdIyBJryyRerfMBpm5gvlxx8uiz65?usp=drive_link)

## Combined dataset overview

Included Species (6):
- Salmonella enterica
- Staphylococcus aureus
- Escherichia coli
- Acinetobacter baumannii
- Mycobacterium tuberculosis
- Klebsiella pneumoniae

Included Drugs (66):
<details>
<summary>Click to expand full list of drugs</summary>

<ul>
  <li>Streptomycin</li>
  <li>Amikacin/Kanamycin</li>
  <li>Macrolides</li>
  <li>Vancomycin</li>
  <li>Ceftriaxone</li>
  <li>Oxacillin</li>
  <li>Clindamycin</li>
  <li>Fusidic acid</li>
  <li>Beta-lactam</li>
  <li>Erythromycin</li>
  <li>Linezolid</li>
  <li>Methicillin</li>
  <li>Gentamicin</li>
  <li>Kanamycin/Tobramycin</li>
  <li>Trimethoprim-Sulfamethoxazole</li>
  <li>Fosfomycin</li>
  <li>Ciprofloxacin</li>
  <li>Tetracycline</li>
  <li>Streptothricin</li>
  <li>Nitrofurantoin</li>
  <li>Fluoroquinolones</li>
  <li>Chloramphenicol</li>
  <li>Penicillin</li>
  <li>Trimethoprim</li>
  <li>Lincosamide</li>
  <li>Daptomycin</li>
  <li>Cefoxitin</li>
  <li>Amikacin</li>
  <li>Ampicillin-Sulbactam</li>
  <li>Cefepime</li>
  <li>Cefotaxime</li>
  <li>Ceftazidime</li>
  <li>Colistin</li>
  <li>Doripenem</li>
  <li>Imipenem</li>
  <li>Levofloxacin</li>
  <li>Meropenem</li>
  <li>Minocycline</li>
  <li>Moxifloxacin</li>
  <li>Polymyxin_B</li>
  <li>Tigecycline</li>
  <li>Tobramycin</li>
  <li>Ampicillin</li>
  <li>Amoxicillin-Clavulanic acid</li>
  <li>Azithromycin</li>
  <li>Sulfisoxazole</li>
  <li>Kanamycin</li>
  <li>Nalidixic acid</li>
  <li>Ceftiofur</li>
  <li>Amoxicillin</li>
  <li>Capreomycin</li>
  <li>Clarithromycin</li>
  <li>Clofazimine</li>
  <li>Cycloserine</li>
  <li>Ethambutol</li>
  <li>Ethionamide</li>
  <li>Gatifloxacin</li>
  <li>Isoniazid</li>
  <li>Nicotinamide</li>
  <li>Ofloxacin</li>
  <li>para-aminosalicylic acid</li>
  <li>Prothionamide</li>
  <li>Pyrazinamide</li>
  <li>Rifabutin</li>
  <li>Rifampicin</li>
  <li>Aztreonam</li>
  <li>Cefuroxime</li>
  <li>Piperacillin-Tazobactam</li>
</ul>

</details>
<br>

Notebook used to create Master Table using csv file with labels from previous studies: [Master_Table](https://colab.research.google.com/drive/1dhboCENastOxyPSaOhRuYQfQ6jTG54XH?usp=sharing)


| Species                     | CSV with Labels                                                                 | Project Number                                           | Paper                                                                 |
|-----------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------|------------------------------------------------------------------------|
| *Staphylococcus aureus*     | [link](https://journals.asm.org/doi/suppl/10.1128/msystems.01185-20/suppl_file/msystems.01185-20-st001.xlsx) | _missing_                                                | [DOI](https://doi.org/10.1128/msystems.01185-20)                      |
| *Staphylococcus aureus*     | [link](https://zenodo.org/records/7101559)                                      | _missing_                                                | [DOI](https://doi.org/10.1002/minf.202300263)                         |
| *Escherichia coli*          | [link](https://github.com/tan0101/GSM_mSystems_2021/blob/main/Ecoli_genomes_metadata.xlsx)         | _missing_                                                | [DOI](https://doi.org/10.1128/msystems.00913-20)                      |
| *Salmonella enterica*       | [link](https://journals.asm.org/doi/suppl/10.1128/jcm.01260-18/suppl_file/jcm.01260-18-s0002.xlsx)  | PRJNA292661, PRJNA292666                                 | [DOI](https://doi.org/10.1128/jcm.01260-18)                           |
| *Klebsiella pneumoniae*     | [link](https://www.microbiologyresearch.org/deliver/fulltext/mgen/10/3/001222_2.xlsx)               | PRJEB27342                                               | [DOI](https://doi.org/10.1099/mgen.0.001222)                          |
| *Acinetobacter baumannii*   | [link](https://journals.asm.org/doi/suppl/10.1128/mbio.02852-24/suppl_file/mbio.02852-24-s0002.csv) | PRJNA1014981, PRJNA317141, PRJNA419431                   | [DOI](https://doi.org/10.1128/mbio.02852-24)                          |
| *Mycobacterium tuberculosis*| [link](https://github.com/aggreen/MTB-CNN/blob/main/input_data/master_table_resistance.csv)         | _missing_                                                | [DOI](https://doi.org/10.1038/s41467-022-31236-0)                     |

Note: for *Escherichia coli* and *Acinetobacter baumannii* more projects were used but their project numbers were not provided

## Data Encoding
Genomic sequences can be very large (_more than 3 million base per sequence_) and can vary a lot in size. In this research, we used Frequency Chaos Game Representation (FCGR) encoding which is an extension of Chaos Game Representation (CGR) encoding. It encodes sequences into images based on kmer frequencies. All samples were encoded into 256x256 images using 8-mer.

[Notebook](https://colab.research.google.com/drive/1KT3IifghuhJ8cfU4x7zERPTlFaYRUtWp?usp=drive_link)
_i cant find notebook you used for encoding_


# Selecting Drugs and Filtering Tables
The Master Table was used as a base to create tables for different models. From the available species, we selected three — *Staphylococcus aureus*, *Escherichia coli* and *Salmonella enterica* — based on the overall quality of their datasets. Quality of the datasets was determined by the balance between Resistnace (R) and Sensitive (S) labels, number of missing values (NULL) and suffiecent samples count for each drug.

We created a Species-Specific models for each of the selected species in addition to a General Model that combines samples from the three chosen species.

For drug selection, a score was calculated for each drug based on the Resistnace (R) / Sensitive (S) labels ratio and percentage of missing (NULL) values.

[Notebook](https://colab.research.google.com/drive/1Bad4Pw5tKiPYJM2SPluJbXt4MpBUEFPj?usp=drive_link)

# Homology splitting
To avoid data leakage in train, validation and test sets, sequences were comared aganist each other and assigned to clusters based on how similar they are. Samples in the same cluster are at least **95%/98%** similar and should not be in the same set. For comaparing samples together, Sourmash was used with the following parameter: k = 31, scaled = 1000 and threshold = 0.05/0.02.

[Notebook](https://colab.research.google.com/drive/11sSRr6gM8QC1sHBjLHbb2NfhHqvU5tey?usp=sharing)

Random cluster-aware split was used when dividing dataset into train, validation and test. Since clusters sizes are varied, we needed to ensure that not all large clusters are added to one set and small clusters are added to the other as it can greatly negetively affect diversity in sets. To avoid that, clusters were divided into groups based on size and a few clusters were randomly selected from each group.

[Notebook](https://colab.research.google.com/drive/1IQAgm1MvkCtmvderFYl3fNSvhR3_92kF?usp=drive_link)
<br> _the notebook needs cleaning_

# Training
**Pytorch** and **FastAI** were used to create and train model. After creating a Pytorch dataset, samples were split into train and test using homology-aware splitting mentioned before. Then, train set was divided — also homology aware — into **five** folds using **GroupKFold** in order to perform cross validation. Models were evaluated using a range of performance metrics, all of which were modified to mask missing (NULL) values. The metrics included:
- masked_acc
- masked_precision
- masked_recall
- masked_f1
- masked_fbeta
- masked_auc
- masked_jaccard
- masked_hamming
- masked_mcc

_i was planning on changing parameters and model architecture and compare results_
_architectures: ResNet, Xception and EfficientNet_

The mean and standard deviation of the results of cross validation were saved along with per drug evaluation. For General Model, per species evaluation was also calculated.

[Notebook](https://colab.research.google.com/drive/1zvtU66M9qVdQMwCIlHlQ5-6QI3M-vTHz?usp=sharing)

# Drive
[Link](https://drive.google.com/drive/folders/13LGqe__ULhjG0hZmpgxz8WqE0fNXsVNQ?usp=drive_link)

