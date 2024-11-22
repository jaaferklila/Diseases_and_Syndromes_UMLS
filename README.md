# 🩺 **Diseases and Syndromes Extraction from UMLS**

## 🔍 **Overview**
> The **Unified Medical Language System (UMLS)** facilitates the development of computer systems that "understand" the language of biomedicine and health.  
This repository focuses on extracting and analyzing **diseases and syndromes** from UMLS datasets, leveraging its semantic types and relationships.

---

## 📂 **Code and Dataset**
### 🗂 **Code Location**:
- The main code for this project can be found in the file:
  - 📄 `diseases-and-syndromes-umls.ipynb`
- You can also access the full project on Kaggle [Here](https://kaggle.com](https://www.kaggle.com/code/klilajaafer/diseases-and-syndromes-umls), where the **UMLS dataset** is pre-uploaded.  
  **(No need to download it again!)**

### 📊 **Final Outputs**:
- **Filtered defintion for diseases and syndromes **:
  - 📝 `cui_name_def_source_english.csv`: This file contains the name and definition for diseases and syndromes extracted from the UMLS dataset.
    ## 📄 **cui_name_def_source_english.csv**

This file contains filtered definitions for diseases and syndromes from the UMLS dataset. Below is a sample of the file's content:

| **CUI**     | **Name**                | **Definition**                                                                 | **Source** |
|-------------|--------------------------|--------------------------------------------------------------------------------|------------|
| C0000744    | Abetalipoproteinemia     | An autosomal recessive disorder of lipid metabolism.                           | MSH        |
| C0000744    | Abetalipoproteinemia     | Disorder of lipid metabolism inherited as an autosomal recessive trait.        | CSP        |

### **Columns Description**
- **CUI**: Concept Unique Identifier for the medical term.
- **Name**: Name of the disease or syndrome.
- **Definition**: Description or definition of the disease/syndrome.
- **Source**: Source of the definition (e.g., `MSH`, `CSP`).



- **Filtered Relationships**:
  - 📝 `filtered_relationships_with_rel_descriptions.csv`: This file includes filtered relationships between medical concepts.
## 📄 **filtered_relationships_with_rel_descriptions.csv**

This file includes filtered relationships between medical concepts, with details about the relationships. Below is a sample of the file's content:

| **CUI1**    | **AUI1**    | **STYPE1** | **REL**                   | **CUI2**    | **AUI2**    | **STYPE2** | **RELA** | **RUI**      | **SRUI** | **SAB** | **SL** | **RG** | **DIR** | **SUPPRESS** | **CVF** |
|-------------|-------------|------------|---------------------------|-------------|-------------|------------|----------|--------------|----------|---------|--------|---------|-------------|--------|
| C0000744    | A0017771    | SDUI       | Has parent relationship   | C0020597    | A10900707   | SDUI       | NaN      | R71362968    | NaN      | MSH     | MSH    | NaN     | NaN      | N           | NaN    |
| C0000744    | A0472584    | AUI        | Has parent relationship   | C0268197    | A1192421    | AUI        | NaN      | R05670678    | NaN      | CSP     | CSP    | NaN     | NaN      | N           | NaN    |

### **Columns Description**
- **CUI1**: Concept Unique Identifier for the first entity.
- **AUI1**: Atom Unique Identifier for the first entity.
- **STYPE1**: Semantic type of the first entity.
- **REL**: Relationship type (e.g., "Has parent relationship").
- **CUI2**: Concept Unique Identifier for the second entity.
- **AUI2**: Atom Unique Identifier for the second entity.
- **STYPE2**: Semantic type of the second entity.
- **RELA**: Relationship attribute (if available).
- **RUI**: Relationship Unique Identifier.
- **SRUI**: Semantic Relationship Unique Identifier (if applicable).
- **SAB**: Source abbreviation.
- **SL**: Source label.
- **RG**: Relationship group (if applicable).
- **DIR**: Direction of the relationship (if applicable).
- **SUPPRESS**: Suppression flag.
- **CVF**: Content view flag.

> **Note**: This is a sample from the file. The full dataset contains more relationships for various medical concepts.

---

## 🎯 **Purpose**
This project focuses on extracting **diseases** and **syndromes**, specifically targeting UMLS concepts with semantic type `T047`.  

💡 **Applications**:
- Building and enhancing ontologies.
- Constructing biomedical knowledge graphs.
- Preparing structured datasets for machine learning models in biomedical domains.

---

## 📂 **Key UMLS Files**

| **File**        | **Purpose**                                   | **Use**                                      |
|------------------|----------------------------------------------|---------------------------------------------|
| **MRSTY.RRF**    | Identifies semantic types for concepts.      | Filter diseases and syndromes (e.g., T047). |
| **MRCONSO.RRF**  | Provides names, synonyms, and abbreviations. | Retrieve names of diseases and syndromes.   |
| **MRDEF.RRF**    | Contains definitions for concepts.           | Add definitions to diseases and syndromes.  |
| **MRREL.RRF**    | Describes relationships between concepts.    | Build connections between diseases.         |

---

## 🎯 **Why Focus on the Metathesaurus?**
For extracting **diseases**, **syndromes**, and their relationships, the Metathesaurus is the most relevant component because:
- It includes terms from multiple vocabularies like SNOMED, MeSH, and ICD.
- It provides definitions from various sources, enriching datasets for analysis.

---

## 🛠 **How to Use**
1. Download the UMLS data from the [UMLS Website](https://www.nlm.nih.gov/research/umls/).
   - **Note**: You will need an account and a license agreement.
2. Use the following key files:
   - `MRSTY.RRF`: For semantic types.
   - `MRCONSO.RRF`: For concept names.
   - `MRDEF.RRF`: For definitions.
   - `MRREL.RRF`: For relationships.
