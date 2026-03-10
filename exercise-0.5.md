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
    server-->>-browser: [{ content: "yolo!", date: "2026-03-10T13:34:27.029Z" }, ... ]
    deactivate server
 ```
