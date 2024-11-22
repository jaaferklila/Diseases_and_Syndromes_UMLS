<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">
    Purpose of the UMLS
</h2>
<p style="text-align: justify;font-size: 16px;">
    The <strong>Unified Medical Language System (UMLS)</strong> facilitates the development of computer systems that behave as if they "understand" the language of biomedicine and health. To that end, the <strong>National Library of Medicine (NLM)</strong> produces and distributes the UMLS Knowledge Sources (databases) and associated software tools (programs).
</p>
<p style="text-align: justify;font-size: 16px;">
    Developers use the Knowledge Sources and tools to build or enhance systems that create, process, retrieve, and integrate biomedical and health data and information. The Knowledge Sources are multi-purpose and are used in systems that perform diverse functions involving information types such as <em>patient records</em>, <em>scientific literature</em>, <em>guidelines</em>, and <em>public health data</em>.
</p>
<p style="text-align: justify;font-size: 16px;">
    The associated software tools assist developers in customizing or using the UMLS Knowledge Sources for particular purposes. The <strong>Lexical Tools</strong> work more effectively in combination with the UMLS Knowledge Sources, but can also be used independently.
</p>


<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">
    Components of the UMLS
</h2>
<p style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6; text-align: justify;">
    The <strong>Unified Medical Language System (UMLS)</strong> is composed of three main components that work together to support healthcare and biomedical informatics tasks:
</p>

<h3 style="color: green; font-size: 20px;">1. UMLS Metathesaurus</h3>
<p style="text-align: justify;font-size: 16px;">
    The <strong>Metathesaurus</strong> integrates terms and relationships from various biomedical vocabularies into a single, concept-based structure.
</p>
<ul style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6;">
    <li><strong>Unified Concepts:</strong> Groups terms and codes from different vocabularies under a single concept (<code>CUI</code>).</li>
    <li><strong>Semantic Relationships:</strong> Maps synonyms, broader/narrower terms, and causal links across vocabularies.</li>
</ul>



<h3 style="color: green; font-size: 20px;">2. UMLS Semantic Network</h3>
<p style="text-align: justify;font-size: 16px;">
    The <strong>Semantic Network</strong> organizes concepts from the Metathesaurus into high-level categories and relationships.
</p>
<ul style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6;">
    <li><strong>Semantic Types:</strong> Groups concepts into broad categories like <code>Disease or Syndrome</code> (TUI: <code>T047</code>).</li>
    <li><strong>Semantic Relationships:</strong> Links semantic types with predefined relationships (e.g., "affects").</li>
</ul>


<h3 style="color: green; font-size: 20px;">3. SPECIALIST Lexicon and Lexical Tools</h3>
<p style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6; text-align: justify;">
    The <strong>SPECIALIST Lexicon</strong> and associated <strong>Lexical Tools</strong> provide linguistic resources to process biomedical text.
</p>
<ul style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6;">
    <li><strong>SPECIALIST Lexicon:</strong> A curated lexicon of biomedical terms with linguistic information such as part of speech and inflection.</li>
    <li><strong>Lexical Tools:</strong> Software tools for text normalization, stemming, and word variation generation.</li>
</ul>

<h3 style="color: darkblue; font-size: 20px;">Comparison of the Three Components</h3>
<table border="1" style="width: 100%; border-collapse: collapse; font-family: Arial, sans-serif; font-size: 16px;">
    <thead style="background-color: #f2f2f2;">
        <tr>
            <th style="padding: 10px;">Component</th>
            <th style="padding: 10px;">Key Focus</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="padding: 10px;">Metathesaurus</td>
            <td style="padding: 10px;">Terms and relationships across vocabularies.</td>
        </tr>
        <tr>
            <td style="padding: 10px;">Semantic Network</td>
            <td style="padding: 10px;">Categorization and high-level relationships.</td>
        </tr>
        <tr>
            <td style="padding: 10px;">SPECIALIST Lexicon/Tools</td>
            <td style="padding: 10px;">Linguistic resources for biomedical text.</td>
        </tr>
    </tbody>
</table>


<h3 style="color: darkblue; font-size: 20px;">Why Focus on the Metathesaurus?</h3>
<p style="text-align: justify;font-size: 16px;">
    For extracting diseases, syndromes, definitions, and relationships, the <strong>Metathesaurus</strong> is the most relevant component because it:
</p>
<ul style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6;">
    <li><strong>Comprehensive Terminology:</strong> It includes terms from multiple vocabularies (e.g., SNOMED, MeSH, ICD).</li>
    <li><strong>Mappings and Relationships:</strong> It connects concepts with relationships like "causes" or "associated_with".</li>
    <li><strong>Definitions:</strong> It provides definitions from different sources to enrich datasets.</li>
</ul>


<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">Summary of the Files and Their Roles</h2>

<table border="1" style="width: 100%; border-collapse: collapse; font-family: Arial, sans-serif; font-size: 16px;">
    <thead style="background-color: #f2f2f2; text-align: left;">
        <tr>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>File</strong></th>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>Role</strong></th>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>Use</strong></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;"><code>MRSTY.RRF</code></td>
            <td style="padding: 10px; border: 1px solid #ddd;">Identifies semantic types of concepts (<code>Disease or Syndrome</code>).</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Filter diseases and syndromes by <code>STY</code>.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;"><code>MRCONSO.RRF</code></td>
            <td style="padding: 10px; border: 1px solid #ddd;">Provides terms and synonyms for each concept.</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Retrieve names of diseases and syndromes.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;"><code>MRDEF.RRF</code></td>
            <td style="padding: 10px; border: 1px solid #ddd;">Contains definitions of concepts.</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Add definitions to diseases and syndromes.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;"><code>MRREL.RRF</code></td>
            <td style="padding: 10px; border: 1px solid #ddd;">Describes relationships between concepts.</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Build connections between diseases and syndromes (e.g., "causes").</td>
        </tr>
    </tbody>
</table>


<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">Where to Find the UMLS Files</h2>
<h3 style="color: blue">Download UMLS</h3>
<ul>
    <li>You can download the UMLS Metathesaurus from the <a href="https://www.nlm.nih.gov/research/umls/" target="_blank">UMLS website</a>.</li>
    <li>You need an account and a license agreement to access the files.</li>
</ul>

<h3 style="color: blue">Installation Location</h3>
<ul>
    <li>After downloading and extracting the UMLS files using the <strong>MetamorphoSys</strong> installer, you'll find the files in the specified output directory.</li>
    <li>Look for the <strong>RRF (Rich Release Format)</strong> files in the <code>META</code> folder.</li>
</ul>

<h2 style="color: red;font-size: 16px;">Key UMLS Files We Will Use</h2>

