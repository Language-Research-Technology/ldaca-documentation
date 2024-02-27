---
title: "Search"
date: 2024-01-23T14:23:27+11:00
draft: false
description: "Further refine your queries with word, phrase and pattern searches."
---

<br>

Search allows you to further refine your queries throughout collections, objects and files, both through single or group word queries, as well as specific patterns through regular expressions. The Portal has both basic and advanced search capabilities.

<br>

### Basic Search

<br>

The Basic Search is accessed from the top left section of the Portal main page.

<br>

![Basic Search](/help_docs/basic-search.png "Basic Search")
 
<br>

Basic Search allows you to search for:
- single words
- multiple words where at least one of these occur (e.g. `northern territory` will return results where 'northern' and 'territory' occur in isolation, as well as any instances where 'northern' and 'territory' occur in the same object.)

Basic Search does not allow you to search for:
- exact phrases
- parts of words

<br>

Results are ordered by default according to relevance and in descending order. Each result will display a _Relevance Score_ based on the search query. If at least one of the query words occurs in the text field of an object, this will be highlighted in yellow, however highlighting will not occur for matches within other fields such as name and description.

Note that queries in Basic Search will be applied to all content in the collections (e.g. name, description, text). If you need to refine the search field, use Advanced Search.

<br>

### Advanced Search

<br>

The Advanced Search is accessed by selecting ___Advanced Search___ below the Basic Search bar.

<br>

![Advanced Search](/help_docs/advanced-search.png "Advanced Search")

<br>

##### Search Fields

By default, queries in Advanced Search are applied to all fields, however this can be refined in the top-left dropdown menu. The current fields of search available are _Name_, _Description_, _Language_ and _Text_. Multiple search fields can be added by selecting ___Add New Line___.

To reset your search, select ___Clear___.

The information entered in the Advanced Search box(es) is treated as part of a 'mini-language'.

- The query string is parsed into a series of terms and operators.
- In general, the search functions are not case-sensitive. Exceptions to this are Boolean operators (see below). 

<br>

##### Boolean Operators

The standard Boolean operators `AND`, `OR` and `NOT` are supported in advanced search. These can either be added in the dropdown menu when ___Add New Line___ is selected, or included within the search text field, but parentheses should be used whenever multiple operators occur together.

For instance, to search for items that contain both 'public' and 'house' or 'government' and 'house' but not 'cottage', the query should be:

`((public AND house) OR (government AND house)) NOT cottage`

To search for the literal words AND, OR and NOT, add a backward slash (\\) before that word to escape it, e.g. `\OR`. Note that this is a situation where the search is case-sensitive; 'and' does not need to be escaped, but 'AND' does. Escaping will not return case-sensitive matches; it will just prevent its use as a Boolean operator.

<br>

##### Query String Syntax

Symbol | Function
--- | ---
" " | Use double quotation marks before and after a phrase to search for that exact phrase, e.g. `"public house"`. Searching for space in a phrasal search will also return entries where a hyphen occurs instead.
^ | Boost operator that makes one term more relevant than another, e.g. `quick^2 fox`
~ | Creates a fuzzy query to return results similar to the search term by changing, removing, inserting or transposing one character. Can also be applied to phrase searches allowing the specified words to be further apart or in a different order. Add a number following this to increase the number of variations, e.g. `brwn~2` and `"house home"~3`
? | Wildcard to replace zero or one of the previous character. Wildcards cannot be included in a phrase search.
\* | Wildcard to replace zero or more of the previous character. Wildcards cannot be included in a phrase search.
\+ | Wildcard to replace one or more of the previous character. Wildcards cannot be included in a phrase search.
( ) | Defines a sub-expression.

<br>

##### Regular Expressions

Some regular expression patterns can be used within the query string by surrounding the pattern in forward slashes, e.g. `/gr[ae]y/` or `/honou*r/`. Currently, regular expressions can only be used for full-word searches and not phrases. This search engine does not support full Perl-compatible regex syntax, for more information see: [RegExp Syntax](https://www.elastic.co/guide/en/elasticsearch/reference/current/regexp-syntax.html).

<br>

##### Reserved Characters

`+ − = && ; || > < ! ( ) { } [ ] ^ " ~ * ? : \ /`

<br>

##### Show Query

If you need to check your search command against what it is actually sent to the search engine, select ___Show Query___.

For example, setting the search field to _Language_ and searching for `Danish` has the following query string:

`( language.name.@value: Danish )`

<br>