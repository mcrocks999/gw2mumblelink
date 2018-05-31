# Guild Wars 2 Mumble Link
Retrieve data from the GW2 client through the data exposed for Mumble.

[![NPM](https://nodei.co/npm/gw2mumblelink.png)](https://nodei.co/npm/gw2mumblelink/)

[![npm](https://img.shields.io/npm/dt/gw2mumblelink.svg)](https://www.npmjs.com/package/gw2mumblelink)

## Quick Start

Below is a short snippet, I recommend looking through the examples folder to find what you're looking for.

```javascript
const MumbleLink = require('gw2mumblelink');
let mumbleLink = new MumbleLink();

if (!mumbleLink.init()) return console.error("Failed to initialise!");

mumbleLink.getName(); // Should be Guild Wars 2

let identity = mumbleLink.getIdentity();

console.log(identity.name); // Your character's name =)
```

## To-Do

- Create documentation for module
- Finish support for [ML struct](https://wiki.guildwars2.com/wiki/API:MumbleLink#MumbleLink_structure), this includes: f* vars, the context, desc and other variables.