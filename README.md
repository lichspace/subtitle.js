# subtitle.js

Parse and manipulate SRT (SubRip) format.

## Installing

`npm install subtitle --save`

## Usage

```javascript
var Subtitle = require('subtitle');

var subtitle = new Subtitle('your srt here');

console.log(subtitle.parse());
```

It's gonna return an array like this:

```javascript
[
  {
    index: 1,
    start: '00:00:20,000',
    end: '00:00:24,400',
    text: 'Bla Bla Bla Bla'
  },
  {
    index: 2,
    start: '00:00:24,600',
    end: '00:00:27,800',
    text: 'Bla Bla Bla Bla'
  }
]
```

## Tests

`npm test`

## Roadmap
* [x] Basic SRT parser
* [ ] Basic manipulation
* [ ] Stringfy
* [ ] Time conversion
* [ ] Duration property
* [ ] WebVTT support
* [ ] Browser support (including for Browserify)
* [ ] Better docs