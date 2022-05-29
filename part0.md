0.4 New note

title 0.4

note over browser:
user submits new comment 
end note
browser->server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note
server-->browser: HTTP status code 302 (redirect to /exampleapp/notes)
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
server-->browser: HTML
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
server-->browser: main.js
browser->server: HTTP GET ttps://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{ content: "Note", date: "2022-05-29" }, ...]