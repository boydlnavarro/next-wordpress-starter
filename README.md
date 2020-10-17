# Next.js WordPress Starter

[![Netlify Status](https://api.netlify.com/api/v1/badges/24a546d8-e917-4e55-9e86-74bf437d651b/deploy-status)](https://app.netlify.com/sites/next-wordpress-starter/deploys)

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

Scaling WordPress with the power of Next.js and the static web!

## ⚡️ Quick Start

```bash
yarn create next-app -e https://github.com/colbyfayock/next-wordpress-starter
# or
npx create-next-app -e https://github.com/colbyfayock/next-wordpress-starter
```

Add an `.env.local` file to the root with the following:
```
WORDPRESS_HOST="http://wordpressite.com"
```

## 🚀 Getting Started

### Requirements
* [WordPress](https://wordpress.org/) project
* [WPGraphQL](https://www.wpgraphql.com/)

### Environment

This project makes use of WPGraphQL to query WordPress with GraphQL. In order to make that request to the appropriate endpoint, we need to set a environment variable to let Next.js know where to request the site information from.

Create a new file locally called `.env.local` and add the following:

```bash
WORDPRESS_HOST="[host]"
```

Replace `[host]` with your the home URL of your WordPress instance.

### Development

To start the project locally, run:

```bash
yarn dev
# or
npm run dev
```

The project should now be available at [http://localhost:3000](http://localhost:3000)!

## 🛠 Configuring Your Project

### package.json

In order to avoid an additional configuration file, we take advantage of some built-in properties of `package.json` to configure parts of the website.

- homepage: Setting the `homepage` property will update instances where the full URL is required such as Open Graph tags

### WordPress

This project aims to take advantage of as many built-in WordPress features by default. Those include:

- Site Title: Used for the homepage header as well as page metadata
- Tagline: Used on the homepage for the header subtitle
- Site Language: Used on the `<html>` tag to set the `lang` attribute

There is some specific WordPress configuration required to allow for the best use of this starter.

### Images

By default, this Starter doesn't provide any mechanisms for dealing with image content from WordPress. The images are linked to "as is", meaning if the image is uploaded via the WordPress interface, the image will be served from WordPress.

To serve the images statically, you have a few options.

#### Jetpack

By enabling the Image Accelerator from Jetpack, your images will automatically be served statically and cached via the wp.com CDN. This feature comes free with the basic installation of Jetpack, requiring only that you connect the WordPress site to the Jetpack service.

[Jetpack CDN](https://jetpack.com/features/design/content-delivery-network/)

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://colbyfayock.com/newsletter"><img src="https://avatars2.githubusercontent.com/u/1045274?v=4" width="100px;" alt=""/><br /><sub><b>Colby Fayock</b></sub></a><br /><a href="https://github.com/colbyfayock/next-wordpress-starter/commits?author=colbyfayock" title="Code">💻</a> <a href="https://github.com/colbyfayock/next-wordpress-starter/commits?author=colbyfayock" title="Documentation">📖</a></td>
    <td align="center"><a href="http://www.kevincunningham.co.uk"><img src="https://avatars3.githubusercontent.com/u/8320213?v=4" width="100px;" alt=""/><br /><sub><b>Kevin Cunningham</b></sub></a><br /><a href="https://github.com/colbyfayock/next-wordpress-starter/commits?author=doingandlearning" title="Code">💻</a></td>
    <td align="center"><a href="http://guilleangulo.me"><img src="https://avatars0.githubusercontent.com/u/50624358?v=4" width="100px;" alt=""/><br /><sub><b>Guillermo Angulo</b></sub></a><br /><a href="https://github.com/colbyfayock/next-wordpress-starter/commits?author=GuilleAngulo" title="Code">💻</a></td>
    <td align="center"><a href="http://www.heinsnyman.co.za"><img src="https://avatars0.githubusercontent.com/u/22816814?v=4" width="100px;" alt=""/><br /><sub><b>Hein Snyman</b></sub></a><br /><a href="https://github.com/colbyfayock/next-wordpress-starter/commits?author=HeinSnyman" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
