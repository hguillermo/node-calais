# node-calais #

node-calais allows semantic analysis of text using the Calais web service.

## Install ##

Install using npm:
    $ npm install calais

## Usage ##

    var calais = new Calais('<YOUR API KEY>')
    calais.set('content', 'The Federal Reserve is the enemy of Ron Paul.')
    calais.fetch(function(result) {
      // do something with result
    })

## Example ##

Run quick example:
    $ node example.js

## Options ##

In addition to using the "set" method, a hash of option settings can be passed
as the second argument when constructing. For example:

    var calais = new Calais('<YOUR API KEY>', {'cleanResult': false})

Any Calais input parameter can be passed, as well as the 'cleanResult' parameter
(which can be set to false to show the raw Calais result).

** Test **

Run tests:
    $ expresso test/calais.test.js

Tested with node.js v0.3.0

(c) 2010 Mike Cantelon, MIT license