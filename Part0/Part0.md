# Exerise
## Exercise 0.1

## Exercise 0.4 Mermaid
```mermaid
sequenceDiagram
    participant browser
    participant client

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    Note right of browser: Payload Form Data: note=hhhhhh
    server->>browser: 302 Found
    deactivate server
    Note right of browser: Update the html page
```

## Exercise 0.5 Single page app diagram
```mermaid
sequenceDiagram
	participant browser
	participant server
	browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
	activate server
	server->>browser: HTTP 200 OK
	server->>browser: "message: note created"
	deactivate server
```

## Exercise 0.6 New note in Single page app diagram
```mermaid
sequenceDiagram
	participant browser
	participant server
	browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
	activate server
	server->>browser: HTTP 201 Created
	server->>browser: "message: note created"
	deactivate server
```
