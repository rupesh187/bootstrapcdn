# BootstrapCDN An Amazing Project

[![LGTM alerts](https://img.shields.io/lgtm/alerts/g/MaxCDN/bootstrapcdn.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/MaxCDN/bootstrapcdn/alerts/)
[![Build Status](https://github.com/MaxCDN/bootstrapcdn/workflows/Tests/badge.svg)](https://github.com/MaxCDN/bootstrapcdn/actions)
[![Coverage Status](https://img.shields.io/coveralls/github/MaxCDN/bootstrapcdn/develop.svg?style=flat-square)](https://coveralls.io/github/MaxCDN/bootstrapcdn)
[![dependencies Status](https://img.shields.io/david/MaxCDN/bootstrapcdn.svg?style=flat-square)](https://david-dm.org/MaxCDN/bootstrapcdn)
[![devDependencies Status](https://img.shields.io/david/dev/MaxCDN/bootstrapcdn.svg?style=flat-square)](https://david-dm.org/MaxCDN/bootstrapcdn?type=dev)

[![Backers on Open Collective](https://img.shields.io/opencollective/backers/getbootstrapcdn.svg?style=flat-square)](#backers)
[![Sponsors on Open Collective](https://img.shields.io/opencollective/sponsors/getbootstrapcdn.svg?style=flat-square)](#sponsors)

## Deploy your own copy on Heroku

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Requirements

1. [Node.js](https://nodejs.org/)

## Running

Use `npm run <task>`.

### Development

```sh
npm install

npm test && npm run dev
```

### Demonized

```shell
# start development server and watch for changes
npm run dev
# or
npm run watch

# start production server
npm start

# and more
npm run
```

## Configuration

### `config/_app.yml`

The Express.js app configuration.

* port: Integer value of the Node application port.
* theme: Integer value of the default theme we use; it's the array index value from the `bootswatch4` section below.
* siteurl: Our canonical URL.
* authors: Array of author Objects. Accepts the following:
    * name
    * twitter: the Twitter handler without `@`
    * url: author's website URL (optional)
    * work: (optional) Object which can contain:
        * text: the text to show for the `url` bellow
        * url: the link to the work
* description: String containing the default meta description of the site.
* favicon: The path to `favicon.ico`.
* stylesheet: Array of stylesheet file(s) we use apart from the Bootswatch stylesheet.
* javascript: Array of javascript file(s) we use.
* redirects: Array of Objects for the page redirects.

### `config/_extras.yml`

Contains the `/showcase/` and `/integrations/` config we use in the Express.js app.

### `config/_files.yml`

Contains the CDN files we host.The SRI values are updated by running `npm run integrity`.

### `config/helmet-csp.js`

Our CSP config using <https://github.com/helmetjs/csp>

## Updating Bootstrap/Bootlint/Bootswatch

Replace `package` by the package you want to update and `version` with its version in the following commands:

```shell
npm i package@version -ED
npm run package version
```

1. Update `config/_config.yml` accordingly
2. `npm run integrity`
3. Make sure `npm run all` passes after the files are on S3/CDN and verify the frontend works as expected without any visual breakage

## Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/getbootstrapcdn#backer)]

[![Bakers](https://opencollective.com/getbootstrapcdn/backers.svg?width=890)](https://opencollective.com/getbootstrapcdn#backers)

## Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/getbootstrapcdn#sponsor)]

[![OC sponsor 0](https://opencollective.com/getbootstrapcdn/sponsor/0/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/0/website)
[![OC sponsor 1](https://opencollective.com/getbootstrapcdn/sponsor/1/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/1/website)
[![OC sponsor 2](https://opencollective.com/getbootstrapcdn/sponsor/2/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/2/website)
[![OC sponsor 3](https://opencollective.com/getbootstrapcdn/sponsor/3/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/3/website)
[![OC sponsor 4](https://opencollective.com/getbootstrapcdn/sponsor/4/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/4/website)
[![OC sponsor 5](https://opencollective.com/getbootstrapcdn/sponsor/5/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/5/website)
[![OC sponsor 6](https://opencollective.com/getbootstrapcdn/sponsor/6/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/6/website)
[![OC sponsor 7](https://opencollective.com/getbootstrapcdn/sponsor/7/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/7/website)
[![OC sponsor 8](https://opencollective.com/getbootstrapcdn/sponsor/8/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/8/website)
[![OC sponsor 9](https://opencollective.com/getbootstrapcdn/sponsor/9/avatar.svg)](https://opencollective.com/getbootstrapcdn/sponsor/9/website)
