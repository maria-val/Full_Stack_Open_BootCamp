```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created, [{"message":"note created"}]
    deactivate server

    Note over browser: {content: "spa note", date: "2024-10-20T19:42:10.320Z"}
```

    