```mermaid



sequenceDiagram



\&#x20;   participant browser



\&#x20;   participant server







\&#x20;   browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new\_note\_spa



\&#x20;   activate server



\&#x20;   server-->>browser: 201 Created Response



\&#x20;   deactivate server









\&#x20;   Note right of browser: The browser executes the Javascript code adding and rendering the new note without re-requesting the html page

```