<h3 style="color: green">1. MRSTY.RRF: Semantic Types</h3>
<p><strong>Purpose:</strong></p>
<ul>
    <li>Contains the semantic types (categories) for each concept (<code>CUI</code>).</li>
    <li>Helps identify diseases and syndromes under the semantic type <code>Disease or Syndrome</code> (TUI: <code>T047</code>).</li>
</ul>

<p><strong>Content:</strong></p>
<p>Each row associates a concept (<code>CUI</code>) with a semantic type (<code>STY</code>).</p>

<p><strong>Important Columns:</strong></p>
<table border="1">
    <tr>
        <th>Column</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>CUI</code></td>
        <td>Concept Unique Identifier (e.g., <code>C0011847</code>).</td>
    </tr>
    <tr>
        <td><code>STY</code></td>
        <td>Semantic Type (e.g., "Disease or Syndrome").</td>
    </tr>
    <tr>
        <td><code>TUI</code></td>
        <td>Type Unique Identifier (e.g., <code>T047</code>).</td>
    </tr>
</table>


<h3 style="color: green">2. MRCONSO.RRF: Concept Names</h3>
<p><strong>Purpose:</strong></p>
<ul>
    <li>Contains all the names, synonyms, and abbreviations for each concept (<code>CUI</code>).</li>
    <li>Used to retrieve the terms (names) for diseases and syndromes.</li>
</ul>

<p><strong>Content:</strong></p>
<p>Each row provides a <code>CUI</code> and its associated names in multiple languages.</p>

<p><strong>Important Columns:</strong></p>
<table border="1">
    <tr>
        <th>Column</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>CUI</code></td>
        <td>Concept Unique Identifier.</td>
    </tr>
    <tr>
        <td><code>LAT</code></td>
        <td>Language of the term (e.g., <code>ENG</code> for English).</td>
    </tr>
    <tr>
        <td><code>STR</code></td>
        <td>Name or term for the concept.</td>
    </tr>
    <tr>
        <td><code>SAB</code></td>
        <td>Source Vocabulary (e.g., SNOMED, MeSH).</td>
    </tr>
    <tr>
        <td><code>TTY</code></td>
        <td>Term Type (e.g., <code>PT</code> for Preferred Term).</td>
    </tr>
</table>



<h3 style="color: green">3. MRDEF.RRF: Definitions</h3>
<p><strong>Purpose:</strong></p>
<ul>
    <li>Contains definitions for some concepts.</li>
    <li>Useful for providing context to diseases and syndromes.</li>
</ul>

<p><strong>Content:</strong></p>
<p>Each row links a <code>CUI</code> to a definition (<code>DEF</code>).</p>

<p><strong>Important Columns:</strong></p>
<table border="1">
    <tr>
        <th>Column</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>CUI</code></td>
        <td>Concept Unique Identifier.</td>
    </tr>
    <tr>
        <td><code>DEF</code></td>
        <td>Definition text.</td>
    </tr>
</table>



<h3 style="color: green">4. MRREL.RRF: Relationships</h3>
<p><strong>Purpose:</strong></p>
<ul>
    <li>Contains relationships between concepts (e.g., diseases causing other diseases).</li>
    <li>Helps build connections between diseases and syndromes for a graph or text corpus.</li>
</ul>

<p><strong>Content:</strong></p>
<p>Each row describes a relationship between two concepts (<code>CUI1</code> and <code>CUI2</code>).</p>

<p><strong>Important Columns:</strong></p>
<table border="1">
    <tr>
        <th>Column</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>CUI1</code></td>
        <td>Source Concept.</td>
    </tr>
    <tr>
        <td><code>REL</code></td>
        <td>Type of relationship (e.g., <code>causes</code>).</td>
    </tr>
    <tr>
        <td><code>CUI2</code></td>
        <td>Target Concept.</td>
    </tr>
    <tr>
        <td><code>RELATYPE</code></td>
        <td>Additional type of relationship.</td>
    </tr>
</table>






<h2 style="color: red;">Step 1: Extract Diseases, Syndromes, and Their Relationships</h2>
<p style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6; text-align: justify;">
    In this step, we focus on extracting concepts categorized as <strong>"Disease or Syndrome"</strong> from the UMLS Metathesaurus. These concepts are identified using the semantic type <code>Disease or Syndrome</code> (TUI: <code>T047</code>) in the <code>MRSTY.RRF</code> file.
</p>

<p style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6; text-align: justify;">
    We will:
</p>
<ul style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6;">
    <li>Retrieve their names and synonyms from the <code>MRCONSO.RRF</code> file.</li>
    <li>Attach definitions from the <code>MRDEF.RRF</code></li>
    <li>Extract relationships between diseases and syndromes from the <code>MRREL.RRF</code> file.</li>
    <li>Save the extracted data into structured CSV files.</li>
</ul>


<h3 style="color: green;">Adding Relationships</h3>
<p style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6; text-align: justify;">
    Relationships between diseases and syndromes are essential for understanding how medical concepts are interconnected. These relationships are stored in the <code>MRREL.RRF</code> file 


<h3 style="color: blue;">Plan for Extracting Relationships</h3>
<ol style="font-family: Arial, sans-serif; font-size: 16px; line-height: 1.6;">
    <li>Filter relationships in the <code>MRREL.RRF</code> file where both <code>CUI1</code> and <code>CUI2</code> belong to the "Disease or Syndrome" semantic type.</li>
    <li>Extract the relationship type (<code>REL</code>) .</li>
    <li>Merge the results with disease and syndrome names from the <code>MRCONSO.RRF</code> file for readability.</li>
</ol>


<h3 style="color: orange;">Setup and Verify File Paths</h3>


```python
# Import necessary libraries
import os

# Define the UMLS folder path
umls_dir = "/kaggle/input/umls-2024aa"

# List all files in the directory
print("Files in the UMLS folder:")
for file in os.listdir(umls_dir):
    print(file)

```

    Files in the UMLS folder:
    MRDEF.RRF
    MRSTY.RRF
    MRREL.RRF
    MRCONSO.RRF


<h3 style="color: orange;">Load the Files</h3>

We'll load the necessary files (MRSTY.RRF, MRCONSO.RRF, MRDEF.RRF, MRREL.RRF) using Pandas for easier filtering and processing.

<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">Column Descriptions <code>MRSTY.RRF</code></h2>
Soure: <a href="https://www.ncbi.nlm.nih.gov/books/NBK9685/#ch03.sec3.2">MRSTY.RRF</a>
<table border="1" style="width: 100%; border-collapse: collapse; font-family: Arial, sans-serif; font-size: 16px;">
    <thead style="background-color: #f2f2f2; text-align: left;">
        <tr>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>Column</strong></th>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>Description</strong></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CUI</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of concept</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">TUI</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of Semantic Type</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">STN</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Semantic Type tree number</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">STY</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Semantic Type. The valid values are defined in the Semantic Network.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">ATUI</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for attribute</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">CVF</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Content View Flag. Bit field used to flag rows included in Content View. This field is a varchar field to maximize the number of bits available for use.</td>
        </tr>
    </tbody>
