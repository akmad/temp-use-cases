# INST-USCT-1 - Unconditional Social Cash Transfer

## Product Use Case Summary

| ID      | INST-USCT-1                        |
| ------- | ---------------------------------- |
| Name    | Unconditional Social Cash Transfer |
| Sector  | Institution                        |
| Version | 1.0                                |
| Status  | Draft                              |

This use case profiles specifically the digital integration steps within the delivery journey of a generalized unconditional social cash transfer service. Unconditional cash transfers are cash payments provided to financially disadvantaged or vulnerable people or households without requiring anything in return (i.e. without conditionality). This is different from a conditional payment where the benefit needs to be applied on the basis of achieving a certain result (e.g. higher school attendance, or prenatal care visit), or to be expended specifically on a type of resource (e.g. housing, or agricultural equipment). Governments in low- and middle-income countries increasingly use these benefit schemes in attempt to reduce poverty or other vulnerabilities, such as those related to health.

## SDG Targets

* 16.6: Develop effective, accountable and transparent institutions at all levels&#x20;
* SDG Target 2: Target description

## Actors

* Name: Description
* Name: Description

## Steps

### 1 - Outreach Communications

Staff from the Ministry of Social Welfare or another leading agency / organization organizes an information campaign to inform about a social assistance programme aimed at potential target population / beneficiary group(s) and implemented via predefined approaches and partners. The campaign is conveyed via mobile messaging and/or aired on national radio/television, while a more capillary village to village campaign is performed by district / local social welfare officers. Outreach communication is intensive during the kick-off phase of the new programme, but also requires ongoing touchpoints and additional information sharing, e.g. on grievance procedures, rights and responsibilities, behavioural change communication, etc.

#### Building Block Workflows

**Messaging**

* Workflow 1

**Scheduling**

* Workflow 1

### 2 - Registration

Registration is the process of collecting information on potential beneficiaries for assessment of their needs and conditions. Depending on specific country context, registration works in very different ways – either through mass-census survey, or on-demand at local offices (either approach potentially building on interoperability existing data sources). While the practicalities of data collection differ across the two, with very different implications for data quality, currency and completeness, the underlying digital processes are broadly the same: Mass census survey registration is sometimes carried out in-house, other times by statistics agency or trained enumerators. A percentage\* of households across the country are interviewed on a periodic basis to collect socio-economic data (especially if to target population in poverty), geo-location data, and key documentation. On-demand registration is primarily carried out in-house via capacity at local levels of implementation (e.g. social welfare offices or municipalities) and involves people pro-actively applying when in need. In either case data (both at individual and household-levels) is entered into a registry that serves one social assistance programme alone or several: the Social Registry\*\* (SRIS). This is sometimes done directly at the moment of interview via computer assisted interview methods (CAPI), other times subsequently post-enumeration.

\* Percentage varies greatly across countries; 10-95% range depending on prior policy choices, etc.

\*\* The Social Registry collects, organizes, stores, processes, transforms, creates, and distributes information necessary to support intake and registration of potential beneficiaries (gateway function). It is part of a broader Social Assistance Information System, further discussed below and in subsequent steps.

#### Building Block Workflows

