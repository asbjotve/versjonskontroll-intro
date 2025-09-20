```mermaid
flowchart TD
    movie -->|has| movie_in_collection
    movie_in_collection -->|belongs to| physical_collection
    disc -->|in| disc_in
    disc_in -->|belongs to| physical_collection
    person -->|has| has_role
    has_role --> movie
```