</table>



```python
import os
import pandas as pd

# Define column names for the MRSTY file
mrsty_columns = ["CUI", "TUI", "STN", "STY", "ATUI", "CVF", "EMPTY"]

# Path to the MRSTY.RRF file
mrsty_file = os.path.join(umls_dir, "MRSTY.RRF")

# Load MRSTY.RRF with correct column names
mrsty = pd.read_csv(mrsty_file, sep="|", header=None, names=mrsty_columns, dtype=str)

# Remove the last empty column caused by the trailing separator
mrsty = mrsty.drop(columns=["EMPTY"], errors="ignore")

# Display first few rows of MRSTY
print("Sample rows from MRSTY:")
print(mrsty.shape)
mrsty.head()

```

    Sample rows from MRSTY:
    (3549497, 6)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>TUI</th>
      <th>STN</th>
      <th>STY</th>
      <th>ATUI</th>
      <th>CVF</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000005</td>
      <td>T116</td>
      <td>A1.4.1.2.1.7</td>
      <td>Amino Acid, Peptide, or Protein</td>
      <td>AT17648347</td>
      <td>256</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000005</td>
      <td>T121</td>
      <td>A1.4.1.1.1</td>
      <td>Pharmacologic Substance</td>
      <td>AT17575038</td>
      <td>256</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000005</td>
      <td>T130</td>
      <td>A1.4.1.1.4</td>
      <td>Indicator, Reagent, or Diagnostic Aid</td>
      <td>AT17634323</td>
      <td>256</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000039</td>
      <td>T109</td>
      <td>A1.4.1.2.1</td>
      <td>Organic Chemical</td>
      <td>AT45562015</td>
      <td>256</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000039</td>
      <td>T121</td>
      <td>A1.4.1.1.1</td>
      <td>Pharmacologic Substance</td>
      <td>AT17567371</td>
      <td>256</td>
    </tr>
  </tbody>
</table>
</div>



<h3 style="color: orange;">Extract <span style="color: darkorange;">Disease or Syndrome Concepts</span></h3>
<p>Filter <code>MRSTY.RRF</code> for concepts with the semantic type <strong>"Disease or Syndrome"</strong> 
<span style="color: darkorange;">(TUI: T047)</span>.</p>



```python
# Filter for "Disease or Syndrome"
disease_cuis = mrsty[mrsty["TUI"] == "T047"]["CUI"].unique()

# Display the number of CUIs identified
print(f"Number of 'Disease or Syndrome' CUIs: {len(disease_cuis)}")

```

    Number of 'Disease or Syndrome' CUIs: 118579


<h3 style="color: orange;">Retrieve <span style="color: darkorange;">Disease Names</span> from <code>MRCONSO.RRF</code></h3>
<p>Using the filtered CUIs, extract the associated names (<strong>STR</strong>) from <code>MRCONSO.RRF</code>.</p>


<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">Column Descriptions <code>MRCONSO.RRF</code></h2> Source: <a href="https://www.ncbi.nlm.nih.gov/books/NBK9685/table/ch03.T.concept_names_and_sources_file_mr/">MRCONSO.RRF</a> <table border="1" style="width: 100%; border-collapse: collapse; font-family: Arial, sans-serif; font-size: 16px;"> <thead style="background-color: #f2f2f2; text-align: left;"> <tr> <th style="padding: 10px; border: 1px solid #ddd;"><strong>Column</strong></th> <th style="padding: 10px; border: 1px solid #ddd;"><strong>Description</strong></th> </tr> </thead> <tbody> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CUI</td> <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for concept</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">LAT</td> <td style="padding: 10px; border: 1px solid #ddd;">Language of the term</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">TS</td> <td style="padding: 10px; border: 1px solid #ddd;">Term status</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">LUI</td> <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for the term</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">STT</td> <td style="padding: 10px; border: 1px solid #ddd;">String type</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">SAB</td> <td style="padding: 10px; border: 1px solid #ddd;"> Abbreviated source name. Examples include: <ul> <li><strong>RSAB:</strong> Short form without version, e.g., "AIR".</li> <li><strong>VSAB:</strong> Versioned abbreviation, e.g., "AIR93".</li> </ul> </td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">STR</td> <td style="padding: 10px; border: 1px solid #ddd;">String</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">TTY</td> <td style="padding: 10px; border: 1px solid #ddd;">Abbreviation for term type in source vocabulary</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CODE</td> <td style="padding: 10px; border: 1px solid #ddd;">Most useful source-asserted identifier</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">SUPPRESS</td> <td style="padding: 10px; border: 1px solid #ddd;"> Suppressible flag. Examples: <ul> <li><strong>O:</strong> Obsolete content</li> <li><strong>E:</strong> Editor-marked suppressible</li> <li><strong>Y:</strong> Suppressible during inversion</li> <li><strong>N:</strong> Not suppressible</li> </ul> </td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CVF</td> <td style="padding: 10px; border: 1px solid #ddd;">Content View Flag used to flag rows</td> </tr> </tbody> </table>

<h3 style="color: #33FF33;">Filtering English Terms for Disease-Related CUIs</h3>

This script processes the UMLS MRCONSO.RRF file to extract terms related to diseases and syndromes. It filters the data to retain only English-language terms (LAT = "ENG") and those matching a predefined list of Concept Unique Identifiers (CUIs) associated with diseases. 




```python

# Load MRCONSO.RRF
mrconso_file = os.path.join(umls_dir, "MRCONSO.RRF")
mrconso = pd.read_csv(mrconso_file, sep="|", header=None, dtype=str, index_col=False)

# Assign column names to MRCONSO
mrconso.columns = [
    "CUI", "LAT", "TS", "LUI", "STT", "SUI", "ISPREF", "AUI",
    "SAUI", "SCUI", "SDUI", "SAB", "TTY", "CODE", "STR",
    "SRL", "SUPPRESS", "CVF","EMPTY"
]

# Filter for English terms corresponding to disease CUIs
disease_terms = mrconso[(mrconso["CUI"].isin(disease_cuis)) & (mrconso["LAT"] == "ENG")]

# Display sample rows
disease_terms.reset_index(drop=True, inplace=True)
print("number of cui related to disease and Syndrome:")
print(disease_terms.shape)
print("Sample disease terms:")
print(disease_terms[["CUI", "STR","SAB"]].head())

```

    number of cui related to disease and Syndrome:
    (593057, 19)
    Sample disease terms:
            CUI                   STR    SAB
    0  C0000744  Abetalipoproteinemia    MSH
    1  C0000744  Abetalipoproteinemia    MTH
    2  C0000744  Abetalipoproteinemia  RCDAE
    3  C0000744  Abetalipoproteinemia    SNM
    4  C0000744  Abetalipoproteinemia   SNMI



