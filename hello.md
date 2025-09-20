```mermaid
flowchart TD
    movie["movie"] -->|has| movie_in_collection["movie_in_collection"]
    movie_in_collection -->|belongs to| physical_collection["physical_collection"]
    disc["disc"] -->|in| disc_in["disc_in"]
    disc_in -->|belongs to| physical_collection
    person["person"] -->|has| has_role["has_role"]
    has_role --> movie
```
