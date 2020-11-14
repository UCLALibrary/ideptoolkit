---
layout: page
title: Descriptive Terms
menu: true
order: 3
lang: English
ref: terms
permalink: /terms
---
<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. Filename (Required) & Identifiers](#1-filename-required-identifiers)
- [2. Title (Required)](#2-title-required)
- [3. Creator / Contributor (Recommended)](#3-creator-contributor-recommended)
- [4. Publication information (Recommended)](#4-publication-information-recommended)
- [5. Date (Required)](#5-date-required)
- [6. Language (Required)](#6-language-required)
- [7. Type (Required)](#7-type-required)
- [8. Physical Description (Recommended)](#8-physical-description-required)
- [9.  Institution/Repository and Physical Collection information (Required)](#9-institutionrepository-and-physical-collection-information-required)
- [10. Rights (Required)](#10-rights-required)
- [11. Abstract and other Notes (Recommended)](#11-abstract-and-other-notes-recommended)
- [12. Subject terms(Recommended)](#12-subject-termsrecommended)
- [13. Digital Collection Title (Required)](#13-digital-collection-title-required)

<!-- /TOC -->

### 1. Filename (Required) & Identifiers
##### A. Filename (Required)
The filename of the object (ex. `arce_lrwp_0001.tiff`) is recorded in the "**Filename**" field. For file naming best practices, see the the "[File Naming & Organization Guide](https://uclalibrary.github.io/ideptoolkit/filenaming.html)."

##### B. Local ID (Recommended)
A **Local ID** is any identifier assigned locally. This can be a shelf-mark, item or catalog number, or in some cases the filename without the extension (ex. `arce_lrwp_0001`).

### 2. Title (Required)
The title of the resource being described. Titles may be transcribed or supplied. A transcribed title is taken from the resource. If there is no title inscribed on the resource, a title may be created by the metadata contributor, supplied by the creator or the owning institution, or taken from a reference work or another reliable source.

Do not include initial definite or indefinite articles in the title (The, A, An). Use standard title capitalization of the language used.

There are three types of titles:

#### A. Title (Original Language)
The primary title that will be used for sorting. This can be in English or in the language of the resource.

#### B. Translated Title (English language title)
Used for translations of the title. Titles in non-English languages should be translated into English here.

#### C. Alternative Title
Used if the work is known by another title or has a variant.

### 3. Creator / Contributor (Recommended)

#### A. Creator
The entity or entities primarily responsible for making the content of the resource (i.e. author, artist, etc).

#### B. Contributor
Those responsible for making contributions to the intellectual or artistic content, or the physical production and dissemination, of the resource (i.e. translator, editor, etc.).

##### Preferred sources for Creator and Contributor names:
* Virtual International Authority File (VIAF): [https://viaf.org](https://viaf.org)
* Library of Congress Name Authority File (LCNAF): [http://id.loc.gov/authorities/names.html](http://id.loc.gov/authorities/names.html)
* Getty Union List of Artists’ Names (ULAN): [http://www.getty.edu/research/tools/vocabularies/ulan/](http://www.getty.edu/research/tools/vocabularies/ulan/)

If a person’s name does not appear in an authority file, establish it following the form LASTname, FIRSTname or according to the convention of the original language. If an organization’s name does not appear in an authority file, use the organization’s full, preferred name (not an abbreviation, etc.).

```
EXAMPLES (Creator)
* Master of Saint Francis (Italian, active 2nd half of 13th century)
* Big Deal Design (Firm)
* Unknown Tahitian artist
* Koblecky, Jarko
```
```
EXAMPLES (Contributor)
* Landsforeningen for bøsser og lesbiske
* Dickinson, John
```

### 4. Publication information (Recommended)

The name and place of the publisher for published resources. Can also include volume and issue for periodicals.

#### A. Publisher
If the item is published, add the publisher name here. The publisher name should be taken from the resource if available. If no publisher is provided, but the publisher is known, use a standard naming authority file, such as:
* Library of Congress Subject Headings: [http://id.loc.gov/authorities/names.html](http://id.loc.gov/authorities/names.html)
* VIAF: [https://viaf.org](https://viaf.org)

#### B. Publisher.place
The name of the place where the resource was published. The form of the place name should be taken from the resource. When the object does not provide a place, but is known, use a standard naming authority file, such as:
* MARC List for Geographic Areas: [http://id.loc.gov/vocabulary/geographicAreas.html](http://id.loc.gov/vocabulary/geographicAreas.html)

#### C. volume/year
If the resource is a periodical (journal, newspaper, magazine), record the volume or year as it appears on the resource. For example, “vol. 2” or “1972”

```
EXAMPLES
* Vol. 2
* 1972
```

#### D. issue
If the resource is a periodical (journal, newspaper, magazine), record the issue number as it appears on the resource. For example, “no. 16”

```
EXAMPLES
* Issue 54
* no. 47
```

### 5. Date (Required)
A point or period of time associated with creation or publication of the resource.

Where exact dates are unknown, metadata contributors should provide a range of possible dates for the resource, such as the decade or century in which it was created or published.

#### A. Date (human) (Recommended)
This is a human-readable date that will display on the item view page.

#### B. Date.created [single OR start/end] (Required)
A machine-readable date suitable for processing (e.g. search limiting, results sorting), following the format `YYYY-MM-DD` (year-month-day).

In the metadata template spreadsheet, notice there are separate columns in the spreadsheet for a single date vs. a date range. Use the fields following the examples below:

*EXAMPLES*

| Date (human) | Date.created (single) | Date.created (start) | Date.created (end) |
| -- | -- | -- | -- |
| 1965 | 1965 | | |
| 1967-1985 | | 1967 | 1985 |
| August 02, 1969 | 1969-08-02 | | |
| Between 1967 and 1985 | | 1967 | 1985 |
| August 2001 | | 2001-08-01 | 2001-08-31 |
| 19th century | | 1801 | 1900 |
| July or August 1991 | | 1991-07 | 1991-08 |

### 6. Language (Required)
The language in which the content of the resource is expressed.

This field contains both the English term for the language as well as the ISO language codes, formatted as: `Armenian | arm`. For multilingual materials, each language featured should be entered into a separate column.

##### Preferred sources for Language codes:
* Codes for the representation of names of languages (ISO 639-3): [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)

For non-textual materials such as photographs, enter `zxx` (no linguistic content)
```
EXAMPLES
* Arabic | ara
* Japanese | jpn
```
** A bilingual newsletter in both Spanish and English should have two language columns - one column for `Spanish | spa` and another column for `English | eng`.

### 7. Type (Required)
The nature or genre of the content of the resource. To describe the file format, physical medium, or dimensions of the resource, use the Physical Description element below.

#### A. TypeOfResource
The general type of content of the resource. The metadata template contains a pull-down menu of the acceptable terms. An item can have only one (1) type.

```
TERMS
* still image
* sound recording
* text
* cartographic
* moving image
* three dimensional object
* software/multimedia
* mixed material
```

#### B. Genre
A category characterizing a particular style, form, or content, such as artistic, musical literary composition, etc. This qualifier allows for more specificity than the terms used in TypeOfResource. The metadata template contains a pull-down menu of the acceptable terms.

An item can have multiple genre terms. For multiple terms, separate the terms with the pipe character `|`. For example, `postcards | autographs`.

##### Preferred sources for Genre terms:
* Getty Art & Architecture Thesaurus Online (AAT): [http://www.getty.edu/research/tools/vocabularies/aat/](http://www.getty.edu/research/tools/vocabularies/aat/)

```
EXAMPLES
* posters
* periodicals
* postcards | autographs
* black-and-white photographs
```

### 8. Physical Description
The Physical Description element may be used to record information about the physical features of a resource, such as the extent, dimensions, and medium.

* **Extent** – Number of items, number of pages, or duration (length, such as seconds) of the resource. (May be the same whether referring to the original resource or the digital object.)

```
EXAMPLES
* 22 pp.
* 95 min.
```

* **Dimensions** – The measurements of the original resource, including its size or scale.

```
EXAMPLES
* 61 x 43 cm. (24 x 17 in.)
* 161.5 cm. (circumference, sphere)
```

* **Medium** – The material or physical carrier of the resource (i.e. the materials of which the resource is composed).

```
EXAMPLES
* pen and ink on paper
```

### 9.  Institution/Repository and Physical Collection information (Required)
#### A. Institution/Repository
The name of the repository where the physical resource is currently located.

##### Preferred sources for Organizational Names:
* Virtual International Authority File (VIAF): [https://viaf.org](https://viaf.org)
* Library of Congress Name Authority File (LCNAF): [http://id.loc.gov/authorities/names.html](http://id.loc.gov/authorities/names.html)

If an organization does not appear in an authority file, enter it according to the preferred form from the organization.

```
EXAMPLES
* MEDU Art Ensemble (Gaborone, Botswana)
* American Research Center in Egypt (Cairo, Egypt)
```

#### B. Physical or archival collection name
If items are part of a physical collection (e.g. archival),  enter the name of the physical collection.
```
EXAMPLES
* Salton Sea Photographic Scrapbooks
* Roman Wall Paintings at Luxor Temple  
```

#### C. Archival collection number or identifier
If items are part of a physical collection (e.g. archival),  enter the collection identifier (if any) for the physical collection.
```
EXAMPLES
* UCLASC 124
```

#### D. Box number / Folder number
If the archival collection is stored in boxes and folders, record the box and folder numbers in this field.
```
EXAMPLES
* box 26
* folder 4
```

### 10. Rights (Required)
Information about the creation and/or publication of a resource that is related to the intellectual property rights associated with the object.

**.copyrightStatus:** Choose from the list:
* copyrighted – the material is under copyright
* public domain – material is in the public domain (more specific public domain values follow)
* unknown – if the copyright status of an item is unknown

**.publicationStatus:** Choose from the list:
* published
* unpublished
* unknown

**.servicesContact:** Contact information for any services offered related to this item. Could be contact information for rights requests and/or requests for master images.
```
EXAMPLES
* National Library of Armenia, nla@library.nla.am
* UCLA Library Special Collections, speccoll@library.nla.am
```

### 11. Abstract and other Notes (Recommended)
An account of the content of the resource, and other descriptive information about the resource. Description may include information such as an abstract, table of contents, or a free-text account of the content.

#### A. Abstract (English and Original Language)
Used to record a succinct summary of the content or context of the resource.

#### B. Note (English and Original Language)
Used for information that is not encoded in another, more specific field.
```
EXAMPLES
* Inscription: "Longhaired" Palisades High School students protest school's demand that they get hair cut. [from caption on resource.]
* Physical description: Missing page 52
```

### 12. Subject terms(Recommended)
Any of the topics or themes of a work, essentially the “aboutness”. Subjects can be persons, organizations, places, topics, or time periods. If there are multiple subject terms, separate these using ` | ` (space pipe space).

##### Preferred sources for Subject Names:
* Virtual International Authority File (VIAF): [https://viaf.org](https://viaf.org)
* Library of Congress Name Authority File (LCNAF): [http://id.loc.gov/authorities/names.html](http://id.loc.gov/authorities/names.html)
* Getty Union List of Artists’ Names (ULAN): [http://www.getty.edu/research/tools/vocabularies/ulan/](http://www.getty.edu/research/tools/vocabularies/ulan/)

If a name does not appear in an authority file, enter it using the format in the examples below.
```
EXAMPLES
* Antoniani, Pietro, d ca. 1740-1805
* Institute without Boundaries
```

##### Preferred sources for Subject Places:
* MARC List for Geographic Areas: [http://id.loc.gov/vocabulary/geographicAreas.html](http://id.loc.gov/vocabulary/geographicAreas.html)

```
EXAMPLES
* Armenia (Republic)
* Havana (Cuba)
```

##### Preferred sources for Subject Topics:
* Library of Congress Subject Headings (LCSH): [http://id.loc.gov/authorities/subjects.html](http://id.loc.gov/authorities/subjects.html)

```
EXAMPLES
* Fruit crate labels
* Depression (Mental state)
* Regional planning
```

##### Preferred sources for Subject Time Periods (Temporal):
* PeriodO: [https://test.perio.do/#/p/Canonical/](https://test.perio.do/#/p/Canonical/)

```
EXAMPLES
* Tetrarchy (284-313 AD)
* New Kingdom Egypt (1548-1086)
```

### 13. Digital Collection Title (Required)

The title of the digital collection as it will appear on the IDEP website. This field allows users to limit their search/browse to a specific collection and will display under the “Collections” facet in the search interface.
```
EXAMPLES
* Soviet Armenian Posters
* Carteles de Cine
```
