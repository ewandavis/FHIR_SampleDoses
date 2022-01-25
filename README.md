#NHS Digital Sample Dosages Work Package

This repository contains the data files used by and created as part of the NHS Digital Sample Dosages Work Package

THIS IS WORK IN PROGRESS AND ONLY PROVIDE FOR CHECKING

##OrderSentences.xls

This contains the source data in columns (black column names) and data generated from these (green column names)

Generated data includes Medication Order Sentences (column B) in both dose and product based form, indicated by the type in column A

Currently the latest version of the processing software is operating on data in the ‘BigSample’ tab.

##FHIR.json.fhir

This contains allthe the generated dosages in JSON FHIR format along with some debugging data.I know many of these are wrong.

##OrderSentences_Review.json.fhir

This contains a subset of generated dosages which I believe are correct or have only known issues

Know issues are it does not handle:

* Timing specified as **at least** before or after rather than a specific time
* Timing where **both** a time before and a time after are specified 
