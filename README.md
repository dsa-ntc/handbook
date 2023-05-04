# NTC Handbook

This README should lay technical tasks like how to build the handbook frontend locally. This README is not part of the handbook, it's part of the frontend build process.

## Running mkdocs locally

To develop against our public-facing handbook (everything in [/docs](./docs)), you will need docker and vscode installed, along with the dev containers extension for vscode. With docker running, run the dev containers 'rebuild and launch' command from VSCode to load the application in a containerized environment. From there you can start the application from the vscode shell with `mkdocs serve`.