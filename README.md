# Yo Extend

Maintainer: [Simon Fan](https://github.com/simonfan)

## Documentation conventions

For simplicity's sake it is important to have a set of 
conventions in this man page. 

_generator_ refers to the generator-package at which the 
`yo extend` method was invoked.

_parent-generator_ refers to a generator-package from 
which _generator_ inherits subgenerators.

_GENERATED-PROJECT_ refers to the project that should be 
scaffolded by _generator_.


## Usage

Install `generator-extend`:

    npm install -g generator-extend

Make a new directory, and `cd` into it:

    mkdir my-new-generator && cd $_

Start your generator:

    yo generator

Run any of the following:

    yo extend
    yo extend %someGenerator
    yo extend %someGenerator:%someSubGenerator
    yo extend %someGenerator:%someSubGenerator,%someOtherSubGenerator,%andYetAnother

## Prompts

#### `generator`

The _parent-generator_.

#### `subgenerators`

The subgenerators that the _generator_ should inherit from the _parent-generator_.

#### `package`
#### `version_or_source`

The npm package name for the _parent-generator_.
dependencies: {
    _parent-generator_: _version_or_package_source_
}


## Under the hood

### Proxy Generators

Generator inheritance is 

### Dependency transfers

