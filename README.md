# rwanda

[![Build Status](https://travis-ci.org/knowbee/rwanda.svg?branch=master)](https://travis-ci.org/knowbee/rwanda)
[![Maintainability](https://api.codeclimate.com/v1/badges/3f5c5282ff06934496dd/maintainability)](https://codeclimate.com/github/knowbee/rwanda/maintainability)
[![npm](https://img.shields.io/npm/dt/rwanda.svg)](https://www.npmjs.com/package/rwanda)
[![Dependency Status](https://david-dm.org/knowbee/rwanda.svg)](https://david-dm.org/knowbee/rwanda)
[![npm](https://img.shields.io/npm/v/rwanda.svg)](https://www.npmjs.com/package/rwanda)
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
[![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)

[![NPM](https://nodei.co/npm/rwanda.png)](https://nodei.co/npm/rwanda/)

This is a simple npm package that returns provinces, districts, sectors, villages and cells found in Rwanda.

Rwanda is organized in four provinces in addition to the Kigali city, 30 Districts, 416 Sectors, 2148 Cells and 14 837 Villages.

## Example

```js
const { Provinces, Districts } = require("rwanda");

console.log(Provinces()); // [ 'East', 'Kigali', 'North', 'South', 'West' ]
console.log(Districts()); // [ 'Bugesera', 'Gatsibo', 'Kayonza', 'Kirehe',...]
```

And how to get districts of a given province

```js
const { District } = require("rwanda");

console.log(District("kigali")); // [ 'Gasabo', 'Kicukiro', 'Nyarugenge' ]
```

## Methods

Usage:

```js
const {
  Provinces,
  Districts,
  Sectors,
  Cells,
  Villages,
  District,
  Sector,
  Cell,
  Village,
} = require("rwanda");
```

All inputs are case-insensitive.

### Provinces()

Returns array of country provinces.

```js
["East", "Kigali", "North", "South", "West"];
```

### Districts()

Returns array of country districts.

### Sectors()

Returns array of country sectors.

### Cells()

Returns an array of all country cells.

### Villages()

Returns an array of all country villages.

### District(province)

Returns an array of districts found in the given province.
It returns `undefined` if province is not found.

### Sector(province, district)

Returns an array of sectors found in the given province and district.
It returns `undefined` if either province or district is not found.

### Cell(province, district, sector)

Returns an array of Cells found in the given province, district, and sector.
It returns `undefined` if either province, district or sector is not found.

### Village(province, district, sector, cell)

Returns an array of Villages found in the given province, district, sector and cell.
It returns `undefined` if either province, district , sector or cell is not found.

## Install

```cli
npm install rwanda
```

or

```cli
yarn add rwanda
```

# Contributors

| [<img src="https://github.com/oesukam.png" width="100px;"><br><sub><b>Olivier Esuka</b></sub>](https://github.com/oesukam) | [<img src="https://github.com/knowbee.png" width="100px;"><br><sub><b>Igwaneza Bruce</b></sub>](https://github.com/knowbee) |
| :------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------: |


# Contribution

- Please before making a PR, read first this [Contributing Guideline](./CONTRIBUTING.md)

## License

MIT

## Author

Igwaneza Bruce
