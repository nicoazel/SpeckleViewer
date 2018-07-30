<a href="url"><img src="https://speckle.works/img/logos/2xlogo-white.png" align="left" height="128" ></a>
# speckle-viewer

> A simple Speckle.Works stream viewer, built with [VueJS](https://vuejs.org/). For more, check [speckle.works](https://speckle.works/doc/onlineviewer/).

![Image of Speckle Viewer](https://speckle.works/img/onlineviewer/headerimg4c.png)

More info to come.

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8888 (8080 is taken by the local speckle server instance 💯)
npm run dev

# build for production with minification
npm run build
```
## Deployment

You will need to modify the ./dist/config.js file to fit your deployment details. It’s rather self-descriptive, it just exports a global object with info:

```
var SpkAppConfig = {
  serverUrl: 'http://localhost:8080',
  allowGuestAccess: true,
  logoUrl: 'https://company.png'
}

window.SpkAppConfig = SpkAppConfig
```
It’s rather important to serve things to ```https``` and make sure the server is allowing ```cors```.

## Adding Streams Once Running

To add more streams, just add more stream ids to the url, separated by commas:
 ```https://s003.speckle.works/view/?ryuFyiHuz,rkf6JoHuf```
