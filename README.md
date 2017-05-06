# [FallenArk的Disucz主题]

FallenArk专属的Discuz主题，没什么好说的呀。

希望有前端能力的同学多多加入其中~

## Features
* Sass for stylesheets
* [Webpack](https://webpack.github.io/) for compiling assets, optimizing images, and concatenating and minifying files
* [Browsersync](http://www.browsersync.io/) for synchronized browser testing
* Remove the Auto-Width style.
* Remove Discuz DIY module.
* Support SSL/TLS .

## Requirements

开发环境需要准备以下工具：

* [Discuz](http://www.discuz.net/) >= 4.7
* [Node.js](http://nodejs.org/) >= 6.9.x
* [Yarn](https://yarnpkg.com/en/docs/install)

## Theme installation

During theme installation you will have the options to:

* Update theme headers (theme name, description, author, etc.)
* Select a CSS framework (Bootstrap, Foundation, none)
* Add Font Awesome
* Configure Browsersync (path to theme, local development URL)

## Theme structure

```shell
template/fallenark/       # → Root of Fallenark theme
├── assets/               # → Front-end assets
│   ├── config.json       # → Settings for compiled assets
│   ├── build/            # → Webpack and ESLint config
│   ├── fonts/            # → Theme fonts
│   ├── images/           # → Theme images
│   ├── scripts/          # → Theme JS
│   └── styles/           # → Theme stylesheets
├── common/               # → Common template modules.
├── dist/                 # → Built theme assets (never edit)
├── forum/                # → Template for forum
├── group/                # → Template for group
├── home/                 # → Template for home
├── member/               # → Template for member
├── mobile/               # → Template for mobile
├── node_modules/         # → Node.js packages (never edit)
├── package.json          # → Node.js dependencies and scripts
├── portal/               # → Template for portal
├── ranklist/             # → Template for ranklist
├── search/               # → Template for search
├── style/                # → Website style
├── tag/                  # → Template for tag page
├── touch/                # → Template for smartphone
├── userapp/              # → Template for user application
└── wml/                  # → Template for phone
```

## Theme development

* Run `yarn` from the theme directory to install dependencies
* Update `assets/config.json` settings:
  * `devUrl` should reflect your local development hostname
  * `publicPath` should reflect your Discuz folder structure (`/template/fallenark`) installs)

### Build commands

* `yarn run start` — Compile assets when file changes are made, start Browsersync session
* `yarn run build` — Compile and optimize the files in your assets directory
* `yarn run build:production` — Compile assets for production

