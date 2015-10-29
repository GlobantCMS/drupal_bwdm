# Drupal - Build with Drush make
This project contains all the files needed to build a Drupal installation using `ant`. The profile has some example downloads and dependecies, like `views` and `beans`.

## Dependencies
* Apache Ant
* Drush

*NOTE:* This project works properly in MacOS, Linux or other SO with a *nix kernel. For usage on Windows, please install a Virtual Machine.

## How to Use it
1. Create a copy of the file `build.properties.dist` called `build.properties` and change the properties of installation.
2. Create a copy of the file `example.local.settings.php` in `sites/default` called `local.settings.php` and update database connection info. *NOTE:* The `settings.php` file is not ignored by git, so all changes will be part of the repository.
3. Create a directory called `files` in `sites/default`.
4. Run the command `ant develop-install` for initial installation or `ant develop-update` for code update.