```python
disease_terms[["CUI", "STR","SAB","LAT"]].head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>STR</th>
      <th>SAB</th>
      <th>LAT</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>MSH</td>
      <td>ENG</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>MTH</td>
      <td>ENG</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>RCDAE</td>
      <td>ENG</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>SNM</td>
      <td>ENG</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>SNMI</td>
      <td>ENG</td>
    </tr>
  </tbody>
</table>
</div>




```python
data=pd.read_csv("/kaggle/working/disease_terms.csv")
print(data.shape)
data.head()
```

    (593057, 19)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>LAT</th>
      <th>TS</th>
      <th>LUI</th>
      <th>STT</th>
      <th>SUI</th>
      <th>ISPREF</th>
      <th>AUI</th>
      <th>SAUI</th>
      <th>SCUI</th>
      <th>SDUI</th>
      <th>SAB</th>
      <th>TTY</th>
      <th>CODE</th>
      <th>STR</th>
      <th>SRL</th>
      <th>SUPPRESS</th>
      <th>CVF</th>
      <th>EMPTY</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>ENG</td>
      <td>P</td>
      <td>L0000744</td>
      <td>PF</td>
      <td>S0009088</td>
      <td>N</td>
      <td>A0017771</td>
      <td>NaN</td>
      <td>M0000012</td>
      <td>D000012</td>
      <td>MSH</td>
      <td>MH</td>
      <td>D000012</td>
      <td>Abetalipoproteinemia</td>
      <td>0</td>
      <td>N</td>
      <td>256.0</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>ENG</td>
      <td>P</td>
      <td>L0000744</td>
      <td>PF</td>
      <td>S0009088</td>
      <td>N</td>
      <td>A0017772</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>MTH</td>
      <td>PT</td>
      <td>U000241</td>
      <td>Abetalipoproteinemia</td>
      <td>0</td>
      <td>N</td>
      <td>256.0</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>ENG</td>
      <td>P</td>
      <td>L0000744</td>
      <td>PF</td>
      <td>S0009088</td>
      <td>N</td>
      <td>A0017774</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>RCDAE</td>
      <td>PT</td>
      <td>C3253</td>
      <td>Abetalipoproteinemia</td>
      <td>3</td>
      <td>N</td>
      <td>256.0</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>ENG</td>
      <td>P</td>
      <td>L0000744</td>
      <td>PF</td>
      <td>S0009088</td>
      <td>N</td>
      <td>A0017775</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>SNM</td>
      <td>PT</td>
      <td>D-1367</td>
      <td>Abetalipoproteinemia</td>
      <td>9</td>
      <td>N</td>
      <td>256.0</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>ENG</td>
      <td>P</td>
      <td>L0000744</td>
      <td>PF</td>
      <td>S0009088</td>
      <td>N</td>
      <td>A0017776</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>SNMI</td>
      <td>PT</td>
      <td>D6-60210</td>
      <td>Abetalipoproteinemia</td>
      <td>9</td>
      <td>N</td>
      <td>256.0</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Get unique values from the SAB column
unique_sab_values = disease_terms["SAB"].unique()

# Print the unique values
print("Unique values in the SAB column:")
print(unique_sab_values)
print("the number of source vocabluries is",len(unique_sab_values))
```

    Unique values in the SAB column:
    ['MSH' 'MTH' 'RCDAE' 'SNM' 'SNMI' 'OMIM' 'NCI' 'ICD10CM' 'HPO'
     'SNOMEDCT_US' 'MDR' 'ORPHANET' 'MTHICD9' 'DXP' 'CSP' 'CHV'
     'ICPC2ICD10ENG' 'MEDCIN' 'RCD' 'ICD9CM' 'ICD10AM' 'ICD10' 'ICPC2P'
     'CCPSS' 'CCS' 'CST' 'WHO' 'COSTAR' 'LCH' 'LNC' 'MEDLINEPLUS' 'LCH_NW'
     'AOD' 'BI' 'SNOMEDCT_VET' 'PSY' 'QMR' 'RAM' 'ICPC' 'ICPC2EENG' 'AIR'
     'MTHMST' 'PDQ' 'DSM-5' 'ICD10AMAE' 'ICD10AE' 'NOC' 'JABL' 'NANDA-I' 'OMS'
     'CCSR_ICD10CM' 'MTHICPC2EAE' 'HL7V3.0' 'HL7V2.5' 'MTHICPC2ICD10AE' 'ICNP'
     'CPM' 'PCDS' 'CCC' 'ULT' 'UWDA' 'RCDSA' 'RCDSY' 'GO' 'DDB' 'AOT' 'MED-RT']
    the number of source vocabluries is 67


<h3 style="color: orange;">Extract <span style="color: darkorange;">Definitions</span> from <code>MRDEF.RRF</code></h3>
<p>We’ll load MRDEF.RRF and extract all definitions (DEF) for the filtered CUIs. 

<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">Column Descriptions <code>MRDEF.RRF</code></h2> <p style="font-size: 16px; font-family: Arial, sans-serif;"> The <code>MRDEF.RRF</code> file contains concept definitions from various sources within the UMLS Metathesaurus. Each row provides a unique identifier for the concept and the associated definition, along with metadata such as the source and suppressibility status. </p> <table border="1" style="width: 100%; border-collapse: collapse; font-family: Arial, sans-serif; font-size: 16px;"> <thead style="background-color: #f2f2f2; text-align: left;"> <tr> <th style="padding: 10px; border: 1px solid #ddd;"><strong>Column</strong></th> <th style="padding: 10px; border: 1px solid #ddd;"><strong>Description</strong></th> </tr> </thead> <tbody> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CUI</td> <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for the concept.</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">AUI</td> <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for the atom (variable length, 8 or 9 characters).</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">ATUI</td> <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for the attribute.</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">SATUI</td> <td style="padding: 10px; border: 1px solid #ddd;">Source asserted attribute identifier (optional).</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">SAB</td> <td style="padding: 10px; border: 1px solid #ddd;"> Abbreviated source name (SAB) of the source of the definition. Maximum field length: 20 alphanumeric characters. <ul> <li><strong>Root Source Abbreviation (RSAB)</strong>: Short form, no version information (e.g., "AIR").</li> <li><strong>Versioned Source Abbreviation (VSAB)</strong>: Includes version information (e.g., "AIR93").</li> </ul> </td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">DEF</td> <td style="padding: 10px; border: 1px solid #ddd;">The definition of the concept.</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">SUPPRESS</td> <td style="padding: 10px; border: 1px solid #ddd;">Suppressible flag. Values: O, E, Y, or N. Reflects the suppressible status of the attribute.</td> </tr> <tr> <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">CVF</td> <td style="padding: 10px; border: 1px solid #ddd;">Content View Flag. Bit field used to flag rows included in Content View.</td> </tr> </tbody> </table>


