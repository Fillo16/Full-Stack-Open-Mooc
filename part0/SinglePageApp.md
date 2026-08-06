```mermaid

sequenceDiagram

&#x20;   participant browser

&#x20;   participant server



&#x20;   browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa

&#x20;   activate server

&#x20;   server-->>browser: HTML document

&#x20;   deactivate server



&#x20;   browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css

&#x20;   activate server

&#x20;   server-->>browser: CSS file

&#x20;   deactivate server



&#x20;   browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js

&#x20;   activate server

&#x20;   server-->>browser: JavaScript file

&#x20;   deactivate server

&#x20;   Note right of browser: The browser starts executing the JavaScript code, that not only fetches the JSON form the server but also manages all the functionality of the page, namely the new note functionality



&#x20;   browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json

&#x20;   activate server

&#x20;   server-->>browser: JSON file: \[{ "content": "HTML is easy", "date": "2023-1-1" }, ... ]

&#x20;   deactivate server



&#x20;   Note right of browser: The browser executes the callback function that renders the notes

```

