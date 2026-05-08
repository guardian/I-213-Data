# I-213 Data 

This is a repo containing data on I-213 forms, covering FY 2022 through August 2025. 

Here is a Drive link to the [data](https://drive.google.com/drive/folders/1LWRrNh3Qfyd-2YYBBls8hMkCiYns-wMd?usp=drive_link).

The Guardian sued for access to bulk I-213 forms and in December 2025, DHS released the data as a part of on-going FOIA litigation. 

I-213 forms are legal documents that the government files in immigration court to prove that a person is in the country illegally. The data has details on each person, including the number of minor children they have and criminal history. 

This data has been minimally processed to remove potentially identifiable information. If you feel that you need these columns, please get in touch. 

Columns that we removed are:
- HAIR_COLOR_CODE
- EYE_COLOR_CODE
- COMPLEXION_CODE
- HEIGHT
- WEIGHT
- BIRTH_CITY_NAME
- APP_LDMK_OTHER_COMMENT_TEXT

Many fields are the same as those included in the Deportation Data Project, so consult [their documentation as well](https://deportationdata.org/docs/ice.html).

If you make use of this data, please cite the Guardian and [let me know](mailto:will.craft@theguardian.com). I will include a link to stories here.


#### Links

###### News stories using I-213 data
[Worst of the worst? Most US immigrants targeted for deportation in 2025 had no criminal charges, documents reveal](https://www.theguardian.com/us-news/2026/feb/22/us-immigration-trump-administration), The Guardian

[Revealed: The Trump administration arrested the parents of at least 27,000 kids in seven months](https://www.theguardian.com/us-news/ng-interactive/2026/may/08/trump-administration-parents-arrested)

[Trump Has Detained the Parents of More Than 11,000 U.S. Citizen Kids](https://www.propublica.org/article/trump-family-deportations-ice-citizen-kids), ProPublica

[After Trump called Portland ‘war-ravaged,’ ICE apprehensions near the city spiked 600%](https://www.opb.org/article/2026/03/13/oregon-portland-ice-apprehensions-multnomah-washington-marion/), Oregon Public Broadcasting

###### Studies and documents
[New Data on PNW Immigration Enforcement Reveal Powerful Surge in Late 2025](https://jsis.washington.edu/humanrights/2026/03/11/new-data-on-pnw-immigration-enforcement-reveal-powerful-surge-in-late-2025/), University of Washington Center for Human Rights

[I-213 Analysis](https://github.com/UWCHR/i-213-analysis), University of Washington Center for Human Rights

[What to do when ICE submits an I-213 in immigration court](https://www.ilrc.org/sites/default/files/2023-12/What%20to%20Do%20When%20ICE%20Submits%20an%20I-213%20In%20Immigration%20Court.pdf), Imigration Legal Resource Center

[ICE 287 (G) Participant Workbook - I-213 Preparation](https://www.scribd.com/document/21968656/ICE-287-g-Participant-Workbook-I-213-Preparation)

#### Column definitions 
Column | Definition
---|---
SITE_CODE | Three letter code designating the ICE sub-field office. 
SITE_NAME | Name of the ICE sub-field office. 
AREA_OF_RESPONSIBILITY_CODE | Three letter code for the ICE Area of Responsibility (AOR).
AREA_OF_RESPONSIBILITY_NAME | AOR full name.
DOCUMENT_TYPE_DESCR | Document type. Every entry is `I-213 (NEW 4/1/97) - Record of Deportable/Inadmissible Alien`
DOC_COMPLETION_DATE | Date document was completed.
PROCESSING_DISPOSITION_DESCR | Processing disposition at the time of apprehension. For details see: https://deportationdata.org/docs/ice.html
CITIZENSHIP_COUNTRY_DESCR | Citizenship country.
GENDER_CODE | Gender. ICE uses three values: `M`, `F`, `U` 
AGE | Age
BIRTH_COUNTRY_DESCR | Birth country
MARITAL_STATUS_DESCR | Marital status
OCCUPATION_TEXT | Occupation. This is a messy column, and [page 5](https://www.scribd.com/document/21968656/ICE-287-g-Participant-Workbook-I-213-Preparation) of the 287g I-213 instruction manual says to fill it out as "laborer" if the person worked multiple jobs. 
APPREHENSION_DATE | Date of initial apprehension.
APPREHENSION_METHOD_DESCR | Method of apprehension. For details see: https://deportationdata.org/docs/ice.html 
APPREHENSION_LANDMARK_DESCR | General description of where the person was apprehended.
ENTRY_DATE | Date of entry into the US.
ENTRY_PORT_OF_ENTRY_CODE | Code for the port of entry into the US.
ENTRY_PORT_OF_ENTRY_DESCR | Description of the port of entry.
ENTRY_ADMISSION_CLASS_DESCR | Legal category for admissibility. 
MOTHER_CITIZENSHIP_COUNTRY_DESCR | Citizenship of the apprehended person's mother.
FATHER_CITIZENSHIP_COUNTRY_DESCR | Citizenship of the apprehended person's father.
SPOUSE_CITIZENSHIP_COUNTRY_DESCR | Citizenship of the person's spouse.
HEALTH_STATUS_COMMENT_TEXT | Indicates the person's answer to a question on their health status.
ADMIN_CHARGES | Administrative charges, in JSON format.
CRIMINAL_CHARGES | Criminal charges, in JSON format.
CHILD_COUNT | Number and nationality of minor children, in JSON format. 
