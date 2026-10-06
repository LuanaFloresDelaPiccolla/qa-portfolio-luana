# CON-44 — Settings reloads the home page

## Environment
Windows with Ubuntu (WSL), Google Chrome.
Buffalo running locally; PostgreSQL running in Docker.
URL: http://127.0.0.1:3000

## Precondition
The user is logged in.

## Steps to reproduce
1. Open the home page.
2. Click Settings in the navigation menu.

## Actual result
The home page reloads instead of opening account settings.
The user cannot access profile editing through Settings.

## Expected result
The account settings page opens and allows the user to edit their profile.

## Supporting terminal log
After clicking Settings, the terminal records:
GET / — status 200

This request is for the home page, rather than an account settings page.

## Evidence
- [Page after clicking Settings](../evidence/settings-result.png)
- [Terminal log](../evidence/terminal-log.png)

## Jira
Bug: CON-44
Related story: CON-43
