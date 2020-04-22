# MongoDB Cookbook

Description:

This cookbook installs mongodb from source. It creates its own package and then
installs it. The recipe also creates the config files and the service files with
dynamic input of variables.

## Installs
- Monngodb

## Options and variables

Changes are made in the 'attributes' file
- Changing the port:
````
default['mongo']['port'] = <new_value_here>
````

## Commands

## Test Locally

1. Running my Unit Test:
````
chef exec rspec
````

2. Running my Intergration Test and closing the machine:
````
kitchen test
````

## Test in AWS

Running Intergration Test in AWS:
````
KITCHEN_YAML=kitchen_cloud.yml kitchen test
````
