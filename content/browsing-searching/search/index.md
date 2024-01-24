---
title: "Search"
date: 2024-01-23T14:23:27+11:00
draft: false
description: "TODO"
---

<br>

TODO: Add general description of search.

<br>

### Basic Search

The Basic Search is accessed from the top left section of the Portal main page.

Basic Search allows you to search for:
- single words
- multiple words where at least one of these occurs (e.g. `northern territory` will return results where 'northern' and 'territory' occur in isolation, as well as any instances where 'northern' and 'territory' occur in the same object.)

Basic Search does not allow you to search for:
- exact phrases

<br>

Results are ordered by default according to relevance and in descending order. Each result will display a _Relevance Score_ based on the search query. If at least one of the query words occurs in the text field of an object, this will be highlighted in yellow, however highlighting will not occur for matches within other fields such as name and description.

Note that queries in Basic Search will be applied to all content in the collections (e.g. name, description, text). If you need to refine the search field, use Advanced Search.

<br>

### Advanced Search

TODO: add guide for accessing advanced search

 The information entered in the Advanced Search box(es) is treated as part of a 'mini-language'.

- The query string is parsed into a series of terms and operators.
- In general, the search functions are not case-sensitive. Exceptions to this are Boolean operators (see below). 

<br>

__Boolean Operators__

The standard Boolean operators `AND`, `OR` and `NOT` are supported in advanced search. These can either be added in the dropdown menu when _Add New Line_ is selected, or included within the search text field, but parentheses should be used whenever multiple operators occur together.

For instance, to search for items that contain both 'public' and 'house' or 'government' and 'house' but not 'cottage', the query should be:

`((public AND house) OR (government AND house)) NOT cottage`

To search for the literal words AND, OR and NOT, add a backward slash (\\) before that word to escape it, e.g. `\OR`. Note that this is a situation where the search is case-sensitive; 'and' does not need to be escaped, but 'AND' does. Escaping will not return case-sensitive matches; it will just prevent its use as a Boolean operator.

<br>

__Query String Syntax__

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

__Regular Expressions__

Some regular expression patterns can be used within the query string by surrounding the pattern in forward slashes, e.g. `/gr[ae]y/` or `/honou*r/`. Currently, regular expressions can only be used for full-word searches and not phrases. This search engine does not support full Perl-compatible regex syntax, for more information see: [RegExp Syntax](https://www.elastic.co/guide/en/elasticsearch/reference/current/regexp-syntax.html).

<br>

__Reserved Characters__

`+ − = && ; || > < ! ( ) { } [ ] ^ " ~ * ? : \ /`

<br>