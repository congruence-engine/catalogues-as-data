# _Museums' online catalogue-as-data_ investigation

## Data and code 

The 'Museums' online catalogue-as-data' investigation was developed by [@amsichani](https://github.com/amsichani) and [@jamieu](https://github.com/jamieu) as part of the [Congruence Engine](https://www.sciencemuseumgroup.org.uk/project/the-congruence-engine/) project. The investigation started with an interest to explore the museum (online) catalogues from a technical and data-point of view, in order to assess potential obstacles and weaknesses to the catalogues’ underlying data that limit their linking with other museums’ collections and records. In order to do a first assessment, we use the SMG catalogue dataset as a case-study. [@kunika](https://github.com/kunika) supported in various aspects with data/code - thanks!- and [@johnstack](https://github.com/johnstack) followed the investigation with a critical eye - cheers!.

In this repository you can find :

* the SMG objects dataset as uncompressed/unzipped file can be found here : [smg_objects_06_06_2022.json](https://github.com/congruence-engine/datasets/blob/main/smg/smg_objects.md) 
* [SMG dataset mapping.xlsx](https://github.com/congruence-engine/catalogues-as-data/blob/main/SMG%20dataset%20mapping.xlsx): The key fields identified by AMS for analysis.
* [smg_objects_06_06_2022_extracted.json]: Dataset containing only the key fields extracted from the SMG objects dataset.
* [smg_objects_06_06_2022_extracted_converted.json]: Copy of smg_objects_06_06_2022_extracted.json as converted to regular JSON.
* [smg_objects.ipynb](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects.ipynb): Jupiter Notebook containing the code used for data extraction. Data was extracted and exported as provided, no cleaning nor transformation was applied.
 
 The following are CSVs of each key fields (see [mapping](https://github.com/congruence-engine/catalogues-as-data/blob/main/SMG%20dataset%20mapping.xlsx), with nested fields flattened and extracted into separate columns and multi-value (array) field expanded into individual rows:
* [smg_objects_categories.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects_categories.csv)
* smg_objects_description.csv
* [smg_objects_lifecycle_creation_date.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects_lifecycle_creation_date.csv)
* [smg_objects_materials.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects_materials.csv)
* [smg_objects_name.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects_name.csv)
* [smg_objects_title.csv]

 
N.B. Column names are in dot notation format, based on field data structure e.g. [smg_objects_categories.csv](https://github.com/congruence-engine/catalogues-as-data/blob/main/smg_objects_categories.csv):
| JSON                                | CSV |
| ------------------------------------| ---------------------- |
| "categories": [                     |                 |  
|    {                                |                    |
|       "museum": "SCM"               |  category.museum    |
|"name": "Veterinary Medicine"        |  category.name    |
| "value": "SCM - Veterinary Medicine"|   category.value   |
| }
]


All the CSVs include object ids, which can be used to reconstruct the full extracted dataset e.g. by importing each CSV into a Pandas dataframe and joining/merging the dataframes on the [id] field. 

Read the [brief commentary on our data-focused work](https://github.com/congruence-engine/catalogues-as-data/blob/main/museum%20online%20catalogues-as-data_data-focused%20work.pdf).

## Report and Assesment framework/matrix
As part of this investigation a report alongside an assesment framework and matrix for museums' online catalogues has been produced.
This report aims to contribute towards the design and development of a sector-level strategy regarding the improvement and connectivity of online catalogues of cultural heritage institutions as part of a national collection’s infrastructure. Through the investigation we embark on exploring and demystifying common practices in museum online catalogues, aiming to reveal potential obstacles that suspend their connectivity and advanced use from various users.The first part of the report offers a state-of-the-art of digital cataloguing practices in the museum sector. The second part focuses on specific technical challenges, found in online museum catalogues, by introducing a sector-specific assessment framework through a combination of empirical research and landscape analysis. For this framework we employed Science Museum Group (SMG) online collection catalogue as a case study to showcase existing challenges and limitations. Finally, in the third part a minimum technical passive provision is explored in order to serve as a foundational infrastructure for drawing together a cultural heritage national collection. The Appendix hosts two questions-as-provocations that we invite the Congruence Engine team to consider further. 

Read here the [report](https://github.com/congruence-engine/catalogues-as-data/blob/main/museum%20online%20catalogues-as-data_report_FINAL.pdf).


Please get in touch if with [Anna-Maria](annamaria.sichani@sas.ac.uk) or [Jamie](jamie.unwin@sciencemuseum.ac.uk) if you are interested in our work - we 'd love to hear from you.
