# 🩺 **Diseases and Syndromes Extraction from UMLS**

## 🔍 **Overview**
> The **Unified Medical Language System (UMLS)** facilitates the development of computer systems that "understand" the language of biomedicine and health.  
This repository focuses on extracting and analyzing **diseases and syndromes** from UMLS datasets, leveraging its semantic types and relationships.

---

## 📂 **Code and Dataset**
### 🗂 **Code Location**:
- The main code for this project can be found in the file:
  - 📄 `diseases-and-syndromes-umls.ipynb`
- You can also access the full project on Kaggle [Here]([https://kaggle.com](https://www.kaggle.com/code/klilajaafer/diseases-and-syndromes-umls)]), where the **UMLS dataset** is pre-uploaded.  
  **(No need to download it again!)**

### 📊 **Final Outputs**:
- **Filtered Relationships**:
  - 📝 `filtered_relationships.csv`: Contains relationships specifically for diseases and syndromes.
- **Enriched Relationships**:
  - 📝 `enriched_relationships.csv`: Includes concepts relationships.

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
