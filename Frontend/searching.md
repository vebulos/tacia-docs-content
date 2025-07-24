---
title: Search Functionality in TaciaDocs
description: How to use and customize the search capabilities in TaciaDocs
tags: search, find, navigation, user-experience
---

# Search Functionality

TaciaDocs features a powerful, client-side search system that helps users find content quickly and efficiently.

## How Search Works

- **Instant Results**: Search updates as you type
- **Fuzzy Matching**: Finds relevant results even with typos
- **Tag Filtering**: Use `tag:name` to filter by tags
- **Section Filtering**: Limit search to specific sections

## Search Syntax

- **Basic Search**: `keyword`
- **Phrase Search**: `"exact phrase"`
- **Exclude Terms**: `-exclude`
- **Required Terms**: `+required`
- **Grouping**: `(term1 OR term2) AND term3`
- **Wildcards**: `doc*` matches "document", "documentation", etc.

## Advanced Features

- **Search Operators**: `AND`, `OR`, `NOT`
- **Proximity Search**: `"term1 term2"~5` (terms within 5 words)
- **Field Search**: `title:installation` or `content:configuration`
- **Regular Expressions**: `/[a-z]+/`

## Customizing Search

You can customize search behavior through:

1. **Configuration Files**: Modify search parameters
2. **Custom Filters**: Add custom search filters
3. **Search UI**: Customize the search interface
4. **Indexing**: Control what gets indexed
