# Learn-CI/CD (Notely)

This repo contains the starter code for the "Notely" application for the "Learn
CICD" course on [Boot.dev](https://boot.dev).

- Simple CRUD app, but robust CI/CD

## Accomplishments

### CI

Set up a `CI(Continuous Integration)` pipeline with `Github Actions` that
ensures new PRs pass certain checks before they are merged to `main`:

- Unit tests pass
- Formatting checks pass
- Linting checks pass
- Security checks pass

### CD

Configured a `cloud-based SQLite` database hosted on `Turso` You set up a
`CD(Continuous Deployment` pipeline with `GitHub Actions` that does the
following whenever changes are merged into `main`:

- Builds a new server binary
- Builds a new `Docker image` for the server
- Pushes the Docker image to the `Google Artifact Registry`
- Deploys a new `Cloud Run` revision with the new image and serves the app to
  the public internet
