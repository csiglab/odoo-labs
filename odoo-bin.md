# Odoo CLI (odoo-bin)

> The `odoo-bin` CLI (Command Line Interface) command is used to control various aspects of the Odoo ERP system, such as starting the server, updating the database, or running tests. This command is central to managing Odoo installations, especially in a development or deployment context.
> 

> Here’s a table outlining some of the most commonly used `odoo-bin` CLI commands and their purposes:
> 

| Command | Description |
| --- | --- |
| odoo-bin | Starts the Odoo server with the default configuration. |
| odoo-bin -c configfile | Starts Odoo using the specified configuration file. |
| odoo-bin -d dbname | Specifies the database name to connect to or manage. |
| odoo-bin -u module_name | Updates the specified module. Multiple modules can be specified, separated by commas. |
| odoo-bin -i module_name | Installs the specified module. Multiple modules can be specified, separated by commas. |
| odoo-bin --test-enable | Enables unit tests; usually run along with -i or -u to test installing or updating. |
| odoo-bin --stop-after-init | Stops the server after performing the initialization specified (like installation or update). |
| odoo-bin --log-level=level | Sets the logging level (e.g., info, warn, error, debug). |
| odoo-bin --without-demo=all | Disables loading demo data for all modules during installation. |
| odoo-bin --addons-path=path | Specifies the addons directory path. Multiple paths can be included, separated by commas. |
| odoo-bin --db-filter=regex | Filters the list of databases shown in the database selector based on the provided regex. |