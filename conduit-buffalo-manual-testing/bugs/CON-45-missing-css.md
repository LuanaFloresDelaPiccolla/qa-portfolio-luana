# CON-45 — Application pages appear unstyled

## Environment
Windows with Ubuntu (WSL), Google Chrome.
Buffalo running locally; PostgreSQL running in Docker.
URL: http://127.0.0.1:3000

## Steps to reproduce
1. Open the application.
2. Observe the page layout.
3. Check the terminal logs and the browser Network tab.

## Actual result
The page displays plain HTML without the expected styling.
The local stylesheets buffalo.css and application.css return 404.
The external stylesheet https://demo.productionready.io/main.css also returns 404.

## Expected result
The stylesheets load successfully, and the page displays its intended layout and formatting.

## Terminal log excerpts
These excerpts were transcribed from the terminal screenshot:

could not find assets/buffalo.css status=404
could not find assets/application.css status=404

## Browser evidence
The Network tab shows a GET request to:
https://demo.productionready.io/main.css

Response: 404 Not Found.

## Evidence
- [Unstyled page](../evidence/settings-result.png)
- [Terminal errors](../evidence/terminal-log.png)
- [External stylesheet 404 response](../evidence/main-css-404.png)

## Jira
Bug: CON-45
Related story: CON-43
