# .functions

Plz `npm run build` at project root

## mkdir & files
package.json
functions
hosting
hosting/static

## package.json

```json
{
  "name": "functions",
  "description": "Nuxt-SSR-Firebase: Nuxt.js with Firebase Functions Production Setup",
  "dependencies": {
    "express": "^4.15.3",
    "firebase-admin": "^7.0.0",
    "firebase-functions": "^2.2.0",
    "nuxt": "^2.4.0"
  },
  "scripts": {
    "clean": "rimraf ./functions/* && rimraf ./hosting/*",
    "copy": "cpx ../.nuxt/ ./functions &&  cpx ../.nuxt/dist/client/ ./hosting/static &&  cpx ../static/ hosting",
    "deploy": "firebase login && firebase use --add && firebase deploy"
  },
  "devDependencies": {
    "rimraf": "^2.6.3",
    "cpx": "^1.5.0"
  },
  "engines": {
    "node": "8"
  },
  "private": true
}
```

`npm install`

`npm run clean`

`npm run copy`

`npm run deploy`