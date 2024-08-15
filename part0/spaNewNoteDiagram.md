```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: User clicks 'Save' on the browser
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created
    deactivate server
    Note left of server: {"message":"note created"} 

```