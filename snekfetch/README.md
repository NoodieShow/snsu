[![npm](https://img.shields.io/npm/v/snekfetch.svg?maxAge=3600)](https://www.npmjs.com/package/snekfetch)
[![npm](https://img.shields.io/npm/dt/snekfetch.svg?maxAge=3600)](https://www.npmjs.com/package/snekfetch)
[![David](https://david-dm.org/guscaplan/snekfetch.svg)](https://david-dm.org/guscaplan/snekfetch)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bhttps%3A%2F%2Fgithub.com%2Fdevsnek%2Fsnekfetch.svg?type=shield)](https://app.fossa.io/projects/git%2Bhttps%3A%2F%2Fgithub.com%2Fdevsnek%2Fsnekfetch?ref=badge_shield)

[![NPM](https://nodei.co/npm/snekfetch.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/snekfetch/)

# snekfetch

Snekfetch is a fast, efficient, and user-friendly library for making
HTTP requests.

The API was inspired by superagent, and any methods that snekfetch has should
be dropin with superagent.

Documentation is available as JSDOC in `src/index.js`

## Some examples

```js
const snekfetch = require('snekfetch');

snekfetch.get('https://s.gus.host/o-SNAKES-80.jpg')
  .then(r => fs.writeFile('download.jpg', r.body);

snekfetch.get('https://s.gus.host/o-SNAKES-80.jpg')
  .pipe(fs.createWriteStream('download.jpg'));
```

```js
const snekfetch = require('snekfetch');

snekfetch.post('https://httpbin.org/post')
  .send({ meme: 'dream' })
  .then(r => console.log(r.body));
```


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bhttps%3A%2F%2Fgithub.com%2Fdevsnek%2Fsnekfetch.svg?type=large)](https://app.fossa.io/projects/git%2Bhttps%3A%2F%2Fgithub.com%2Fdevsnek%2Fsnekfetch?ref=badge_large)