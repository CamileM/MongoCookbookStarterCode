# MongoDB Cookbook 'mongo'

DESCRIPTION:

- This repo will include the details on using the MongoDB. This cookbook is set
to install MongoDB from its source, as it creates its own package and then installs it.

## What is Chef?

- Chef is an Configuration Management Tool, chef allows files on the machine to be
configured, and it ensures that the machine is responding correctly and accordingly.

## How to use Cookbook?

- In a small and detailed concept, in order to run the recipe file we will need to
provision the code on to the machine as it will allow us to test the environment.

## Pre-requisites (Things We've Used):
- Chef
- GitHub
- AWS CLI Version 2

## Installs:
- MongoDB

## Options and Variables

Changes are made in the 'attributes' file
- Changing the port:
````
default['mongo']['port'] = <new_value_here>
````

## Commands Used For Testing in Chef

### Test Locally

1. Running the Unit Test:
````
chef exec rspec
````

2. Running the Integration Test and closing the machine:
````
kitchen test
````

### Test in AWS

Running Integration Test in AWS:
````
KITCHEN_YAML=kitchen_cloud.yml kitchen test
````
