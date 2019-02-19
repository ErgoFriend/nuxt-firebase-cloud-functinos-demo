# nuxt-cloud-functinos-demo

> My rad Nuxt.js project

## add to package.json

```json
{
    "scripts": {
        "copy": "cpx .nuxt/**/* .functions/functions/ &&  cpx .nuxt/dist/client/**/* .functions/hosting/static/ &&  cpx static/**/* .functions/hosting/"
    },
    "devDependencies": {
        "cpx": "^1.5.0"
    }
}
```

## Build Setup

``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn run dev

# build for production and launch server
$ yarn run build
$ yarn start

# generate static project
$ yarn run generate
```

For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).
