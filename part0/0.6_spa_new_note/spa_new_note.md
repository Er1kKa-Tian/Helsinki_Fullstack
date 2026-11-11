# Sequence Diagram for Single Page App

```mermaid
sequenceDiagram
    participant user
    participant browser
    participant server

    user->>browser: Write contents

    user->>browser: Click save button

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa a JSON object
    
    Note right of browser: browser JSON code modifies DOM API to add new note

    Note right of server: server adds new note
```