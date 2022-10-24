# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

The following setup steps have been tested and should allow the solution to run on your local environment.

  1. From the repository root, run `docker-compose up`

     *Note: if you have not already pulled the required Docker images locally,
     this step may take some time for the images to download.*

     This will create a complete environment with front end, back end, and database services.

  2. Test the back end by loading the following URL in a browser `http://localhost:3000/api/ping`

  3. **If you see a `PendingMigrationError`**, run the migration to ensure that the database schema is up to date.

  4. The site should now be fully working, you can register a new user from the front end at `http://localhost:3001/register`

  5. To stop services, use Ctrl-C to exit out of the Docker compose session.