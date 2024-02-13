---
title: "Basic Navigation"
date: 2024-01-29T11:45:30+11:00
draft: false
---

<br>

### Home Page

There are three main sections of the Home Page; the top menu bar, the left panel and the main panel. TODO right panel? main panel?

<br>

##### Top Menu

<br>

![Home Page: Top Menu](/help_docs/portal01-topMenu.png)

<br>

The top menu of the home page contains some of the main features of the Portal:
- __LDaCA logo:__ Returns you to the home page from anywhere in the Portal. TODO is the word home next to it redundant?
- __Collections:__ Filters the main results section so that only collections are shown (rather than objects, files and notebooks as well).
- __Browse:__ Resets your results to the default settings (TODO check - this seems to work exactly the same as the LDaCA logo unless I'm missing something, is it redundant?)
- __Login:__ Takes you to the CILogon page where you can login in order to apply for access to collections or view your current access. For more details on this, see [Login](/accessing-data/login/).
- __Help:__ Provides more general information about the infrastructure the Portal was built with, as well as the Oni API functionalities. It also links back to this user guide for easy reference.

<br>

##### Left Panel

<br>

![Home Page: Left Panel](/help_docs/portal01-leftPanel.png)

<br>

The left panel of the Portal home page allows you to refine your data query through the use of a search field and filtering. Hovering over the information icon ![Information Icon](/help_docs/information.png) next to each filter will display tooltips related to that item. For more details on how to use the search and filter functions, see the pages [Search](/browsing-searching/search/) and [Filters](/browsing-searching/filters/).

<br>

##### Main Panel

<br>

![Home Page: Main Panel](/help_docs/portal01-mainFrame.png)

<br>

The main panel on the right of the home page allows you to view the top-level descriptions of collections, objects, files and notebooks in the Portal. The top row shows the total number of index entries or items; this total will reduce as you apply filters and search queries to your requests. Below this, there are options to ___Reset Search___, clearing the request of all filters and searches. The ___Sort By___ and ___Order By___ dropdowns can also be configured; to learn more about their usage, see [Sort and Order](/browsing-searching/sort-and-order/). Pagination options appear below this and are also accessible from the end of the page, with every page having a total of 10 results.

<br>

The results in the main panel contain a set of top-level descriptions:
- __Name:__ The name of the collection, object, file or notebook.
- __Type:__ TODO should this be updated to record type so it's in line with the filter name?
- __Language:__ The language(s) of the materials (including PrimaryMaterials, DerivedMaterials and Annotations) in this item.
- __Description:__ An abstract of the collection, object, file or notebook.
- __Members:__ The number of items within the given collection. TODO is there another name for this section?
- __Member of:__ The collection that an object, file or notebook is a part of.

<br>

Hovering over the icons next to each item shows three further levels of detail about that item:

Icon | Category | Description
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

![Collection Page: Braided Channels Example](/help_docs/collectionPage_BraidedChannels.png)

<br>

The main panel of the Collection page lists the main details and metadata associated with the collection. Clicking on the question mark icon ![Question Mark Icon](/help_docs/question.png) and information icon ![Information Icon](/help_docs/information.png) next to each term will display tooltips related to that item.

Following the main description and metadata is a count of the number of objects present in the collection, with each of these objects listed below. Pagination options are also available for collections with more than 10 objects. TODO how are these ordered?

The right panel has the following sections:
- __Access:__ Defines the license and access conditions for the current collection. TODO together with a click-through link to the full license.
- __Content:__ Lists some of the main features of the current collection including _Language_, _Linguistic Genre_, _Modality_, _File Formats_ and _Data licenses for access_.
- __Retrieve Metadata:__ View or download the metadata associated with the current collection. The license and access conditions for this metadata is also listed.
- __Notebooks:__ Lists any notebooks associated with the current collection.

<br>

### Object Page

<br>

Clicking on one of the objects or files from either the main page results or from a collection page will take you to the Object page for that item.

<br>

![Object Page: A Corpus of Oz Early English Example](/help_docs/objectPage_COOEE.png)

The left panel of the Object page lists the main details and metadata associated with the object. Clicking on the question mark icon ![Question Mark Icon](/help_docs/question.png) and information icon ![Information Icon](/help_docs/information.png) next to each term will display tooltips related to that item.

The right panel has the following sections:
- __Access:__ Defines the license and access conditions for the current object, together with a click-through link to the full license.
- __Member Of:__ Lists the collection that the current object is a part of.
- __Other Objects in this Collection:__ Lists the other objects that are in the same collection as the current object.

The end of the Object page provides details about the files that form part of the current object. In the example above, the object _Text 1-028 1791 Convict_ has two associated files; the plain text version and a text version including metadata codes, both of which can be viewed with the dropdown option on the right. A preview of the file is available (provided that the access conditions permit this), and there are options ___View File___ to display the full file in the web browser, or ___Download File___ to save a copy of the file to your local system.

<br>