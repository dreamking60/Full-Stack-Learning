# Exerise
## Exercise 0.4 Mermaid
```mermaid
sequenceDiagram
    participant browser
    participant client

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    Note right of browser: Payload Form Data: note=hhhhhh
    activate server
    server->>browser: 302 Found
    deactivate server
    Note right of browser: Update the html page
```