JSHashtable for nodejs
==================

PLEASE NOTE NodeJS now supports [Map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map) which achieves natively what this library attempts to do.

Port of jshashtable as nodejs package. jshashtable is a standalone implementation of hash table in JavaScript. It associates keys with values, and allows any object to be used as the key (unlike JavaScript's built-in Object, which only allows strings as property names).

Original website:
http://www.timdown.co.uk/jshashtable/


Installation:
-------------

npm install jshashtable

Usage:
------

    var Hashtable = require('jshashtable');
    var typesHash = new Hashtable();

    typesHash.put("A string", "string");
    typesHash.put(1, "number");

    var o = {};
    typesHash.put(o, "object");

    console.log( typesHash.get(o) ); // "object"
