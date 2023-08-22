# php-migration-tool

Utility script to help manage database migrations.

Usage:

```bash
Syntax: migrate.php [create|status|up|up-to|reset|down|down-to] [args]

options:
 status         Show the status of the migrations
 create         Create a migration with the provided name
                Ex: migrate.php create example
 up-one         Applies the next pending migration
 up             Applies all the pending migrations
 up-to          Applies all the pending migrations up to the migration with the provided ID
                Ex: migrate.php up-to 1692628446_example
 reset          Rolls back all the applied migrations
 down           Rolls back the last applied migration
 down-to        Rolls back all the applied migrations back to the migration with the provided ID
                Ex: migrate.php down-to 1692628446_example

OBS: You need to provide the database connection credentials:
 Ex: migrate.php up HOST=localhost USER=user PASSWORD=password DATABASE=db_name
```
