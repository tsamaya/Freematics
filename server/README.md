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
