erDiagram
    MOVIE {
        int movie_id PK
        string title
        string original_title
    }
    DISC {
        int disc_id PK
        string type_disc
        string format
    }
    PHYSICAL_COLLECTION {
        int collection_id PK
        string barcode
        string format
        string box_set_ean
    }
    PERSON {
        int person_id PK
        string name
        string id_tmdb
        string id_tvdb
        string artwork
    }
    HAS_ROLE {
        int person_id FK
        int movie_id FK
        string role
    }
    MOVIE_IN_COLLECTION {
        int movie_id FK
        int collection_id FK
    }
    DISC_IN {
        int disc_id FK
        int collection_id FK
    }
