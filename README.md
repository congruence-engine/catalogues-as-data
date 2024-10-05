# Museums' online catalogues-as-data

## Short summary

In the field of digital cultural heritage, museum collections are often seen as ideal datasets for computationally-driven research and work. Not surprisingly, museum online catalogues are thus used as a public-facing entry point to museum collections, enhancing collections’ access and exploration while ensuring engagement with various audiences.
Museum online catalogues are rich information architectures/carriers/structures, usually including digitised versions/surrogates of the analogue assets alongside associated metadata in various formats, combined with data management and search tools. 

Although large focus and investment in the digital cultural heritage sector is given into understand and assess (digital) cataloguing practices as well as into experimenting with interface design and ‘generous interfaces’, advanced computing power and functionalities of online catalogues, the connecting tissue that will allow connectivity between online museum catalogues, and thus collections, is still a desideratum. 

In addition to this, online museum catalogues and corresponding digital collections have been allowing users to leverage computational methods like machine learning, computer vision, text mining, visualization, and network analysis. However, the outcomes of these computational attempts have not been questioned about the degree of bias they contained, assuming that collections and catalogues are unbiased.

Museum online catalogues-as-data draws inspiration from recent GLAM initiatives on the area of Collections-as-data (Padilla et al 2018) and highlights one of the most important topics in digital cultural heritage and digital scholarship today: connectivity/functionality. 


## Research Questions

- Why can't we link different online museum catalogues and collections efficiently and easily? What would be the useful joining points? What would be required to produce these links?
  
- What are the strengths and weaknesses of the underlying data, for what type of usage, and how can we address those weaknesses ?


Through this investigation we seek to assess online museum catalogues-as-data, by assessing existing literature on digital cataloguing practices and user/audience needs as well as by tracing data disparities and gaps by (historical) cataloguing practices, as found in online museum catalogues, using the Science Museum Group online catalogue as case-study. 

## People

#### Anna-Maria Sichani 
Conceptualization, Data curation, Formal analysis, Methodology, Software, Writing- original draft & editing 

#### Jaimie Unwin 
Conceptualization, Methodology, Software, Writing – review & editing

#### John Stack 
Writing – review & editing

#### Kunika Kono 
Software, Writing – review & editing

--

In this repository you can find :

* the SMG objects dataset can be found in [SMG's datasets repository](https://github.com/congruence-engine/datasets/blob/main/smg/smg_objects.md).
* [SMG dataset mapping.xlsx](https://github.com/congruence-engine/catalogues-as-data/blob/main/SMG%20dataset%20mapping.xlsx): The key fields identified by [@amsichani](https://github.com/amsichani) for analysis.
* [smg_objects_06_06_2022_extracted.json]: Dataset containing only the key fields extracted from the SMG objects dataset.
* [smg_objects_06_06_2022_extracted_converted.json]: Copy of smg_objects_06_06_2022_extracted.json as converted to regular JSON.
* [smg_objects.ipynb](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects.ipynb): Jupyter Notebook containing the code used for data extraction. For the purpose of this investigation, data was extracted as provided and no cleaning nor transformation was applied.


 
 The following are CSVs of each key fields (see [mapping](https://github.com/congruence-engine/catalogues-as-data/blob/main/SMG%20dataset%20mapping.xlsx), with nested fields flattened and extracted into separate columns and multi-value (array) field expanded into individual rows:
* [smg_objects_categories.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/data/smg_objects_categories.csv)
* [smg_objects_description.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/data/smg_objects_description.csv.zip)
* [smg_objects_lifecycle_creation_date.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/data/smg_objects_lifecycle_creation_date.csv)
* [smg_objects_materials.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/data/smg_objects_materials.csv)
* [smg_objects_name.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/data/smg_objects_name.csv)
* [smg_objects_title.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/data/smg_objects_title.csv.zip)

 


All the CSVs include object ids, which can be used to reconstruct the full extracted dataset e.g. by importing each CSV into a Pandas dataframe and joining/merging the dataframes on the [id] field. 

Read the [brief commentary on our data-focused work](https://github.com/congruence-engine/catalogues-as-data/blob/main/museum%20online%20catalogues-as-data_data-focused%20work.pdf).

## Report and Assesment framework/matrix
As part of this investigation a report alongside an assesment framework and matrix for museums' online catalogues has been produced.
This report aims to contribute towards the design and development of a sector-level strategy regarding the improvement and connectivity of online catalogues of cultural heritage institutions as part of a national collection’s infrastructure. Through the investigation we embark on exploring and demystifying common practices in museum online catalogues, aiming to reveal potential obstacles that suspend their connectivity and advanced use from various users.The first part of the report offers a state-of-the-art of digital cataloguing practices in the museum sector. The second part focuses on specific technical challenges, found in online museum catalogues, by introducing a sector-specific assessment framework through a combination of empirical research and landscape analysis. For this framework we employed Science Museum Group (SMG) online collection catalogue as a case study to showcase existing challenges and limitations. Finally, in the third part a minimum technical passive provision is explored in order to serve as a foundational infrastructure for drawing together a cultural heritage national collection. The Appendix hosts two questions-as-provocations that we invite the Congruence Engine team to consider further. 

Read here the [full report](https://github.com/congruence-engine/catalogues-as-data/blob/main/museum%20online%20catalogues-as-data_report_FINAL.pdf).


Please get in touch if with [Anna-Maria](mailto:annamaria.sichani@sas.ac.uk) or [Jamie](mailto:jamie.unwin@sciencemuseum.ac.uk) if you are interested in our work - we 'd love to hear from you.
