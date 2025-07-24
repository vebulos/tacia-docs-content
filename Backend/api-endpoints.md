# API Endpoints

This section documents the RESTful API endpoints provided by the TaciaDocs backend. Both the Java and JavaScript implementations expose the same API contract to ensure compatibility with the frontend.

## Content Management

- `GET /api/content`
  - **Description**: Lists the content (files and directories) at a specified path.
  - **Query Params**: `path={directory_path}`

- `GET /api/content/item`
  - **Description**: Gets the details of a specific content item (Markdown file).
  - **Query Params**: `path={file_path}`

- `GET /api/content/raw`
  - **Description**: Gets the raw Markdown content of a file.
  - **Query Params**: `path={file_path}`

## Document Structure

- `GET /api/structure`
  - **Description**: Retrieves the entire hierarchical documentation structure.

- `GET /api/first-document`
  - **Description**: Finds the first available document in a given directory, which is useful for landing pages.
  - **Query Params**: `path={directory_path}`

## Search

- `GET /api/search`
  - **Description**: Performs a full-text search across all documentation files.
  - **Query Params**: `query={search_term}`

## Health Check

- `GET /actuator/health` (Java) or `/health` (JS)
  - **Description**: Checks the health status of the API server. Returns a `200 OK` if the service is running.
