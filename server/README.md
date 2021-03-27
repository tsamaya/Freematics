# Freemantics server / hub

cd ./server/teleserver

## Build

```bash
make
```

## Run

### server

```bash
./teleserver
```

### webapp

and now the webapp:

#### config file

edit [server/teleserver/htdocs/config.js](.teleserver/htdocs/config.js)

```js
// const DATA_FETCH_INTERVAL = 500;
const DATA_FETCH_INTERVAL = 10000;

...

var OPENCAGE_API_KEY = '6c79ee8e1ca44ad58ad1fc493ba9542f'; // 403 IP Blocked
// var OPENCAGE_API_KEY = '2e10e5e828262eb243ec0b54681d699a'; // 403 disabled
// var OPENCAGE_API_KEY = 'd6d0f0065f4348a4bdfe4587ba02714b'; // 429
// var OPENCAGE_API_KEY = '4372eff77b8343cebfc843eb4da4ddc4'; // 402 quota exceeded

// var OPENCAGE_API_KEY = YOUR KEY


// const serverURL =
//   window.location.href.substr(0, 7) == 'file://'
//     ? 'http://localhost:8080/api/'
//     : window.location.href.indexOf('localhost') > 0
//     ? '/api/'
//     : '/hub/api/';
const serverURL = 'http://localhost:8080/api/';

```

#### chrome

quit all chrome sessions

<!-- rm -rf ./chromedata/* -->

```
open -n -a /Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --args --user-data-dir="./chromedata" --disable-web-security

open ./htdocs/simulator.html
allow localisation
login

open ./htdocs/dashboard.html
ID : SIMULATOR
```

#### brave

open -n -a /Applications/Brave\ Browser.app/Contents/MacOS/Brave\ Browser --args --user-data-dir="./chromedata" --disable-web-security

### open

file:///Users/arnaud/projects/github/Freematics/server/teleserver/htdocs/dashboard.html

file:///Users/arnaud/projects/github/Freematics/server/teleserver/htdocs/simulator.html
