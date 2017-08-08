## 0.5.2 to 0.5.3 (unreleased)

 * Events: Subqueries can be extended by the configuration, see the example configuration.
 * Events: Subqueries can need the parameter '%s' more or less than one time in the SQL query, for example:
   ```
   ("source.ip" = '%s' OR "destination.ip" = '%s')
   ```

## 0.5.1 to 0.5.2

 * Contactdb: Fixes annotation/search for organisation\_annotations.


## 0.5.0 to 0.5.1

 * Contactdb: Adds search for annotations by tag-name.
 * Contactdb: Allows to configure the list of common "tags".
 * Contactdb: Changes email search to be case-insensitive.

### Upgrade
 * Configuration: (optional) Add "common\_tags" to the contactdb config file,
     otherwise the default ones may be exposed to users by the frontend.


## 0.4.3.dev0 to 0.5.0
 * Contactdb: Allows tracking of db changes by user.
 * Contactdb: Adds example script for importing a manual whitelist.
 * Technical: Module called "intelmq-fody-backend" now
 * Technical: Compatible with psycopg2 coming with Ubuntu 16.04LTS now.

### Upgrade
 * To enable tracking of db changes by user follow instructions in README.md.
 * Technical: Must make sure that calling code uses the new module name.
