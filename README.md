# DevTools Module

The DevTools module adds command and query inspection handlers to the Flexi CLI. It registers the `command:list` and `query:list` aliases and returns each bus's configured handler definitions as formatted JSON.

The registrations are in `Config/commands.json` and `Config/queries.json`. Install `flexi/flexi-module-devtools`, activate `DevTools`, then use the aliases through the core CLI.

This module exposes framework structure and is intended for development environments. Do not activate it in production unless the CLI access policy is restricted. It supports PHP 7.4+, Flexi Core `^3.2`, and `flexi/contracts` `^5.2.1`.

## Tests

Install the development dependencies with `composer install`, then run `vendor/bin/phpunit tests` from the module root.
