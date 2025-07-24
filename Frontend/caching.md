---
title: Caching in TaciaDocs
description: How TaciaDocs implements client-side and server-side caching
tags: frontend, performance, caching, optimization
---

# Caching Strategy

TaciaDocs employs a comprehensive caching strategy to ensure fast and responsive performance, even with large documentation sets.

## Client-Side Caching

- **Document Structure**: The complete documentation structure is fetched once and cached in the browser's memory
- **Content Caching**: Individual documentation pages are cached as they are viewed
- **Search Index**: The search index is cached to enable instant searches

## Server-Side Caching (Backend-Dependent)

- **File System Caching**: Backends may implement their own caching mechanisms
- **Response Caching**: API responses can be cached to reduce server load

## Cache Invalidation

- Automatic invalidation when content changes
- Manual cache clearing via developer tools
- Version-based cache busting for static assets
