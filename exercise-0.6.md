```mermaid
  sequenceDiagram
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->>-browser: HTML document
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>-browser: CSS file
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    activate server
    server-->>-browser: JS file
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>-browser: [	{ content: "yolo!", date: "2026-03-10T13:34:27.117Z" }, ... ]
    deactivate server

    browser->>+server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>-browser: [{ "message": "note created" }]
    deactivate server
 ```