```python

# Load MRDEF.RRF
mrdef_file = os.path.join(umls_dir, "MRDEF.RRF")
mrdef = pd.read_csv(mrdef_file, sep="|", header=None, dtype=str, index_col=False)

# Assign column names to MRDEF
mrdef.columns = ["CUI", "AUI", "ATUI", "SATUI","SAB","DEF" ,"SUPPRESS","CVF","EMPTY"]

# Filter definitions for CUIs in the diseases/syndromes list
disease_definitions = mrdef[mrdef["CUI"].isin(disease_terms["CUI"])]
disease_definitions.reset_index(drop=True, inplace=True)
# Display sample rows
print("Sample definitions:")
disease_definitions[["CUI", "DEF","SAB"]].head()

```

    Sample definitions:





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>DEF</th>
      <th>SAB</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>An autosomal recessive disorder of lipid metab...</td>
      <td>MSH</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>disorder of lipid metabolism inherited as an a...</td>
      <td>CSP</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>Genetisk brist på betalipoprotein som leder ti...</td>
      <td>MSHSWE</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>An autosomal recessive disorder characterized ...</td>
      <td>NCI</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>An absence of low-density lipoprotein choleste...</td>
      <td>HPO</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Get unique values from the SAB column
unique_sab_values_disease_definitions = disease_definitions["SAB"].unique()

# Print the unique values
print("Unique values in the SAB column:")
print(unique_sab_values_disease_definitions)
print("the number of source vocabluries is",len(unique_sab_values_disease_definitions))
```

    Unique values in the SAB column:
    ['MSH' 'CSP' 'MSHSWE' 'NCI' 'HPO' 'MSHCZE' 'ORPHANET' 'MSHPOR' 'MSHSPA'
     'MEDLINEPLUS' 'MSHNOR' 'MSHFRE' 'AIR' 'SNOMEDCT_US' 'SCTSPA' 'CHV' 'PSY'
     'JABL' 'LNC' 'HL7V3.0' 'PDQ' 'NANDA-I' 'CCC' 'AOT']
    the number of source vocabluries is 24



```python
# Define a list of SABs corresponding to English-language vocabularies
english_sabs = [
    'MSH',          # Medical Subject Headings
    'CSP',          # Computer Retrieval of Information on Scientific Projects
    'NCI',          # National Cancer Institute Thesaurus
    'HPO',          # Human Phenotype Ontology
    'ORPHANET',     # Orphanet Rare Disease Ontology
    'MEDLINEPLUS',  # MedlinePlus
    'AIR',          # AI/Rheumatology
    'SNOMEDCT_US',  # Systematized Nomenclature of Medicine - Clinical Terms (US Edition)
    'CHV',          # Consumer Health Vocabulary
    'PSY',          # Psychological Index Terms
    'LNC',          # Logical Observation Identifiers Names and Codes (LOINC)
    'HL7V3.0',      # Health Level 7 Version 3.0 Vocabulary
    'PDQ',          # Physician Data Query
    'NANDA-I',      # North American Nursing Diagnosis Association International
    'CCC',          # Clinical Care Classification
    'AOT'           # Anatomical Therapeutic Chemical Classification System (ATC)
]

# Filter disease_definitions for English definitions based on SAB
english_definitions = disease_definitions[disease_definitions["SAB"].isin(english_sabs)]

# Display the filtered DataFrame
english_definitions.head()

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>AUI</th>
      <th>ATUI</th>
      <th>SATUI</th>
      <th>SAB</th>
      <th>DEF</th>
      <th>SUPPRESS</th>
      <th>CVF</th>
      <th>EMPTY</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>A0017771</td>
      <td>AT64676894</td>
      <td>NaN</td>
      <td>MSH</td>
      <td>An autosomal recessive disorder of lipid metab...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>A0472584</td>
      <td>AT51222156</td>
      <td>NaN</td>
      <td>CSP</td>
      <td>disorder of lipid metabolism inherited as an a...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>A17680492</td>
      <td>AT198023918</td>
      <td>NaN</td>
      <td>NCI</td>
      <td>An autosomal recessive disorder characterized ...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>A24667044</td>
      <td>AT288968072</td>
      <td>NaN</td>
      <td>HPO</td>
      <td>An absence of low-density lipoprotein choleste...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>6</th>
      <td>C0000744</td>
      <td>A34641265</td>
      <td>AT277513129</td>
      <td>NaN</td>
      <td>ORPHANET</td>
      <td>A severe, familial hypobetalipoproteinemia cha...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
english_definitions.reset_index(drop=True, inplace=True)
print(english_definitions.shape)
english_definitions.head()
```

    (26814, 9)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>AUI</th>
      <th>ATUI</th>
      <th>SATUI</th>
      <th>SAB</th>
      <th>DEF</th>
      <th>SUPPRESS</th>
      <th>CVF</th>
      <th>EMPTY</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>A0017771</td>
      <td>AT64676894</td>
      <td>NaN</td>
      <td>MSH</td>
      <td>An autosomal recessive disorder of lipid metab...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>A0472584</td>
      <td>AT51222156</td>
      <td>NaN</td>
      <td>CSP</td>
      <td>disorder of lipid metabolism inherited as an a...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>A17680492</td>
      <td>AT198023918</td>
      <td>NaN</td>
      <td>NCI</td>
      <td>An autosomal recessive disorder characterized ...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>A24667044</td>
      <td>AT288968072</td>
      <td>NaN</td>
      <td>HPO</td>
      <td>An absence of low-density lipoprotein choleste...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>A34641265</td>
      <td>AT277513129</td>
      <td>NaN</td>
      <td>ORPHANET</td>
      <td>A severe, familial hypobetalipoproteinemia cha...</td>
      <td>N</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Merge disease terms and filtered English definitions
merged_data = pd.merge(
    disease_terms,
    english_definitions[["CUI", "DEF", "SAB"]],
    on="CUI",
    how="inner",
    suffixes=("_terms", "_defs")  # Ensure unique suffixes
)

# Check columns in merged_data
print("Columns in merged_data:")
print(merged_data.columns)

# Select correct SAB column (assume SAB from english_definitions as SAB_defs)
final_data = merged_data[["CUI", "STR", "DEF", "SAB_defs"]]
final_data.columns = ["CUI", "Name", "Definition", "Source"]

# Save to CSV
output_file = "cui_name_def_source_english.csv"
final_data.to_csv(output_file, index=False)

# Display summary and sample rows
print(f"File '{output_file}' created with {final_data.shape[0]} rows.")
print("Sample rows:")
print(final_data.head())

```

    Columns in merged_data:
    Index(['CUI', 'LAT', 'TS', 'LUI', 'STT', 'SUI', 'ISPREF', 'AUI', 'SAUI',
           'SCUI', 'SDUI', 'SAB_terms', 'TTY', 'CODE', 'STR', 'SRL', 'SUPPRESS',
           'CVF', 'EMPTY', 'DEF', 'SAB_defs'],
          dtype='object')
    File 'cui_name_def_source_english.csv' created with 621052 rows.
    Sample rows:
            CUI                  Name  \
    0  C0000744  Abetalipoproteinemia   
    1  C0000744  Abetalipoproteinemia   
    2  C0000744  Abetalipoproteinemia   
    3  C0000744  Abetalipoproteinemia   
    4  C0000744  Abetalipoproteinemia   
    
                                              Definition    Source  
    0  An autosomal recessive disorder of lipid metab...       MSH  
    1  disorder of lipid metabolism inherited as an a...       CSP  
    2  An autosomal recessive disorder characterized ...       NCI  
    3  An absence of low-density lipoprotein choleste...       HPO  
    4  A severe, familial hypobetalipoproteinemia cha...  ORPHANET  



