# PostgreSQL Java examples

The sample connects to the local `Exercises` database as the `postgres` user. Both Java entry points read the password from the `DB_PASSWORD` environment variable and fail before connecting when it is missing.

Set `DB_PASSWORD` in your local run configuration. In Eclipse, open **Run Configurations → Environment** and add it there; keep the value out of source files and shared launch configurations. A `.env` file is ignored by Git but Java does not load it automatically.

Compile the source files under `src/net/codejava/net/`. The extensionless files under `bin/` are existing source copies and use the same environment configuration.

The PostgreSQL JDBC driver must be on the runtime classpath. The existing Eclipse `.classpath` entry points to a machine-specific JAR location; select your local driver installation before running.
