# Arrow Function Snippets

[![Version](https://vsmarketplacebadge.apphb.com/version/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![license](https://img.shields.io/github/license/deinsoftware/vscode-arrow-snippets)](LICENSE.md)
[![Open in VS Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/deinsoftware/vscode-arrow-snippets)

![Arrow](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/social/preview.png 'Arrow Function Snippets')

The quick and easy way to create and use [Arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) with [VS Code](https://code.visualstudio.com/).

## Menu

- [Installation](#installation)
  - [Quick Launch](#quick-launch)
  - [Extension Manager](#extension-manager)
  - [Marketplace](#marketplace)
- [Supported Languages](#supported-languages)
- [Snippets](#snippets)
  - [Arrow Function](#arrow-function)
  - [Promises](#promises)
  - [Helpers](#helpers)
  - [Variables](#variables)
  - [Destructuring](#destructuring)
  - [Object Elements](#object-elements)
  - [JSON Elements](#json-elements)
- [Examples](#examples)
- [About](#about)

---

## Installation

### Quick Launch

Open the quick launch with <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>P</kbd> (Win/Linux) or <kbd>cmd</kbd>+<kbd>shift</kbd>+<kbd>P</kbd> (macOS).

Paste the following command and press `Enter`:

```shell
ext install deinsoftware.arrow-function-snippets
```

### Extension Manager

Open the extension manager with <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>X</kbd> (Win/Linux) or <kbd>cmd</kbd>+<kbd>shift</kbd>+<kbd>X</kbd> (macOS), search for `Arrow Function Snippets` and click on `[Install]` button.

### Marketplace

[Arrow Function Snippets](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)

⇧ [Back to menu](#menu)

---

## Supported Languages

| Language         | Extension |
| ---------------- | --------- |
| JavaScript       | `.js`     |
| TypeScript       | `.ts`     |
| JavaScript React | `.jsx`    |
| TypeScript React | `.tsx`    |
| Vue              | `.vue`    |
| JSON ℹ️           | `.json`   |
| JSONC ℹ️          | `.jsonc`  |
| JSON5 ℹ️          | `.json5`  |

> ℹ️ Only JSON elements snippets are available

⇧ [Back to menu](#menu)

---

## Snippets

Below is a list of all available snippets and the triggers of each one. The **→** means the `TAB` key and `█` the final cursor position.

### Arrow Function

|  Trigger | Description                            | Result JS/TS                |
| -------: | -------------------------------------- | --------------------------- |
|    `af→` | implicit return without args           | `() => █`                   |
|   `afa→` | implicit return with arg(s)            | `(arg) => █`                |
|  `afad→` | implicit return with arg destructuring | `({prop, prop}) => █`       |
|   `afo→` | implicit return object                 | `() => ({prop: value█})`    |
|  `afoa→` | implicit return object with arg(s)     | `(arg) => ({prop: value█})` |
|   `afe→` | explicit return                        | <code>() => {<br>&nbsp;&nbsp;return █<br> }</code>        |
|  `afea→` | explicit return with arg(s)            | <code>(arg) => {<br>&nbsp;&nbsp;return █<br> }</code>     |
| `afead→` | explicit return with arg destructuring | <code>({prop, prop}) => {<br>&nbsp;&nbsp;return █<br> }</code>     |
|   `afp→` | explicit with parentesis               | <code>() => {<br>&nbsp;&nbsp;(█)<br> }</code>             |
|  `afpa→` | explicit with parentesis and arg(s)    | <code>(arg) => {<br>&nbsp;&nbsp;(█)<br> }</code>          |
|  `iiaf→` | immediately invoque                    | `(() => █)()`               |

### Promises

|  Trigger | Description                         | Result JS/TS                     |
| -------: | ----------------------------------- | -------------------------------- |
|   `afr→` | implicit return response            | `(response) => █`                |
|  `afrj→` | implicit return response json       | `(response) => response.json()█` |
|  `afrd→` | implicit return response data       | `(response) => response.data█`   |
|  `afer→` | explicit return response            | <code>(response) => {<br>&nbsp;&nbsp;return █<br> }</code> |
| `aferj→` | explicit return response json       | <code>(response) => {<br>&nbsp;&nbsp;return response.json()<br> }█</code> |
| `aferd→` | explicit return response data       | <code>(response) => {<br>&nbsp;&nbsp;return response.data<br> }█</code> |

### Helpers

|  Trigger | Description                         | Result JS/TS           |
| -------: | ----------------------------------- | ---------------------- |
| `afceq→` | compare equal       | `(element) => element.prop === value█` |
| `afcne→` | compare not equal   | `(element) => element.prop !== value█` |

### Variables

|  Trigger | Description                  | Result JS            | Result TS                          |
| -------: | ---------------------------- | -------------------- | ---------------------------------- |
|    `cv→` | const variable               | `const name = █`     | `const name = █`                   |
|   `cvt→` | const variable type          |                      | `const name: type = █`             |
|   `cvm→` | const variable multiple type |                      | <code>const name: (type &#124; type) = █</code>   |
|    `cs→` | const string                 | `const name = '█'`   | `const name: string = '█'`         |
|    `cn→` | const number                 | `const name = 0█`    | `const name: number = 0█`          |
|    `cb→` | const boolean                | `const name = true█` | `const name: boolean = true█`      |
|    `co→` | const object                 | `const name = {█}`   | `const name = {█}`                 |
|   `coi→` | const object interface       |                      | `const name: Interface = {█}`      |
|    `ca→` | const array                  | `const name = [█]`   | `const name = [█]`                 |
|   `cat→` | const array type             |                      | `const name: type = [█]`           |
|   `cam→` | const array multiple type    |                      | <code>const name: (type &#124; type) = [█]</code> |

### Destructuring

|  Trigger | Description                     | Result JS/TS                          |
| -------: | ------------------------------- | ------------------------------------- |
|   `cod→` | const object dest               | `const {prop, prop} = name█`          |
|  `codr→` | const object dest with rest     | `const {prop, prop, ...rest} = name█` |
|   `cad→` | const array dest                | `const [prop, prop] = name█`          |
|  `cadr→` | const array dest with rest      | `const [prop, prop, ...rest] = name█` |
|    `pd→` | parameter object dest           | `{prop, prop█}`                       |
|   `pdr→` | parameter object dest with rest | `{prop, prop, ...rest█}`              |

### Object Elements

|  Trigger | Description                  | Result JS/TS                       |
| -------: | ---------------------------- | ---------------------------------- |
|   `oev→` | obj element variable         | `key: value,█`                     |
|   `oes→` | obj element string           | `key: 'value',█`                   |
|   `oen→` | obj element number           | `key: number,█`                    |
|   `oeb→` | obj element boolean          | `key: true,█`                      |
|   `oeo→` | obj element object           | `key: {element},█`             |
|  `oeom→` | obj element object multiline | <code>key: {<br>&nbsp;&nbsp;element, <br>},█</code> |
|   `oea→` | obj element array            | `key: [value, ],█`                        |
|  `oeam→` | obj element array multiline  | <code>key: [<br>&nbsp;&nbsp;value, <br>],█</code> |

### JSON Elements

|  Trigger | Description                   | Result JS/TS                                            |
| -------: | ----------------------------- | ------------------------------------------------------- |
|   `jev→` | json element variable         | `key: value,█`                                       |
|   `jes→` | json element string           | `key: 'value',█`                                     |
|   `jen→` | json element number           | `key: number,█`                                      |
|   `jeb→` | json element boolean          | `key: true,█`                                        |
|   `jeo→` | json element object           | `key: { element }█`                                |
|  `jeom→` | json element object multiline | <code>key: {<br>&nbsp;&nbsp;element , <br>},█</code> |
|   `jea→` | json element array            | `key: [ value ],█`                                   |
|  `jeam→` | json element array multiline  | <code>key: [<br>&nbsp;&nbsp;value , <br>],█</code>   |

> ℹ️ Only available in `.json`, `.jsonc` and `.json5` files

⇧ [Back to menu](#menu)

---

## Examples

Create a named arrow function combining `cv` and `af`

![Function](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-function.gif 'Function')

Create a compare equal arrow function inside `.filter()` function with `afceq`

![Filter](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-filter.gif 'Filter')

Create a response for `fetch` promise with `afrj` and `afrd`

![Promise](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-promise.gif 'Promise')

⇧ [Back to menu](#menu)

---

## About

### Built With

- [VS Code](https://code.visualstudio.com/) - Code editing redefined.
- [Figma](https://www.figma.com/) - The collaborative interface design tool.

### Contributing

Please read [CONTRIBUTING](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

### Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [Arrow Function Snippets](https://github.com/deinsoftware/arrow-function-snippets/tags) on GitHub.

### Authors

- **Camilo Martinez** [[Equiman](http://stackoverflow.com/story/equiman)]

See also the list of [contributors](https://github.com/deinsoftware/arrow-function-snippets/contributors) who participated in this project.

### Sponsors

If this project helps you, consider buying me a cup of coffee.

[![paypal](https://img.shields.io/badge/-PayPal-gray?style=flat&labelColor=00457C&logo=paypal&logoColor=white&link=https://paypal.me/equiman/3)](https://paypal.me/equiman/3)
[![patreon](https://img.shields.io/badge/-Patreon-gray?style=flat&labelColor=052d49&logo=patreon&logoColor=F96854&link=https://patreon.com/equiman)](https://patreon.com/equiman)
[![buymeacoffee](https://img.shields.io/badge/-Buy%20Me%20A%20Coffee-gray?style=flat&labelColor=FF813F&logo=buy-me-a-coffee&logoColor=white&link=https://buymeacoff.ee/equiman)](https://buymeacoff.ee/equiman)

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

⇧ [Back to menu](#menu)