```python
print(final_data.shape)
final_data.head()
```

    (621052, 4)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI</th>
      <th>Name</th>
      <th>Definition</th>
      <th>Source</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>An autosomal recessive disorder of lipid metab...</td>
      <td>MSH</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>disorder of lipid metabolism inherited as an a...</td>
      <td>CSP</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>An autosomal recessive disorder characterized ...</td>
      <td>NCI</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>An absence of low-density lipoprotein choleste...</td>
      <td>HPO</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>Abetalipoproteinemia</td>
      <td>A severe, familial hypobetalipoproteinemia cha...</td>
      <td>ORPHANET</td>
    </tr>
  </tbody>
</table>
</div>



<h2 style="color: darkblue; font-size: 24px; border-bottom: 2px solid gray; padding-bottom: 5px;">
    Column Descriptions <code>MRREL.RRF</code>
</h2>
Source: <a href="https://www.ncbi.nlm.nih.gov/books/NBK9685/table/ch03.T.related_concepts_file_mrrel_rrf/">MRREL.RRF</a>
<table border="1" style="width: 100%; border-collapse: collapse; font-family: Arial, sans-serif; font-size: 16px;">
    <thead style="background-color: #f2f2f2; text-align: left;">
        <tr>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>Column</strong></th>
            <th style="padding: 10px; border: 1px solid #ddd;"><strong>Description</strong></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CUI1</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of the first concept.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">AUI1</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of the first atom.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">STYPE1</td>
            <td style="padding: 10px; border: 1px solid #ddd;">The name of the column in MRCONSO.RRF that contains the identifier used for the first element in the relationship (e.g., AUI, CODE, CUI, SCUI, SDUI).</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">REL</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Relationship of the second concept or atom to the first concept or atom.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">CUI2</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of the second concept.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">AUI2</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of the second atom.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">STYPE2</td>
            <td style="padding: 10px; border: 1px solid #ddd;">The name of the column in MRCONSO.RRF that contains the identifier used for the second element in the relationship (e.g., AUI, CODE, CUI, SCUI, SDUI).</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">RELA</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Additional (more specific) relationship label (optional).</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">RUI</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier of the relationship.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">SRUI</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Source-asserted relationship identifier, if present.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">SAB</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Abbreviated source name of the relationship source.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">SL</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Source of relationship labels.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">RG</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Relationship group, used to indicate a set of relationships that should be looked at in conjunction.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">DIR</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Source-asserted directionality flag.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #f9f9f9;">SUPPRESS</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Suppressible flag.</td>
        </tr>
        <tr>
            <td style="padding: 10px; border: 1px solid #ddd; background-color: #ffffff;">CVF</td>
            <td style="padding: 10px; border: 1px solid #ddd;">Content View Flag.</td>
        </tr>
    </tbody>
</table>



```python


```


```python
# Path to the MRREL.RRF file
import os
import pandas as pd
mrrel_file = os.path.join("/kaggle/input/umls-2024aa/MRREL.RRF")

# Define column names for MRREL
mrrel_columns = [
    "CUI1", "AUI1", "STYPE1", "REL", "CUI2", "AUI2", 
    "STYPE2", "RELA", "RUI", "SRUI", "SAB", "SL", 
    "RG", "DIR", "SUPPRESS", "CVF", "EMPTY"
]

# Load MRREL.RRF with correct column names
mrrel = pd.read_csv(mrrel_file, sep="|", header=None, names=mrrel_columns, dtype=str)

# Remove the last empty column caused by the trailing separator
mrrel = mrrel.drop(columns=["EMPTY"], errors="ignore")

# Display the shape and first few rows
print("Sample rows from MRREL:")
print(mrrel.shape)
print(mrrel.head())


```

    Sample rows from MRREL:
    (45548020, 16)
           CUI1       AUI1 STYPE1 REL      CUI2       AUI2 STYPE2            RELA  \
    0  C0000005  A13433185   SCUI  RB  C0036775   A7466261   SCUI             NaN   
    1  C0000005  A26634265   SCUI  RB  C0036775   A0115649   SCUI             NaN   
    2  C0000039   A0016515    AUI  SY  C0000039  A11754881    AUI  translation_of   
    3  C0000039   A0016515    AUI  SY  C0000039  A13042554    AUI  translation_of   
    4  C0000039   A0016515    AUI  SY  C0000039  A13096036    AUI  translation_of   
    
              RUI SRUI     SAB      SL   RG  DIR SUPPRESS  CVF  
    0   R86000559  NaN  MSHFRE  MSHFRE  NaN  NaN        N  NaN  
    1   R31979041  NaN     MSH     MSH  NaN  NaN        N  NaN  
    2  R101808683  NaN  MSHSWE  MSHSWE  NaN  NaN        N  NaN  
    3  R193408122  NaN  MSHCZE  MSHCZE  NaN  NaN        N  NaN  
    4   R73331672  NaN  MSHPOR  MSHPOR  NaN  NaN        N  NaN  



