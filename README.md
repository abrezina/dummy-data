# dummy-data

Simple node.js library for generating dummy data for tests or to use fake names for anomym data

## install

```sh 
npm install --save @abrezina/dummy-data
```

## person generator

Generates a person object with firstname, surname and country. 
Firstname and surname are the 98 most common for the country. 
The country is one of DE, US and JP. 

### example

```js
var personGenerator = require('@abrezina/dummy-data').personGenerator;

var randomPerson = personGenerator.generate();

console.log('Hello %s %s from %s', randomPerson.firstname, randomPerson.surname, randomPerson.country);
```