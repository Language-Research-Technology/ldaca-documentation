---
title: "Basic Portal Navigation"
date: 2024-01-29T11:45:30+11:00
draft: false
description: "TODO"
---

<br>

### Data and Page Structure

Both the data and the webpages in the portals are structured in a heirarchy: Collections contain Objects and Objects contain Files. TODO how do notebooks fit in to this?

Level | Description
--- | ---
Collection | A group of related Objects. Examples of collections include corpora, and sub-corpora, as well as aggregations of cultural objects such as PARADISEC collections, which bring together items collected in a region or a session with consultants.
↓ | 
Object | A single resource or a group of tightly related resources that record a communicative event; for example, a dialogue or session in a speech study, a work (document) in a written corpus.
↓ |
File | The various formats associated with an Object. For example, a single Object could have an audio file as well as a text file transcribing the audio.

<br>

##### Jump to:
##### [Home Page](#home-page) ([Top Menu](#top-menu), [Left Panel](#left-panel), [Main Panel](#main-panel))
##### [Collection Page](#collection-page)
##### [Object Page](#object-page)
##### [File Page](#file-page)

<br>

### Home Page

There are three main sections of the Home Page in the portal: the top menu bar, the left panel and the main panel.

<br>

##### Top Menu

<br>

![Home Page: Top Menu](/help_docs/top-menu.png)

<br>

The top menu of the home page contains some of the main features of the portal:
- ___LDaCA logo___: Returns you to the home page from anywhere in the portal. TODO is the word home next to it redundant?
- ___Collections___: Filters the results section of the main panel so that only collections are shown (excluding objects, files and notebooks).
- ___Browse___: Resets your results to the default settings. (TODO check - this seems to work exactly the same as the LDaCA logo unless I'm missing something, is it redundant?)
- ___Login___: Takes you to the CILogon page where you can login to apply for access to collections or view your current access. See [Login](/accessing-data/login/) for more details.
- ___Help___: Provides more general information about the infrastructure the Portal was built with, as well as the Oni API functionalities. It also links back to this user guide for easy reference.

<br>

##### Left Panel

<br>

![Home Page: Left Panel](/help_docs/left-panel.png)

<br>

The left panel of the Portal home page allows you to refine your data query through the use of a search field and filters. Hovering over the information icon ![Information Icon](/help_docs/information.png) next to each filter will display tooltips related to that filter. See [Search](/browsing-searching/search/) and [Filters](/browsing-searching/filters/) for more details on how to use the search and filter functions.

<br>

##### Main Panel

<br>

![Home Page: Main Panel](/help_docs/main-panel.png)

<br>

The main panel on the right of the home page allows you to view the top-level descriptions of collections, objects, files and notebooks in the Portal. The top row shows the total number of Index entries or items; this total will reduce as you apply filters and search queries. Below this is the option to ___Reset Search___, clearing the query of all filters and searches. The ___Sort by___ and ___Order by___ dropdown boxes can also be configured; see [Sort and Order](/browsing-searching/sort-and-order/) to learn more about their usage. Pagination options appear below this and are also accessible from the end of the page, with 10 results appearing on each page.

<br>

The results in the main panel contain a set of top-level descriptions:
- __Name__: The name of the collection, object, file or notebook.
- __Type__: TODO should this be updated to record type so it's in line with the filter name?
- __Language__: The language(s) of the materials (including PrimaryMaterials, DerivedMaterials and Annotations) in this item.
- __Description__: An abstract of the collection, object, file or notebook.
- __Members__: The number of items within the given collection. TODO is there another name for this section?
- __Member of__: The collection that an object, file or notebook is a part of.

<br>

Hovering over the icons next to each item reveals three further levels of detail (Access, Modality and File Format):

Icon | Category | Icon Tooltip
--- | --- | ---
![Public Icon](/help_docs/public.svg) | Access | You can access this data immediately and by doing so you accept the licence terms specified on the record.
![Login Icon](/help_docs/login.svg) | Access | You can access this data after logging in. You may also have to agree to licence terms in an automatic process.
![Login Plus Icon](/help_docs/loginplus.svg) | Access | There are restrictions on access to this data. Log in to get further information.
![SpokenLanguage Icon](/help_docs/spokenlanguage.svg) | Modality | SpokenLanguage
![WrittenLanguage Icon](/help_docs/writtenlanguage.svg) | Modality | WrittenLanguage
![TXT Icon](/help_docs/file-lines-solid.svg) | File Format | text/plain
![Code Icon](/help_docs/file-code-solid.svg) | File Format | application/tei+xml<br>application/vnd.openxmlformats-officedocument.wordprocessingml.document
![Audio Icon](/help_docs/file-audio-solid.svg) | File Format | audio/mpeg<br>audio/x-wav
![Video Icon](/help_docs/file-video-solid.svg) | File Format | application/mp4
![CSV Icon](/help_docs/file-csv-solid.svg) | File Format | text/csv
![PDF Icon](/help_docs/file-pdf-solid.svg) | File Format | application/pdf

<br>

### Collection Page

<br>

Clicking on one of the collections from the main page results will take you to the Collection page for that item.

<br>

![Collection Page: Braided Channels Example](/help_docs/collection-page.png)

<br>

The main panel of the Collection page lists the main details and metadata associated with the collection. Clicking on the question mark icon ![Question Mark Icon](/help_docs/question.png) or information icon ![Information Icon](/help_docs/information.png) next to each heading will display tooltips related to that item.

Below the main description and metadata is the number of objects present in the collection. The objects are then listed underneath, with pagination options if there are more than 10 objects in the collection. TODO how are these ordered?

The right panel has the following sections:
- __Access__: Defines the license and access conditions for the current collection. TODO (together with a click-through link to the full license - this isn't the case currently).
- __Content__: Lists some of the main features of the current collection including _Language_, _Linguistic Genre_, _Modality_, _File Formats_ and _Data licenses for access_.
- __Retrieve Metadata__: View or download the metadata associated with the current collection, as well as the license and access conditions for this metadata.
- __Notebooks__: Lists any notebooks associated with the current collection.

<br>

### Object Page

<br>

Clicking on one of the objects or files from either the main page results or from a Collection page will take you to the Object page for that item.

<br>

![Object Page: A Corpus of Oz Early English Example](/help_docs/object-page.png)

The left panel of the Object page lists the main details and metadata associated with the object. Clicking on the question mark icon ![Question Mark Icon](/help_docs/question.png) or information icon ![Information Icon](/help_docs/information.png) next to each heading will display tooltips related to that item.

The right panel has the following sections:
- __Access__: Defines the license and access conditions for the current object, together with a click-through link to the full license.
- __Member Of__: Lists the collection that the current object is a part of.
- __Other Objects in this Collection__: Lists the other objects that are in the same collection as the current object.

The end of the Object page provides details about the files that form part of the current object. In the example above, the object _Text 1-028 1791 Convict_ has two associated files: a plain text version and a text version including metadata codes, the contents of which can be viewed using the dropdown arrow to the right of the file name. A preview of the file is available (provided that the access conditions permit this), and there are two options: ___View File___ to display the full file in the web browser, and ___Download File___ to save a copy of the file to your local system.

<br>

### File Page

<br>

Clicking ___View File___ on one of the files in an Object page will take you the File page for that item.

<br>

![File Page: Braided Channels Example](/help_docs/file-page.png)

From this page, you can view the whole file or download it with the option at the end of the page.

<br>