```python
mrrel.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI1</th>
      <th>AUI1</th>
      <th>STYPE1</th>
      <th>REL</th>
      <th>CUI2</th>
      <th>AUI2</th>
      <th>STYPE2</th>
      <th>RELA</th>
      <th>RUI</th>
      <th>SRUI</th>
      <th>SAB</th>
      <th>SL</th>
      <th>RG</th>
      <th>DIR</th>
      <th>SUPPRESS</th>
      <th>CVF</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000005</td>
      <td>A13433185</td>
      <td>SCUI</td>
      <td>RB</td>
      <td>C0036775</td>
      <td>A7466261</td>
      <td>SCUI</td>
      <td>NaN</td>
      <td>R86000559</td>
      <td>NaN</td>
      <td>MSHFRE</td>
      <td>MSHFRE</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000005</td>
      <td>A26634265</td>
      <td>SCUI</td>
      <td>RB</td>
      <td>C0036775</td>
      <td>A0115649</td>
      <td>SCUI</td>
      <td>NaN</td>
      <td>R31979041</td>
      <td>NaN</td>
      <td>MSH</td>
      <td>MSH</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000039</td>
      <td>A0016515</td>
      <td>AUI</td>
      <td>SY</td>
      <td>C0000039</td>
      <td>A11754881</td>
      <td>AUI</td>
      <td>translation_of</td>
      <td>R101808683</td>
      <td>NaN</td>
      <td>MSHSWE</td>
      <td>MSHSWE</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000039</td>
      <td>A0016515</td>
      <td>AUI</td>
      <td>SY</td>
      <td>C0000039</td>
      <td>A13042554</td>
      <td>AUI</td>
      <td>translation_of</td>
      <td>R193408122</td>
      <td>NaN</td>
      <td>MSHCZE</td>
      <td>MSHCZE</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000039</td>
      <td>A0016515</td>
      <td>AUI</td>
      <td>SY</td>
      <td>C0000039</td>
      <td>A13096036</td>
      <td>AUI</td>
      <td>translation_of</td>
      <td>R73331672</td>
      <td>NaN</td>
      <td>MSHPOR</td>
      <td>MSHPOR</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Filter relationships for diseases only (CUI1 or CUI2 in disease CUIs)
disease_relations = mrrel[
    (mrrel["CUI1"].isin(disease_cuis)) | (mrrel["CUI2"].isin(disease_cuis))
]

# Display the number of relationships identified
print(f"Number of relationships involving disease CUIs: {len(disease_relations)}")

# Display sample relationships
print("Sample disease relationships:")
print(disease_relations[["CUI1", "REL", "CUI2", "SAB"]].head())
```

    Number of relationships involving disease CUIs: 7959382
    Sample disease relationships:
              CUI1 REL      CUI2          SAB
    1487  C0000165  RN  C0268296          MSH
    1493  C0000165  RN  C1849695          MSH
    3974  C0000294  RO  C0571184  SNOMEDCT_US
    4019  C0000294  RO  C0010692       MED-RT
    4020  C0000294  RO  C0010692       MED-RT



```python
disease_relations.reset_index(drop=True, inplace=True)
print(disease_relations.shape)
disease_relations.head()
```

    (7959382, 16)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI1</th>
      <th>AUI1</th>
      <th>STYPE1</th>
      <th>REL</th>
      <th>CUI2</th>
      <th>AUI2</th>
      <th>STYPE2</th>
      <th>RELA</th>
      <th>RUI</th>
      <th>SRUI</th>
      <th>SAB</th>
      <th>SL</th>
      <th>RG</th>
      <th>DIR</th>
      <th>SUPPRESS</th>
      <th>CVF</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000165</td>
      <td>A0016695</td>
      <td>SDUI</td>
      <td>RN</td>
      <td>C0268296</td>
      <td>A18468082</td>
      <td>SDUI</td>
      <td>mapped_to</td>
      <td>R148231764</td>
      <td>NaN</td>
      <td>MSH</td>
      <td>MSH</td>
      <td>1</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000165</td>
      <td>A0016695</td>
      <td>SDUI</td>
      <td>RN</td>
      <td>C1849695</td>
      <td>A20980922</td>
      <td>SDUI</td>
      <td>mapped_to</td>
      <td>R134997404</td>
      <td>NaN</td>
      <td>MSH</td>
      <td>MSH</td>
      <td>1</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000294</td>
      <td>A2883946</td>
      <td>SCUI</td>
      <td>RO</td>
      <td>C0571184</td>
      <td>A30268646</td>
      <td>SCUI</td>
      <td>has_causative_agent</td>
      <td>R143833205</td>
      <td>4714306024</td>
      <td>SNOMEDCT_US</td>
      <td>SNOMEDCT_US</td>
      <td>1</td>
      <td>Y</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000294</td>
      <td>A31762929</td>
      <td>SCUI</td>
      <td>RO</td>
      <td>C0010692</td>
      <td>A0044773</td>
      <td>SCUI</td>
      <td>may_be_prevented_by</td>
      <td>R176745649</td>
      <td>NaN</td>
      <td>MED-RT</td>
      <td>MED-RT</td>
      <td>NaN</td>
      <td>N</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000294</td>
      <td>A31762929</td>
      <td>SCUI</td>
      <td>RO</td>
      <td>C0010692</td>
      <td>A0044773</td>
      <td>SCUI</td>
      <td>may_be_treated_by</td>
      <td>R176776810</td>
      <td>NaN</td>
      <td>MED-RT</td>
      <td>MED-RT</td>
      <td>NaN</td>
      <td>N</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
relevant_cuis = final_data["CUI"].unique()
```


```python


# Filter the relationships to include only rows where both CUI1 and CUI2 are in relevant CUIs
filtered_relationships = disease_relations[
    (disease_relations["CUI1"].isin(relevant_cuis)) & (disease_relations["CUI2"].isin(relevant_cuis))
].reset_index(drop=True)

# Display summary of filtered relationships
print(f"Number of filtered relationships: {filtered_relationships.shape[0]}")

# Save the filtered relationships to a CSV file
filtered_relationships_output_file = "filtered_relationships.csv"
filtered_relationships.to_csv(filtered_relationships_output_file, index=False)

print(f"Filtered relationships saved to '{filtered_relationships_output_file}'.")

```

    Number of filtered relationships: 1514164
    Filtered relationships saved to 'filtered_relationships.csv'.



```python
filtered_relationships[["CUI1","CUI2","REL","SAB"]].head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI1</th>
      <th>CUI2</th>
      <th>REL</th>
      <th>SAB</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>C0000744</td>
      <td>SY</td>
      <td>MSHSWE</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>C0000744</td>
      <td>SY</td>
      <td>MSHPOL</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>C0000744</td>
      <td>SY</td>
      <td>MSHCZE</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>C0000744</td>
      <td>SY</td>
      <td>MSHFRE</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>C0000744</td>
      <td>SY</td>
      <td>MSHGER</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Filter relationships for English SABs
filtered_english_relationships = filtered_relationships[
    filtered_relationships["SAB"].isin(english_sabs)
].reset_index(drop=True)

