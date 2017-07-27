---
layout: page
title: Descriptive Terms
menu: true
order: 3
---
<!-- TOC depthFrom:3 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 -->

- [1. Title (Required)](#1-title-required)
- [2. Filename & Identifiers](#2-filename-identifiers)
- [3. Creator / Contributor](#3-creator-contributor)
- [4. Publisher place (Recommended)](#4-publisher-place-recommended)
- [5. Date (Required)](#5-date-required)
- [6. Language (Required)](#6-language-required)
- [7. Type (Required)](#7-type-required)
- [8. Physical Description](#8-physical-description)
- [9. Institution/Repository (Required)](#9-institutionrepository-required)
- [10. Rights (Required)](#10-rights-required)
- [11. Description (Recommended)](#11-description-recommended)
- [12. Subject (Recommended)](#12-subject-recommended)
- [13. Relation (Recommended)](#13-relation-recommended)
- [14. Source (Recommended)](#14-source-recommended)

<!-- /TOC -->
### 1. Title (Required)
##### DEFINITION:

A word, phrase, character or group of characters that names the resource being described.

##### GUIDELINES for creating values for the TITLE element

Titles may be **transcribed**  or **supplied**. A transcribed title appears on the resource. If there is no title inscribed on the resource, a title may be constructed by the metadata contributor, supplied by the creator or the owning institution, or taken from a reference work or another reliable source. It is not necessary to supply square brackets to signify that a supplied title was not taken from the resource.

Do not include initial definite or indefinite articles in the title. Use standard American-style capitalization.

```
EXAMPLES
* Déjeuner sur l’Herbe [example of supplied title]
* Bacot family papers [supplied]
* Sonatas for violin and piano [transcribed]
* Australian aboriginal painting about AIDS [supplied]
* 1965 cityscape of Los Angeles looking northwest toward Santa Monica Mountains [supplied]
```

### 2. Filename & Identifiers
##### Filename (Required)

The filename of the object (ex. `arce_0001.tiff`) is recorded in the "**Filename**" field. For file naming best practices, see the the "[File Naming & Organization Guide](https://uclalibrary.github.io/ideptoolkit/filenaming.html)."

##### Identifier

An **Identifier** is a universal identifier such as ISBN, ISSN, DOI, or an OCLC number.

##### Local ID (Recommended)

A **Local ID** is any identifier assigned locally. This can be a shelf-mark, item or catalog number, or in some cases the filename without the extension (ex. `arce_0001`).

### 3. Creator / Contributor

The **CREATOR** element is **required** (if known), while the CONTRIBUTOR element is recommended.

##### DEFINITION:

CREATOR: The entity or entities primarily responsible for making the content of the resource (i.e. author, photographer, artist, etc). This element is required if the creator of a resource is known.

CONTRIBUTOR: Those responsible for making contributions to the intellectual or artistic content, or the physical production and dissemination, of the resource (i.e. publisher, translator, editor, distributor, etc.).

##### GUIDELINES for creating values for the CREATOR and CONTRIBUTOR elements

It is preferred to take the creator or contributor's name from a standard naming authority file. For IDEP collections, the preferred authority is the [Virtual International Authority File](https://viaf.org) (VIAF). If the name is not found in VIAF, other authority files, such as the Library of Congress Name Authority File (LCNAF), Union List of Artists’ Names (ULAN), or another national authority can be used. If a name does not appear in an authority file, you may establish it in the spreadsheet using the form `LASTname, FIRSTname`.

In the **Authority** column, indicate the code for the authority source from which the name was taken (VIAF, LCNAF, ULAN, etc.). If the name does not appear in an authority file, the source code should be "**local**."

In the case of multiple creators and/or contributors (of the same type), enter each name separated by `/` in the cell. For multiple contributor types (1 editor, 1 translator), enter the names into separate CONTRIBUTOR columns. Contributor columns must be qualified to indicate the role played (i.e. publisher, editor, etc.). There are a few options available in the template pull-down menu. If these do not accurately reflect the role, you may consult the [MARC Code List: Relator codes](https://www.loc.gov/marc/relators/relaterm.html) or the [ULAN role table](http://www.getty.edu/vow/ULANRolePopup).

If CREATOR is unknown, metadata contributors are strongly encouraged to make use of the **CONTRIBUTOR** element.

```
EXAMPLES (Creator)
* Master of Saint Francis (Italian, active 2nd half of 13th century) [example of artist’s name from ULAN]
* Big Deal Design (Firm) [designer’s name from LCNAF]
* Unknown Tahitian artist [artist’s name from local authority file (created according to CCO guidelines)]
```
```
EXAMPLES (Contributor)
* Landsforeningen for bøsser og lesbiske [publisher, from LCNAF]
* Dickinson, John [designer, from ULAN]
```

##### Standards and Guidelines

* [Virtual International Authority File](https://viaf.org) (VIAF) - **Preferred**
* [Library of Congress Name Authority File](http://authorities.loc.gov) (LCNAF)
* [Union List of Artists’ Names](http://www.getty.edu/research/tools/vocabularies/ulan/) (ULAN)

### 4. Publisher place (Recommended)

##### DEFINITION:

The name of the place where a resource has been published. (The name of the publisher itself is recorded in the **Contributor** element.)

##### GUIDELINES for creating values for the PUBLISHER PLACE element

The form of the place name should be taken from the object. When the object does not provide a place, use a standard naming authority file, such as the Thesaurus of Geographic Names (TGN) or the Library of Congress Name Authority file (LCNAF).

```
EXAMPLES
* Copenhagen (Denmark)
* Habana
```

##### Standards and Guidelines

* [Thesaurus of Geographic Names (TGN)](http://www.w3.org/TR/NOTE-datetime)
* [Library of Congress Name Authority file (LCNAF](http://authorities.loc.gov))

### 5. Date (Required)

##### DEFINITION:

A point or period of time associated with an event in the life cycle of the resource (e.g., creation, publication, printing, restoration, etc.).

##### GUIDELINES for creating values for the DATE element

Date information can be derived from the resource itself, or any reliable source, such as documentation related to the resource, etc. Where exact dates are unknown, metadata contributors should provide a range of possible dates for the resource, such as the decade or century in which it was created or published. Use the Description element to describe uncertainty when necessary.

When multiple types of dates are associated with a resource and not all of them are practical to record, the priority should be the type(s) that are most important to users. For example, the date a building was built is probably more important than the date it was photographed or the date the photo was digitized.

Metadata contributors should provide dates to an appropriate level of specificity for the resource. If an exact date or time for the resource is known, it should be provided.

##### Dates should be provided in two formats:

* **Display date:** suitable for display, i.e. `August 26, 2016`
* **Normalized date:** allows for machine processing (e.g. search limiting, results sorting). The normalized date follows the format `YYYY-MM-DD` - for example, `2016-08-26`.

| Examples | Display date | Normalized date |
| -- | -- | -- |
| Year of publication | 1965 | 1965 |
| Range of possible years | Between 1967 and 1985 | 1967/1985 |
| Date span | 1993-1995 | 1993/1995 |
| Exact date | October 26, 1969 | 1969-10-26 |
| Century | 19th century | 1801/1900 |
| Estimated date | July or August 1991 | 1991-07/1991-08 |

##### Standards and Guidelines
* [W3C: Date and time formats](http://www.w3.org/TR/NOTE-datetime)

### 6. Language (Required)
##### DEFINITION:

A designation of the language in which the content of the resource is expressed, or which is primary to understanding the resource. (Note: Not the language of the metadata record itself.)

##### GUIDELINES for creating values for the LANGUAGE element

Use the ISO 639-3 code for the language of the resource (see below).

If non-textual, code as '**zxx**'  (no linguistic content). If language cannot be determined, code as '**und**'  (a language that cannot be determined).
```
EXAMPLES
* ara [Arabic]
* eng [English]
* jpn [Japanese]
```
##### Other Standards and Guidelines
* [Codes for the representation of names of languages (ISO 639-3)](https://www.loc.gov/standards/iso639-2/php/code_list.php)

### 7. Type (Required)

##### DEFINITION:

The nature or genre of the content of the resource. To describe the file format, physical medium, or dimensions of the resource, use the Physical Description element.

##### GUIDELINES for creating values for the TYPE element

_Always include qualifiers for this element._

Required qualifiers:

**Type.collection** – Choose one of two values:

* yes – Record is for a collection of resources
* no – Record is for a single resource

**Type.manuscript** – Choose one of two values:

* yes – Resource being described is a manuscript
* no – Resource being described is not a manuscript

**Type.typeOfResource** – The general type of content of the resource. The metadata template contains a pull-down menu of the acceptable terms (text, still image, cartographic, sound recording, moving image, etc.)

**Type.genre** – A category characterizing a particular style, form, or content, such as artistic, musical literary composition, etc. This qualifier allows for more specificity than terms used in Type.typeOfResource. Use a controlled vocabulary (Art & Architecture Thesaurus Online [AAT] preferred) where possible; otherwise identify the term as a local heading.

```
EXAMPLES
* Type.collection: yes Type.manuscript: yes [Record for a collection of digitized manuscripts.]
* Type.collection: yes Type.manuscript: no [Record for a collection of digitized posters.]
* Type.collection: no Type.manuscript: yes [Record for a single digitized document (on its own, or as part of a larger collection).]
* Type.collection: no Type.manuscript: no [Record for a single digitized poster (on its own, or as part of a larger collection).]
* Type.typeOfResource: still image
* Type.typeOfResource: sound recording
* Type.genre: posters
* Type.genre: Periodicals
* Type.genre: Spaghetti Westerns
```
**Other Standards and Guidelines**

For **Type.genre:**

* ** Art & Architecture Thesaurus Online (AAT)** (preferred)
* Basic Genre Terms for Cultural Heritage Materials (BGTCHM)
* Library of Congress Subject Headings (LCSH)
* Rare Books and Manuscripts Section Controlled Vocabularies (RBMS)
* Thesaurus for Graphic Materials (TGM)

### 8. Physical Description

##### DEFINITION:

The physical medium, extent, or dimensions of the resource. This element is known in some metadata schemas as "format."

##### GUIDELINES for creating values for the PHYSICAL DESCRIPTION element

The Physical Description element may be used to record information about the resource: extent, dimensions, and medium.

**PhysicalDescription.extent** (Required ) -- Number of items, number of pages, or duration (length, such as seconds) of the resource. (May be the same whether referring to the original resource or the digital object.)

**PhysicalDescription.dimensions** (Recommended) -- The measurements of the original resource, including its size or scale.

**PhysicalDescription.medium** (Recommended) -- The material or physical carrier of the resource (i.e. the materials of which the resource is composed).

```
EXAMPLES
* PhysicalDescription.extent: 1 postcard
* PhysicalDescription.dimensions: 61 x 43 cm. (24 x 17 in.) [poster]
* PhysicalDescription.extent: 95 min. [film]
* PhysicalDescription.dimensions: 161.5 cm. (circumference, sphere) [globe]
* PhysicalDescription.medium: pen and ink on paper
```

### 9. Institution/Repository (Required)

##### DEFINITION:

The name of the repository where the resource is currently located.

##### GUIDELINES for creating values for the INSTITUTION/REPOSITORY element

Prefer taking the name from a standard naming authority file, such as the Library of Congress Name Authority File (LCNAF). If a name does not appear in an authority file, establish it according to a content standard such as Anglo-American Cataloguing Rules (AACR2), Cataloging Cultural Objects (CCO), or Describing Archives: a Content Standard (DACS).

```
EXAMPLES
* Charles E. Young Research Library. Department of Special Collections
* Vorderasiatisches Museum (Berlin, Germany)
```

### 10. Rights (Required)

##### DEFINITION:

Information about the creation and/or publication of a resource that is related to the intellectual property rights associated with the object.

##### GUIDELINES for creating values for the RIGHTS element

_Always include qualifiers for this element._

**Required qualifiers:**

**copyrightStatus:** Use control values only.

* copyrighted – the material is under copyright
* public domain – material is in the public domain (more specific public domain values follow)
* public domain - US federal government
* public domain - dedicated (means the rights holder dedicated the item to the public domain)
* public domain - expired (for something that has expired from copyright)
* unknown – if the copyright status of an item is unknown

**publicationStatus:** Choose one of three values:

* published
* unpublished
* unknown

**servicesContact:** Contact information for any services offered related to this item. Could be contact information for rights requests and/or requests for master images. Providing data for this qualifier (especially at the collection level) is recommended to encourage and enable patrons to contact the correct unit for permission, licensing, and high-quality files.

```
EXAMPLES
* Rights.copyrightStatus: copyrighted
* Rights.publicationStatus: published
* Rights.servicesContact: Doe, John (jdoe@email.edu)
```

### 11. Description (Recommended)

##### DEFINITION:

An account of the content of the resource, and other descriptive information about the resource. Description may include information such as an abstract, table of contents, or a free-text account of the content.

##### GUIDELINES for creating values for the DESCRIPTION element

Use qualifiers to distinguish different types of Description (e.g. .abstract, .inscription, .note, etc.). Be judicious in using this element; important information about the resource should be captured in other elements if appropriate.

```
EXAMPLES
* Description.note: Date on back of poster, 1997, reflects when the vendor received the copy later acquired by the UCLA Library.
* Description.inscription: "Longhaired" Palisades High School students protest school's demand that they get hair cut. [from caption on resource.]
```

### 12. Subject (Recommended)

Any of the topics or themes of a work, stated explicitly in the resource or its title or implicitly in its content. Subjects can be persons or organizations, other resources, places, or topics.

##### A. Persons / organizations

##### DEFINITION:

Significant names (personal, corporate, family, meeting) that are the subject of, or that are represented in, on or by the resource.

##### GUIDELINES for creating values for the SUBJECT element

Prefer taking the name from a standard naming authority file, such as VIAF, or other sources such as the Library of Congress Name Authority File (LCNAF) or Union List of Artists’ Names (ULAN). If a name does not appear in an authority file, establish it according to a content standard such as Anglo-American Cataloguing Rules (AACR2), Cataloging Cultural Objects (CCO), or Describing Archives: a Content Standard (DACS).

```
EXAMPLES
* Antoniani, Pietro, d ca. 1740-1805
* Institute without Boundaries
```
##### B. Titles

##### DEFINITION:

Significant titles of other resources (e.g. works, expressions of those works, individual items, etc.) that are the subject of, or that are represented in, on or by the resource.

##### GUIDELINES for creating values for the SUBJECT element

The form of the title should be taken from a standard naming authority file, such as the Library of Congress Name Authority File, which contains uniform titles (LCNAF). If the title does not appear in an authority file, establish the title according to a content standard such as AACR2, CCO, or DACS.

```
EXAMPLES
* Bible. O.T. Psalms
* Maha bha rata
```
##### C. Place

##### DEFINITION:

Significant names of geographic locations that are the subject of, or that are represented in, on or by the resource.

##### GUIDELINES for creating values for the SUBJECT element
The form of the place name should be taken from a standard naming authority file. For IDEP we recommend Thesaurus of Geographic Names (TGN). If the name does not appear in an authority file, establish the name according to a content standard such as AACR2 or CCO.

IDEP uses a hierarchical form for place names, utilizing separate columns for:

* **Subject.country**
* **Subject.city**
* **Subject.place** (for specific locations within a city, region, or country)

```
EXAMPLES
* Subject.place: Acequia Madre de Santa Barbara
* Subject.country: Iran
* Subject.city: Yerevan
```

##### D. Topic

##### DEFINITION:

A description or interpretation of the topics, activities, events, ideas or objects that are the subject of, or that are represented in, on or by the resource. In the case of images, use the Subject element to capture both what the resource is about  (concept), and what it is of  (descriptive), as applicable.

##### GUIDELINES for creating values for the SUBJECT element

The form of the subject term should be taken from a standard subject thesaurus, such as LCSH, MeSH, AAT or TGM.

```
EXAMPLES
* Fruit crate labels
* Depression (Mental state)
* Regional planning
* antimacassars
```

### 13. Relation (Recommended)

##### DEFINITION:

A reference to a related resource. (Note: For objects that are part of digital collections, the Relation -- between the object and the collection that it is part of -- is created automatically.)

##### GUIDELINES for creating values for the RELATION element

_This element should always be qualified._

Recommended best practice is to reference the resource by means of a string or number conforming to a formal identification system when possible.

Relationships may be expressed reciprocally (if the resources on both ends of the relationship are being described) or in one direction only, even when there is a refinement available to allow reciprocity. If free text is used instead of a formal string or identifying numbers, the reference should be appropriately specific. For instance, a formal bibliographic citation might be used to point users to a particular resource.

```
EXAMPLES
* Relation.hasVersion: IFDC report (Spanish edition) [example of a version in another edition, language, etc.]
* Relation.hasFormat: CD-ROM version: Health literacy. Washington, D.C. : National Academies Press, c2004.
* Relation.derivedFrom: Michelangelo Buonarroti, 1475-1564. Creation of Adam. [example of a work inspired by this painting]
```

### 14. Source (Recommended)

##### DEFINITION:

A related resource from which the described resource is derived, in whole or in part. This element may also include information about the ownership or custodial history of the object.

##### GUIDELINES for creating values for the SOURCE element

Recommended best practice is to identify the related resource by means of a string conforming to a formal identification system, when possible. In general, include in this area information about a resource that is related intellectually to the described resource but does not fit easily into a Relation element.

Information about the location of discovery or excavation of the object should be entered in either the **Subject** or the **Coverage.Spatial** element of the record.

Source will not normally be used for born digital objects.

```
EXAMPLES
* BM XV cent., II, p. 346 (IB.5874)
* Smithsonian Archives Record Unit 54, Joseph Henry Collection, 1808, 1825-1878, Box 1, Folder 6, Item 3
```
