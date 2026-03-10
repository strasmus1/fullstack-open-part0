```mermaid
sequenceDiagram
  
    browser->>+server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>-browser: HTML document
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    server-->>-browser: HTML document
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>-browser: the css file
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>-browser: the JavaScript file
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>-browser: [{ "content": "h", "date": "2023-01-23T21:29:40.911Z" }, ... ]
    deactivate server
    
    browser->>+server: GET https://studies.cs.helsinki.fi/favicon.ico
    activate server
    server-->>-browser: HTML document
    deactivate server
 ```
