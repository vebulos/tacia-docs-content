---
title: Tagging System in TaciaDocs
description: How to use tags for organizing and discovering content
tags: tags, organization, metadata, content-management
---

# Tags in TaciaDocs

Tags provide a flexible way to categorize and organize your documentation, making it easier for users to find related content.

## How to Use Tags

### Adding Tags to Content

Add tags to your Markdown files using front matter:

```yaml
---
title: My Document
description: A sample document
tags: getting-started, tutorial, example
---
```

### Tag Syntax

- **Single Word**: `tag:getting-started`
- **Multiple Tags**: Separate with commas: `tags: angular, components, tutorial`
- **Tag with Spaces**: Use quotes: `tags: "getting started", tutorial`

## Tag Features

- **Tag Cloud**: Visual representation of all tags
- **Tag Pages**: View all content with a specific tag
- **Filtering**: Filter search results by tags
- **Related Content**: Automatically suggest related content based on tags

## Best Practices

1. **Be Consistent**: Use consistent naming for similar tags
2. **Use Plural**: Prefer `guides` over `guide`
3. **Be Specific**: Use specific tags like `angular-routing` instead of just `angular`
4. **Limit Number**: 3-5 tags per document is usually sufficient
5. **Hierarchical Tags**: Use slashes for hierarchy: `api/rest`, `api/graphql`

## Advanced Usage

### Tag Aliases

Create aliases for tags that might have multiple names:

```yaml
tags: ["javascript", "js"]
```

### Tag Metadata

Add descriptions or other metadata to tags in your configuration:

```yaml
tags:
  - name: getting-started
    description: "Guides for new users"
  - name: api
    description: "API reference documentation"
```
