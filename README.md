# Drupal json schemas
This schemas can be used to validate Drupal 8+ yaml files.

## Supported yamls:
### Core
|File                   |Status|
|-----------------------|------|
|*.info.yml             |yes   |
|*.layouts.yml          |yes   |
|*.libraries.yml        |yes   | 
|*.breakpoints.yml      |To-do |
|*.schema.yml           |To-do |
|*.routing.yml          |To-do |
|*.services.yml         |To-do |
|*.links.action.yml     |To-do |
|*.links.contextual.yml |To-do |
|*.links.menu.yml       |To-do |
|*.links.task.yml       |yes   |
|*.permissions.yml      |yes   |
|\*/migrations/\*.yml   |To-do |

### Contrib
|Project/File           |Status|
|-----------------------|------|
|Drush (9.x+) yml files |To-do |
|migrate_plus           |To-do |

## TODO:
1. Add this schemas to schemastore.org [issue](https://github.com/SchemaStore/schemastore/issues/710)
1. Add schemas to Drupal core [issue](https://www.drupal.org/project/drupal/issues/3061454)
1. Add schema mappings to PhpStorm via bundled Drupal support or other custom plugin.  

## Usage
### PhpStorm (config file)
*Note:* this may override your existing JSON Schema Mappings.   

Put file [jsonSchemas.xml](https://raw.githubusercontent.com/5n00p4eg/Drupal-json-schemas/master/configs/jsonSchemas.xml) inside of .idea dir in your PhpStorm project dir.
### PhpStorm (manual)
1. Open `File | Settings | Languages & Frameworks | Schemas and DTDs | JSON Schema Mappings`
1. Add needed:
   * *Drupal info*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/info.yml.json`   
       pattern: `*.info.yml`
   * *Drupal layouts*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/layouts.yml.json`   
       pattern: `*.layouts.yml`
   * *Drupal libraries*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/schema/libraries.yml.json`   
       pattern: `*.libraries.yml`
   * *Drupal links (task)*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/links.task.yml.json`   
       pattern: `*.links.task.yml`
   * *Drupal permissions*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/permissions.yml.json`   
       pattern: `*.permissions.yml`
   * *Drupal routing*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/routing.yml.json`   
       pattern: `*.routing.yml`
   * *Drupal services*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/services.yml.json`   
       pattern: `*.services.yml`
   * *Drupal breakpoints*   
      url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/breakpoints.yml.json`   
      pattern: `*.breakpoints.yml`
   * *Drush site aliases*   
       url: `https://5n00p4eg.github.io/Drupal-json-schemas/schema/site.alias.yml.json`   
       pattern: `*.site.yml`
   