# Display the number of filtered rows and sample
print(f"Number of relationships with English SABs: {filtered_english_relationships.shape[0]}")
print("Sample rows:")
print(filtered_english_relationships[["CUI1", "CUI2", "REL", "SAB"]].head())

# Save to a new CSV file
output_file_english_sabs = "filtered_relationships_english_sabs.csv"
filtered_english_relationships.to_csv(output_file_english_sabs, index=False)
print(f"Filtered relationships with English SABs saved to '{output_file_english_sabs}'.")

```

    Number of relationships with English SABs: 119736
    Sample rows:
           CUI1      CUI2  REL  SAB
    0  C0000744  C0020597  PAR  MSH
    1  C0000744  C0000744   SY  MSH
    2  C0000744  C0268197  PAR  CSP
    3  C0000744  C0268197   RB  CSP
    4  C0000744  C0000744   RQ  CSP
    Filtered relationships with English SABs saved to 'filtered_relationships_english_sabs.csv'.



```python
# Filter out rows where CUI1 equals CUI2
filtered_no_self_references = filtered_english_relationships[
    filtered_english_relationships["CUI1"] != filtered_english_relationships["CUI2"]
].reset_index(drop=True)

# Display the number of relationships after filtering and sample rows
print(f"Number of relationships after removing self-references: {filtered_no_self_references.shape[0]}")
print("Sample rows:")
print(filtered_no_self_references[["CUI1", "CUI2", "REL", "SAB"]].head())

# Save the filtered data to a new CSV file
output_file_no_self_references = "filtered_relationships_no_self_references.csv"
filtered_no_self_references.to_csv(output_file_no_self_references, index=False)
print(f"Filtered relationships without self-references saved to '{output_file_no_self_references}'.")

```

    Number of relationships after removing self-references: 73350
    Sample rows:
           CUI1      CUI2  REL  SAB
    0  C0000744  C0020597  PAR  MSH
    1  C0000744  C0268197  PAR  CSP
    2  C0000744  C0268197   RB  CSP
    3  C0000744  C0020597   RQ  CSP
    4  C0000744  C0687751   RQ  CSP
    Filtered relationships without self-references saved to 'filtered_relationships_no_self_references.csv'.



```python
# Retrieve the REL column values as a NumPy array
rel_values = filtered_no_self_references["REL"].value_counts()

# Display the REL values
print(rel_values)

```

    REL
    PAR    24465
    CHD    24465
    RO     12488
    RB      4872
    RN      4872
    RQ      1898
    SY       290
    Name: count, dtype: int64


<h3 style="color: orange;">Map <span style="color: darkorange;">Relationship Abbreviations</span> to Full Descriptions</h3>
<p>We’ll map relationship abbreviations (REL) such as <code>PAR</code>, <code>RB</code>, and <code>SY</code> to their full descriptions like "Has parent relationship," "Has a broader relationship," and "Source asserted synonymy," ensuring the data is more readable and interpretable for analysis.</p>
<span>Source abbreviations</span> <a href="https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html">abbreviations</a>



```python
# Define the mapping for REL (relationships)
rel_mapping = {
   
    "CHD": "Has child relationship",
    
    "PAR": "Has parent relationship",
    
    "RB": "Has a broader relationship",
  
    "RN": "Has a narrower relationship",
    "RO": "Has other relationship",
    "RQ": "Related and possibly synonymous",
    
    "SY": "Source asserted synonymy",
    
   
}

```


```python
# Map REL abbreviations to their descriptions
filtered_no_self_references["REL"] = filtered_no_self_references["REL"].map(rel_mapping)

# Display sample rows with REL descriptions
print("Sample rows with REL descriptions:")
print(filtered_no_self_references[["CUI1", "CUI2", "REL", "SAB"]].head())

# Save the updated dataset to a new CSV file
output_file_rel_descriptions = "filtered_relationships_with_rel_descriptions.csv"
filtered_no_self_references.to_csv(output_file_rel_descriptions, index=False)
print(f"Filtered relationships with REL descriptions saved to '{output_file_rel_descriptions}'.")

```

    Sample rows with REL descriptions:
           CUI1      CUI2                              REL  SAB
    0  C0000744  C0020597          Has parent relationship  MSH
    1  C0000744  C0268197          Has parent relationship  CSP
    2  C0000744  C0268197       Has a broader relationship  CSP
    3  C0000744  C0020597  Related and possibly synonymous  CSP
    4  C0000744  C0687751  Related and possibly synonymous  CSP
    Filtered relationships with REL descriptions saved to 'filtered_relationships_with_rel_descriptions.csv'.



```python
filtered_no_self_references.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CUI1</th>
      <th>AUI1</th>
      <th>STYPE1</th>
      <th>REL</th>
      <th>CUI2</th>
      <th>AUI2</th>
      <th>STYPE2</th>
      <th>RELA</th>
      <th>RUI</th>
      <th>SRUI</th>
      <th>SAB</th>
      <th>SL</th>
      <th>RG</th>
      <th>DIR</th>
      <th>SUPPRESS</th>
      <th>CVF</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>C0000744</td>
      <td>A0017771</td>
      <td>SDUI</td>
      <td>Has parent relationship</td>
      <td>C0020597</td>
      <td>A10900707</td>
      <td>SDUI</td>
      <td>NaN</td>
      <td>R71362968</td>
      <td>NaN</td>
      <td>MSH</td>
      <td>MSH</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>C0000744</td>
      <td>A0472584</td>
      <td>AUI</td>
      <td>Has parent relationship</td>
      <td>C0268197</td>
      <td>A1192421</td>
      <td>AUI</td>
      <td>NaN</td>
      <td>R05670678</td>
      <td>NaN</td>
      <td>CSP</td>
      <td>CSP</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>C0000744</td>
      <td>A0472584</td>
      <td>AUI</td>
      <td>Has a broader relationship</td>
      <td>C0268197</td>
      <td>A1192421</td>
      <td>AUI</td>
      <td>NaN</td>
      <td>R00891659</td>
      <td>NaN</td>
      <td>CSP</td>
      <td>CSP</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>C0000744</td>
      <td>A0472584</td>
      <td>AUI</td>
      <td>Related and possibly synonymous</td>
      <td>C0020597</td>
      <td>A0598667</td>
      <td>AUI</td>
      <td>use</td>
      <td>R43985599</td>
      <td>NaN</td>
      <td>CSP</td>
      <td>CSP</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C0000744</td>
      <td>A0472584</td>
      <td>AUI</td>
      <td>Related and possibly synonymous</td>
      <td>C0687751</td>
      <td>A1302516</td>
      <td>AUI</td>
      <td>use</td>
      <td>R43985600</td>
      <td>NaN</td>
      <td>CSP</td>
      <td>CSP</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>N</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
filtered_no_self_references.shape
```




    (73350, 16)




```python

```
