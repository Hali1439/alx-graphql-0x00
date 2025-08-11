# Character Queries

This project contains GraphQL queries to fetch specific character information from the Rick and Morty API using their `id`.

## API Endpoint
- [rick and morty API](https://rickandmortyapi.com/graphql)
## Query Fields
Each query retrieves:
- `id`
- `name`
- `status`
- `species`
- `type`
- `gender`

## Characters Queried
- ID 1
- ID 2
- ID 3
- ID 4

  ## Paginated Characters Queries

This section contains GraphQL queries and their outputs for retrieving a paginated list of characters from the Rick and Morty API.

**Endpoint:**

**Description:**
- We use the `characters(page: Int)` field to fetch characters for specific pages.
- For each page (1–4), the query retrieves the following fields:
  - `id`
  - `name`
  - `status`
  - `image`
- The results are saved as `.json` files for reference.

**Files:**
- `characters-page-1.graphql` — GraphQL query for characters on page 1
- `characters-page-1-output.json` — JSON output for page 1
- `characters-page-2.graphql` — GraphQL query for characters on page 2
- `characters-page-2-output.json` — JSON output for page 2
- `characters-page-3.graphql` — GraphQL query for characters on page 3
- `characters-page-3-output.json` — JSON output for page 3
- `characters-page-4.graphql` — GraphQL query for characters on page 4
- `characters-page-4-output.json` — JSON output for page 4

**Example Query (Page 1):**
```graphql
query {
  characters(page: 1) {
    results {
      id
      name
      status
      image
    }
  }
}

