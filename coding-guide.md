# Coding guide

## Naming

### Software

Variables, class names etc. should be written in camel case whenever possible. Only if widely supported programming
standards like [PEP-8](https://peps.python.org/pep-0008/#function-and-variable-names) in Python say otherwise, then in
their context their preferred style should be used.

Names should be descriptive of their function.

Boolean variables and functions should start with `is...` or `has...`.

Modules should be used whenever possible.

Name collisions within the same module must be avoided at all costs.

Name collisions within the Ember Nexus organisation should be avoided if namespaced modules exist, and must be avoided
in regard to global variables etc.

Within the Ember Nexus organisation the same names should be used to identify functionally identical parts.

### CI, infrastructure

CI task names should be written as `Function (tool)`, i.e. being descriptive in what the task is, while also giving
credits to the tool and providing context for users who know the tool.

### Repository structure

The top level of repositories should be limited to important files and folders only.

If files can not be moved to other places due to technical reasons, they can remain in the top level, even if
discouraged.

For folders the singular form is the only acceptable variant. No abbreviation should be used.

Files must include their file type. Important files might have their name capitalized.

The following folders and files should be included by default:

```txt
source/             # source code
test/               # folder for all tests, still uses singular
  unit/             # unit tests
  feature/          # feature tests
documentation/      # documentation, should be hostable as a static website
LICENSE.md          # license, legal document
README.md           # readme, firt interaction point
CHANGELOG.md        # changelog, contains the list of changes over time
```
