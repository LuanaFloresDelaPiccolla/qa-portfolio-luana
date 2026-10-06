# Conduit Buffalo — Manual Testing

Manual testing practice by Luana Da Silva Flores, completed on October 6, 2026.

## Objective
Run the application locally, investigate defects, and document findings with screenshots and terminal logs.

## Environment
- Windows with Ubuntu (WSL)
- Google Chrome
- Buffalo application running locally with `buffalo dev`
- PostgreSQL running in a Docker container
- Application URL: http://127.0.0.1:3000

## Testing performed
- Registered a user successfully.
- Checked navigation to account settings.
- Inspected page styling.
- Reviewed terminal logs and browser Network responses.

## Reported bugs
- CON-44: Settings reloads the home page instead of opening account settings.
- CON-45: Application pages appear unstyled because CSS files fail to load.

Both bugs were linked to Jira story CON-43.

## Files
- `bugs/`: bug reports with reproduction steps and results.
- `evidence/`: screenshots and supporting logs.

## Scope
This was a focused exploratory testing exercise, not a complete regression test of the application.
