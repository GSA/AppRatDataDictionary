# Application Rationalization Data Dictionary

## Table of Contents

 - [Introduction](https://github.com/AaronKoppel/AppRatDataDictionary/blob/main/README.md#introduction)
 - [Prerequisites](https://github.com/AaronKoppel/AppRatDataDictionary/blob/main/README.md#prerequisites)
 - [Usage](https://github.com/AaronKoppel/AppRatDataDictionary/blob/main/README.md#usage)
 - [Technical Schema](https://github.com/AaronKoppel/AppRatDataDictionary/blob/main/README.md#technical-schema)
 - [Download](https://github.com/AaronKoppel/AppRatDataDictionary/blob/main/README.md#download)
 - [References](https://github.com/AaronKoppel/AppRatDataDictionary/blob/main/README.md#references)

## Introduction

Current Maintainer: GSA’s IT Modernization division at <dccoi@gsa.gov>

The Application Rationalization Data Dictionary is a supplement to the [Application Rationalization Playbook](https://www.cio.gov/assets/files/Application-Rationalization-Playbook.pdf) to help agencies strategically and systematically identify business applications and determine which should be kept, replaced, retired, or consolidated.<sup>[1](#footnote1)</sup> This resource establishes standards for data exchanges designed to manage application rationalization. Standards for data exchanges in turn allow users and agencies to explore and collaborate on their application rationalization data.

## Prerequisites

The Application Rationalization Data Dictionary is a spreadsheet in .csv format and is best viewed in spreadsheet software. It may also be viewed in GitHub directly.

## Usage

It consists of 10 columns:

**ID1**
- The unique integer, 1 to 176, associated with a given data element

**ID2**
- Structured in three parts: before the first decimal, between the first and second decimal, and after the second decimal
- Corresponds to the structure the Application Rationalization Playbook
- The number before the first decimal corresponds to the step in Application Rationalization Playbook
- The number between the first and second decimal corresponds to the sub-step in the Application Rationalization Playbook
- The number after the second decimal indicates its occurrence within a given sub-step in the Application Rationalization 
- 3.1.13 to 3.1.35 draw from the five Functions of NIST's Cybersecurity Framework<sup>[2](#footnote2)</sup> 
- 4.1.1 to 4.1.88 draw from the Finance and IT Layers of the TBM Taxonomy<sup>[3](#footnote3)</sup> 

**Name**
- Name of the data element

**Description**
- Description of the data element

**Type**
- Format of required/requested data: integer, floating point, or text

**Values**
- Possible categories for a given data element when numbers represent categories

**Codes**
- Numeric data when numbers represent categories

**Required?**
- Declaration (yes or no) if the data element is required 

**Example**
- Example of data element

**Notes**
- Additional information of interest for users

It consists of 176 data elements listed in columns.

## Technical Schema

A JSON schema for machine-readable data interchanges is provided, along with test data which can be used to validate it. The schema may be integrated into government-wide data collection efforts such as Integrated Data Collection (IDC), which enables the Office of Management and Budget (OMB) to oversee implementation of the Data Center Optimization Initiative (DCOI).

Importantly, integration efforts must take into account differences in time intervals. For instance, while IDC is reported quarterly, IDC Strategic Plans are reported in the spring IDC. Similarly, because the Application Rationalization Data Dictionary is intended to function on an annual basis, integration of the JSON schema should consistently occur at the end of only one IDC quarter per fiscal year.

## Download

To download the data dictionary and all related files, please click on the green "Code" button on the top right of the page, and then select "Download ZIP" from the dropdown menu. Alternatively, you can click [here](https://github.com/AaronKoppel/AppRatDataDictionary/archive/refs/heads/main.zip).

## References

<a name="footnote1">1.</a> Data Center and Cloud Optimization Initiative Program Management Office, The Application Rationalization Playbook (2020). CIO Council. https://www.cio.gov/assets/files/Application-Rationalization-Playbook.pdf.

<a name="footnote2">2.</a> National Institute of Standards and Technology, Cybersecurity Framework [Data file and code book] (2018). https://www.nist.gov/document/2018-04-16frameworkv11core1xlsx.

<a name="footnote3">3.</a> *TBM Taxonomy: Version 4.0*. TBM Council (2020, December 16). https://higherlogicdownload.s3.amazonaws.com/TBMCOUNCIL/c15d372f-9951-46c8-9c3f-213c696401b6/UploadedImages/TBM_Taxonomy_V4_0.pdf.
