# Netlify Builder demo
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors)

This repository contains an example of the Angular CLI Architect API.

## Builder

You can find the Architect builder in the `command-builder` directory.

## Sample application

The sample application which uses the Architect builder is available under the `builder-test` directory.

## License

MIT


## Setup

1. Move to command-builder and run the below command

```sh
yarn install
```

2. Run the below command to build the package

```sh
yarn build
```

3. run the below command to link the package

```
npm link
```

## To test pacakge

1. Move to builder-test and run the below command

```sh
yarn install
```

2. Link the package

```sh
npm link @netlify-builder/deploy
```

3. Provide below config in angular.json
```json
   "deploy": {
          "builder": "@netlify-builder/deploy:deploy",
          "options": {
            "command": "deploy",
            "outputPath": "dist/builder-test",
            "netlifyToken": "[tokenValue]",
            "siteId": "[siteId]",
            "args": [
              "src/main.ts"
            ]
          }
        }
```

4. Test the command

```sh
ng run builder-test:deploy
```
## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="https://www.youtube.com/c/NitishKumarSingh"><img src="https://avatars2.githubusercontent.com/u/15886737?v=4" width="100px;" alt="Nitish Kumar Singh"/><br /><sub><b>Nitish Kumar Singh</b></sub></a><br /><a href="https://github.com/ngx-builders/netlify-builder/commits?author=nitishk72" title="Code">💻</a></td>
  </tr>
</table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!