****[**Consent**](https://govstack.gitbook.io/bb-consent/)****

* [4.4.1 Consenting at initial registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.1-consenting-at-initial-registration-pre-registration-using-a-centralised-id-system)
* [4.4.2 Consenting after the registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.2-consenting-after-the-registration-post-registration)

****[**Registration**](https://govstack.gitbook.io/bb-registration/)****

* [8.2 Using a Registration Service](https://govstack.gitbook.io/bb-registration/8-workflows#docs-internal-guid-6bac7ec4-7fff-2f07-f48f-168981104eec)

****[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)****

* [6.1 Identity Registration](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-54ffa6d1-7fff-1219-8f59-d45ca47b2ad7)
* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

### 3 - Data Verification and Validation

Data within the SRIS Social Registry Information System (SRIS) is generally checked\* by central level Social Welfare Ministry managers, against other government databases (eg. ID, tax, land cadastre, etc.) in order to fill in any missing gaps, verify and validate collected information, including authentication of all records. \*Data checking approaches also vary: sometimes batch-sharing via CD, sometimes full interoperability

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

### 4 - Eligibility Determination and Benefit Package(s) Design

NOTE: Depending on the country and programme, eligibility determination takes different forms e.g. categorical by age without income screening , poverty-targeted, etc. often via “Proxy Means Test” calculation to screen and rank households by ‘inferred’ income. "Clean" data from a Social Registry that have undergone the data verification and validation step is used to screen eligible beneficiaries and establish the recommended benefit and services ‘package’. The amount of transfer often varies depending on household composition, and beneficiaries may qualify for other add-on services based on analyzed socioeconomic / demographic information being used for other welfare or social programmes.

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

### 5 - Enrollment

Eligible beneficiaries are re-contacted and asked to enroll onto the programme. During enrolment, further data can be collected (depending on programme design) e.g. bank account details, biometrics, etc.. Further information is exchanged and, in certain program design or context, beneficiaries are issued with a programme card (depending on system setup by country). Programme specific data is often entered into a separate Beneficiary Registry associated with a Beneficiary Operations Management System (BOMS)\*, not the Social Registry used during Step 1. Registration. Non-eligible households are also contacted and informed, depending on program and context.

* Much of the literature on the topic refers to this as the programme’s Management Information System (MIS). In practice, this is a tailored software application that supports beneficiary management functions (e.g. enrolment, payments, case management, M\&E etc.).

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

### 6 - Payment

If a social cash transfer programme has enabled electronic payment processes (e.g. via banks, mobile money, etc.), payments are subsequently paid cyclically according to the programme schedule e.g. often bi-monthly. In the context where a digital financial service system is not employed, each beneficiary would be requested to travel to the nearest designated pay-point\* and collect money by programme-specific authentication. In either case, the money is transferred to the selected payment provider as per generated payroll and is subsequently verified against the individual’s identification of program enrollment. Other possible add-on intervention activities at this step: behaviour change communication; triggering of add-on benefits (or widening of beneficiary pool) in emergency context using GIS data, etc.

* These vary depending on design / implementation choices: banks, armoured vehicles, post offices, schools, etc.

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

### 7 - Ongoing Case Management

Depending on the programme and on the country’s broader social protection policies, this step involves ongoing interaction with beneficiaries via local social welfare officers to help: Ensure information on beneficiaries stays up to date Address complaints, grievances, and appeals Address multi-dimensional risks via connecting beneficiaries to other programmes and services e.g. child protection, etc. Carry out assessment of co-responsibilities / conditionalities, if any (this is achieved in some countries via data integration into e.g. school management system from Education ministry on attendance, or HIS from Health ministry on check-up, etc.) Note that this step also requires clarity, clear decisions, and protocols regarding whose data (or subset of such) is to be updated by which programme personnel or role and at what time.

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

### 8 - Ongoing M\&E

Central level managers and local social welfare officers base decisions and management choices (e.g. where to conduct add-on training, re-registration camps, where to prioritise budget, etc.) on up-to-date data on the programme/s (e.g. who receives what, when, what areas are performing better, etc). Note that countries that do this effectively ensure programme BOMS data is connected / integrated via an Integrated Beneficiary Registry\* and develop effective reporting functions, including GIS enabled spatial reporting. \*This is a Registry that integrates data across existing Beneficiary registries and their associated BOMS to give an overview of who is receiving what across programmes.

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

### 9 - Updating

Ensuring data is up to date to trigger: Programme exit for those who are no longer eligible e.g. when a beneficiary dies, migrates, exceeds eligible age or no longer qualifies for other reasons. This is achieved via a combination of recertification campaigns, automated data updates, and data-sharing with other government databases e.g. civil registration for death. Programme entry for newly eligible beneficiaries, via new data collection or analysis etc. Other changes to entitlements (e.g. benefit type of transfer size) due to changes in household composition, incomes, etc. Note that this step also requires clarity, clear decisions, and protocols regarding whose data (or subset of such) is to be updated by which programme personnel or role and at what time.

#### Building Block Workflows

**BB 1**

* Workflow 1

**BB 2**

* Workflow 1

## Outputs

1. Description

## Failure Points

1. Description. Result (optional)
