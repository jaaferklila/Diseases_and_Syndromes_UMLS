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
