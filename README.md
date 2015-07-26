messa - mongoose express scaffold with angular.js
====

messa is an ExpressJS app to scaffold a CRUD UI for your mongoose models built with angular.js  

## Demo

You can see a live demo [here](https://messa-demo.herokuapp.com/)

## Installation

`npm i messa`

## Usage

messa is an ExpressJS application, as such it can either be used standalone or mounted into an existing application

### Mounted

```js
app.use('/messa', messa(mongoose));
```

### Standalone 

```js
messa(mongoose).listen(3000);
```

## API

`messa(mongoose[, options])`

*mongoose*: a mongoose instance, possibly configured with some models

*options*: a javascript object

- *options.title*: a custom title to override the default 

*Returns*: an ExpressJS app that you can run or mount into another app

## Features

- supports most types of mongoose schemas
- client-side validation based on mongoose validators (where possible)

## Limitations

- limited support for Array schema types, except for arrays of nested schemas, which is well supported

Please do not use with production data!

## Built on top of these great open source projects

- ExpressJS
- mongoose
- angular.js
- angular-material
- angular-ui-grid
