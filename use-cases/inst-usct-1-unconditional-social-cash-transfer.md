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

* [1.3](https://solutions.dial.community/sdgs/no\_poverty): Implement nationally appropriate social protection systems and measures for all, including floors, and by 2030 achieve substantial coverage of the poor and the vulnerable
* [16.6](https://solutions.dial.community/sdgs/peace\_justice\_and\_strong\_institu): Develop effective, accountable and transparent institutions at all levels&#x20;

## Building Blocks

* [Consent](https://govstack.gitbook.io/bb-consent)
* [Identification and Verification](https://govstack.gitbook.io/bb-identity)
* [Messaging](https://govstack.gitbook.io/bb-messaging/)
* [Payments](https://govstack.gitbook.io/bb-payments)
* [Registration](https://govstack.gitbook.io/bb-registration)
* [Scheduling](https://govstack.gitbook.io/bb-scheduler/)
* [Workflow and Algorithm](https://govstack.gitbook.io/bb-workflow)

Future building block inclusion

* Analytics and Business Intelligence
* Artificial Intelligence
* Client Case Management
* Data Collection
* Geographic Information Services (GIS)
* Reporting and Dashboards
* Shared Data Repositories
* Terminology

## Steps

### 1 - Outreach Communications

Staff from the Ministry of Social Welfare or another leading agency / organization organizes an information campaign to inform about a social assistance programme aimed at potential target population / beneficiary group(s) and implemented via predefined approaches and partners. The campaign is conveyed via mobile messaging and/or aired on national radio/television, while a more capillary village to village campaign is performed by district / local social welfare officers. Outreach communication is intensive during the kick-off phase of the new programme, but also requires ongoing touchpoints and additional information sharing, e.g. on grievance procedures, rights and responsibilities, behavioural change communication, etc.

#### Workflows

* **Client communication** to facilitate the spreading of programme awareness for target audience and encouraging enrolment via mobile / media channel(s)
* **Client education** for educating potential target beneficiaries around the approach and objective(s), benefit(s), constraint(s), partner(s), etc. of the programme
* **Content management** for the backend Social Welfare staff to populate relevant educational and promotional content that local officers can use during on-the-ground outreach campaigns
* **Identification and Registration** (with aid of geographic information services tool **** for potential use) in mapping and locating households and individuals for outreach target

#### Building Block Workflows

****[**Messaging**](https://govstack.gitbook.io/bb-messaging/)****

* [9.3.1 Government/BB to Person communication](https://govstack.gitbook.io/bb-messaging/9-workflows#7.3.1-government-bb-to-person-communication)

****[**Scheduling**](https://govstack.gitbook.io/bb-scheduler/)****

* [UseCase-2 Periodic Payroll and Payments Event scheduling : Post-Partum Care & Unconditional Social Benefit transfer programs](https://govstack.gitbook.io/bb-scheduler/9-workflows#usecase-2-periodic-payroll-and-payments-event-scheduling-post-partum-care-and-unconditional-social-b)

**Mobility Management**

* Future Workflow

### 2 - Registration

Registration is the process of collecting information on potential beneficiaries for assessment of their needs and conditions. Depending on specific country context, registration works in very different ways – either through mass-census survey, or on-demand at local offices (either approach potentially building on interoperability existing data sources). While the practicalities of data collection differ across the two, with very different implications for data quality, currency and completeness, the underlying digital processes are broadly the same: Mass census survey registration is sometimes carried out in-house, other times by statistics agency or trained enumerators. A percentage\* of households across the country are interviewed on a periodic basis to collect socio-economic data (especially if to target population in poverty), geo-location data, and key documentation. On-demand registration is primarily carried out in-house via capacity at local levels of implementation (e.g. social welfare offices or municipalities) and involves people pro-actively applying when in need. In either case data (both at individual and household-levels) is entered into a registry that serves one social assistance programme alone or several: the Social Registry\*\* (SRIS). This is sometimes done directly at the moment of interview via computer assisted interview methods (CAPI), other times subsequently post-enumeration.

\* Percentage varies greatly across countries; 10-95% range depending on prior policy choices, etc.

\*\* The Social Registry collects, organizes, stores, processes, transforms, creates, and distributes information necessary to support intake and registration of potential beneficiaries (gateway function). It is part of a broader Social Assistance Information System, further discussed below and in subsequent steps.

#### Workflows

* **Data Collection and Reporting** for capturing interview responses or observation during registration process
* **Identification and Registration** for enrolled identified beneficiaries in the system and enabling possible permissions for interaction with the SRIS, and (with aid of geographic information services tool) to potentially locate and track households during the interview process
* **Client Case Management** for creating beneficiary user records

#### Building Block Workflows

[**Consent**](https://govstack.gitbook.io/bb-consent/)

* [4.4.1 Consenting at initial registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.1-consenting-at-initial-registration-pre-registration-using-a-centralised-id-system)
* [4.4.2 Consenting after the registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.2-consenting-after-the-registration-post-registration)

[**Registration**](https://govstack.gitbook.io/bb-registration/)

* [8.2 Using a Registration Service](https://govstack.gitbook.io/bb-registration/8-workflows#docs-internal-guid-6bac7ec4-7fff-2f07-f48f-168981104eec)

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.1 Identity Registration](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-54ffa6d1-7fff-1219-8f59-d45ca47b2ad7)
* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

### 3 - Data Verification and Validation

Data within the SRIS Social Registry Information System (SRIS) is generally checked\* by central level Social Welfare Ministry managers, against other government databases (eg. ID, tax, land cadastre, etc.) in order to fill in any missing gaps, verify and validate collected information, including authentication of all records. \*Data checking approaches also vary: sometimes batch-sharing via CD, sometimes full interoperability

#### Workflows

* **Client Case Management** for storing and reviewing identification records and eligibility information of potential beneficiaries
* **Data Analysis and Business Intelligence** for cross-referencing and verifying records across multiple registry sources, and reconciling gaps / overlaps

\
**Building Block Workflows**

[**Consent**](https://govstack.gitbook.io/bb-consent/)

* [4.4.2 Consenting after the registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.2-consenting-after-the-registration-post-registration)

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

**Client Case Management**

* Future workflow

**Analytics and Business Intelligence**

* Future workflow

### 4 - Eligibility Determination and Benefit Package(s) Design

NOTE: Depending on the country and programme, eligibility determination takes different forms e.g. categorical by age without income screening , poverty-targeted, etc. often via “Proxy Means Test” calculation to screen and rank households by ‘inferred’ income. "Clean" data from a Social Registry that have undergone the data verification and validation step is used to screen eligible beneficiaries and establish the recommended benefit and services ‘package’. The amount of transfer often varies depending on household composition, and beneficiaries may qualify for other add-on services based on analyzed socioeconomic / demographic information being used for other welfare or social programmes.

#### Workflows

* **Client Case Management** for determining and assigning benefit packages and benefit levels to specific user groups
* **Data Analysis and Business Intelligence / Decision Support** potentially for identifying different benefit levels / types in correlation to target groups’ socioeconomic / demographic information, based on existing eligibility criteria (e.g. via proxy means test, means test or category-based)

#### Building Block Workflows

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

**Client Case Management**

* Future workflow

**Analytics and Business Intelligence**

* Future workflow

**Artificial Intelligence**

* Future workflow

### 5 - Enrollment

Eligible beneficiaries are re-contacted and asked to enroll onto the programme. During enrolment, further data can be collected (depending on programme design) e.g. bank account details, biometrics, etc.. Further information is exchanged and, in certain program design or context, beneficiaries are issued with a programme card (depending on system setup by country). Programme specific data is often entered into a separate Beneficiary Registry associated with a Beneficiary Operations Management System (BOMS)\*, not the Social Registry used during Step 1. Registration. Non-eligible households are also contacted and informed, depending on program and context.

* Much of the literature on the topic refers to this as the programme’s Management Information System (MIS). In practice, this is a tailored software application that supports beneficiary management functions (e.g. enrolment, payments, case management, M\&E etc.).

#### Workflows

* **Data Collection and Reporting** for capturing additional programmatic information on the beneficiaries during enrolment
* **Financial Services** for staging beneficiary account details for cash transfer processing
* **Identification and Registration** for identifying beneficiaries and confirming enrolment
* **Client Case Management** for storing program specific data for tracking

#### Building Block Workflows

[**Payments**](https://govstack.gitbook.io/bb-payments/)

* Unknown Workflow

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

[**Registration**](https://govstack.gitbook.io/bb-registration/)

* [8.2 Using a Registration Service](https://govstack.gitbook.io/bb-registration/8-workflows#docs-internal-guid-6bac7ec4-7fff-2f07-f48f-168981104eec)

**Client Case Management**

* Future workflow

**Artificial Intelligence**

* Future workflow

### 6 - Payment

If a social cash transfer programme has enabled electronic payment processes (e.g. via banks, mobile money, etc.), payments are subsequently paid cyclically according to the programme schedule e.g. often bi-monthly. In the context where a digital financial service system is not employed, each beneficiary would be requested to travel to the nearest designated pay-point\* and collect money by programme-specific authentication. In either case, the money is transferred to the selected payment provider as per generated payroll and is subsequently verified against the individual’s identification of program enrollment. Other possible add-on intervention activities at this step: behaviour change communication; triggering of add-on benefits (or widening of beneficiary pool) in emergency context using GIS data, etc.

* These vary depending on design / implementation choices: banks, armoured vehicles, post offices, schools, etc.

#### Workflows

* **Financial Services** for processing beneficiary payment directly to their account, or for generating payroll to deposit payment amounts for withdrawal by beneficiary from designated banking institution(s) / pay-point(s) thereafter
* **Client Case Management** for identifying and authenticating individual that is making a withdrawal, or to recall / verify deposit account information prior to payment transaction

#### Building Block Workflows

[**Payments**](https://govstack.gitbook.io/bb-payments/)

* [10.2.1 Bulk Disbursement for Unconditional Cash Transfer](https://govstack.gitbook.io/bb-payments/10-workflows#10.2.1-bulk-disbursement-for-unconditional-cash-transfer)

**Client Case Management**

* Future workflow

### 7 - Ongoing Case Management

Depending on the programme and on the country’s broader social protection policies, this step involves ongoing interaction with beneficiaries via local social welfare officers to help: Ensure information on beneficiaries stays up to date Address complaints, grievances, and appeals Address multi-dimensional risks via connecting beneficiaries to other programmes and services e.g. child protection, etc. Carry out assessment of co-responsibilities / conditionalities, if any (this is achieved in some countries via data integration into e.g. school management system from Education ministry on attendance, or HIS from Health ministry on check-up, etc.) Note that this step also requires clarity, clear decisions, and protocols regarding whose data (or subset of such) is to be updated by which programme personnel or role and at what time.

#### Workflows

* **Data Collection and Reporting** for capturing changes in beneficiary information
* **Client Case Management** for identifying and recording beneficiary interaction with local officers and capturing reported cases on grievances / appeals etc., and for determining risks / conditionality by reviewing individual beneficiary client case
* **Work Planning and Coordination** to potentially suggest and connect with departments / agencies offering other social benefits and services to eligible beneficiaries

#### Building Block Workflows

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

[**Consent**](https://govstack.gitbook.io/bb-consent/)

* [4.4.2 Consenting after the registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.2-consenting-after-the-registration-post-registration)

Data Collection

* Future workflow

Geographic Information Services (GIS)

* Future workflow

Scheduling

* Future workflow

**Workflow**

* Future workflow

### 8 - Ongoing M\&E

Central level managers and local social welfare officers base decisions and management choices (e.g. where to conduct add-on training, re-registration camps, where to prioritise budget, etc.) on up-to-date data on the programme/s (e.g. who receives what, when, what areas are performing better, etc). Note that countries that do this effectively ensure programme BOMS data is connected / integrated via an Integrated Beneficiary Registry\* and develop effective reporting functions, including GIS enabled spatial reporting. \*This is a Registry that integrates data across existing Beneficiary registries and their associated BOMS to give an overview of who is receiving what across programmes.

#### Workflows

* **Client Case Management** for ongoing monitoring and tracking of client performance, and integration to other registries for holistic view and reporting
* **Identification and Registration** (with aid of geographic information services tool for potential use) in tracking / locating areas in relation to level of activities and adherence, or client household location
* **Data Analysis and Business Intelligence** / **Decision Support** / **Data Collection and Reporting** to analyze, update, and report programme output / performance information&#x20;

#### Building Block Workflows

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

[**Consent**](https://govstack.gitbook.io/bb-consent/)

* [4.4.2 Consenting after the registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.2-consenting-after-the-registration-post-registration)

Data Collection

* Future workflow

Geographic Information Services (GIS)

* Future workflow

Scheduling

* Future workflow

**Workflow**

* Future workflow

### 9 - Updating

Ensuring data is up to date to trigger: Programme exit for those who are no longer eligible e.g. when a beneficiary dies, migrates, exceeds eligible age or no longer qualifies for other reasons. This is achieved via a combination of recertification campaigns, automated data updates, and data-sharing with other government databases e.g. civil registration for death. Programme entry for newly eligible beneficiaries, via new data collection or analysis etc. Other changes to entitlements (e.g. benefit type of transfer size) due to changes in household composition, incomes, etc. Note that this step also requires clarity, clear decisions, and protocols regarding whose data (or subset of such) is to be updated by which programme personnel or role and at what time.

#### Workflows

* **Data Collection and Reporting** for routine update of information on the beneficiary client base, and integration of other databases and systems for automated data update on client cases overtime
* **Client Case Management** for ongoing review of beneficiary case information
* **Data Analysis and Business Intelligence** / **Decision Support** to support identification of individuals for exit or entry based on analyzing change in programme-specific / socioeconomic data

#### Building Block Workflows

[**Identity and Verification**](https://govstack.gitbook.io/bb-identity/)

* [6.2 Identity Verification](https://govstack.gitbook.io/bb-identity/6-functional-requirements#docs-internal-guid-2affb3f5-7fff-fa73-9e68-7707b820858d)

[**Consent**](https://govstack.gitbook.io/bb-consent/)

* [4.4.2 Consenting after the registration](https://govstack.gitbook.io/bb-consent/9-workflows#4.4.2-consenting-after-the-registration-post-registration)

Data Collection

* Future workflow

Geographic Information Services (GIS)

* Future workflow

Scheduling

* Future workflow

**Workflow**

* Future workflow

## Outputs

1. To Do

## Failure Points

1. To Do
