## Specific Episode Query

**Endpoint:**
[Rick and Morty Endpoint](https://rickandmortyapi.com/graphql)

**Description:**
This query retrieves details of a specific episode from the Rick and Morty API using the `episode(id: ID!)` field.

**Fields Returned:**
- `id` — The unique identifier of the episode
- `name` — The title of the episode
- `air_date` — The date the episode aired
- `episode` — The code of the episode (e.g., S01E01)

**Files:**
- `episode-id-1.graphql` — GraphQL query for episode with ID 1
- `episode-id-1-output.json` — JSON output for episode with ID 1
- `episode-id-2.graphql` — GraphQL query for episode with ID 2
- `episode-id-2-output.json` — JSON output for episode with ID 2
- *(Continue similarly for other IDs if required)*

**Example Query (Episode ID: 1):**
```graphql
query {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}

}


