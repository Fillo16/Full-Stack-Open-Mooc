```mermaid



sequenceDiagram



    participant browser
    participant server


    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new\_note\_spa
    activate server
    server-->>browser: 201 Created Response
    deactivate server

    Note right of browser: The browser executes the Javascript code adding and rendering the new note without re-requesting the html page

```



