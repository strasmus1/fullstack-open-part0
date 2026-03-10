```mermaid
  sequenceDiagram
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->>-browser: HTML document
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>-browser: the css file
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    activate server
    server-->>-browser: the JavaScript file
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>-browser: [{ "content": "hi", "date": "2023-01-23T21:40:14.033Z" }, ... ]
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/favicon.ico
    activate server
    server-->>-browser: HTML document
    deactivate server
 ```
