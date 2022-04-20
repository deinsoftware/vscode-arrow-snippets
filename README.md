# Arrow Function Snippets

[![Version](https://vsmarketplacebadge.apphb.com/version/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![license](https://img.shields.io/github/license/deinsoftware/vscode-arrow-snippets)](LICENSE.md)
[![Open in VS Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/deinsoftware/vscode-arrow-snippets)

![Arrow](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/social/preview.png 'Arrow Function Snippets')

The quick and easy way to create and use [Arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) with [VS Code](https://code.visualstudio.com/).

> We also **recommend** installing his complement extension [Const & Props Snippets](https://marketplace.visualstudio.com/items?itemName=deinsoftware.const-props-snippets)

## Menu

- [Installation](#installation)
  - [Quick Launch](#quick-launch)
  - [Extension Manager](#extension-manager)
  - [Marketplace](#marketplace)
- [Supported Languages](#supported-languages)
- [Regular VS Arrow Functions](#regular-vs-arrow-functions)
- [Snippets](#snippets)
  - [Arrow Function](#arrow-function)
  - [Promises](#promises)
  - [Arrays](#arrays)
  - [Variables](#variables)
  - [Functions](#functions)
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

⇧ [Back to menu](#menu)

---

## Regular VS Arrow Functions

### Syntax

The arrow function allows to accomplish the same result with fewer lines of code and approximately half the typing.
Curly brackets aren't required if only one expression is present.

### Arguments binding

Arrow functions do not have an arguments binding. But the same functionality can be achieved using rest parameters.

### Use of this keyword

Unlike regular functions, arrow functions do not have their own `this`. The value of `this` inside an arrow function remains the same throughout the lifecycle of the function and is always bound to the value of `this` in the closest non-arrow parent function.

### Using new keyword

Regular functions created using function declarations or expressions are constructible and callable. Since regular functions are constructible, they can be called using the `new` keyword. However, the arrow functions are only callable and not constructible, so arrow functions can never be used as constructor functions. Hence, they can never be invoked with the `new` keyword.

### No duplicate named parameters

Arrow functions can never have duplicate named parameters, whether in strict or non-strict mode.

⇧ [Back to menu](#menu)

---

## Snippets

Below is a list of all available snippets and the triggers of each one. The **→** means the `TAB` key and `█` the final cursor position.

### Arrow Function

|  Trigger | Description                            | Result JS/TS                                                     |
| -------: | -------------------------------------- | ---------------------------------------------------------------- |
|    `af→` | implicit return without arg(s          | `() => █`                                                        |
|   `afa→` | implicit return with arg(s)            | `(arg) => █`                                                     |
|  `afad→` | implicit return with arg destructuring | `({prop, prop}) => █`                                            |
|   `afo→` | implicit return object                 | `() => ({prop: value█})`                                         |
|  `afoa→` | implicit return object with arg(s)     | `(arg) => ({prop: value█})`                                      |
|   `afe→` | explicit return                        | <code>() => {<br/>&nbsp;&nbsp;return █<br/> }</code>             |
|  `afea→` | explicit return with arg(s)            | <code>(arg) => {<br/>&nbsp;&nbsp;return █<br/> }</code>          |
| `afead→` | explicit return with arg destructuring | <code>({prop, prop}) => {<br/>&nbsp;&nbsp;return █<br/> }</code> |
|  `afee→` | explicit empty                         | <code>() => {<br/>&nbsp;&nbsp;█<br/> }</code>                    |
| `afeea→` | explicit empty with arg(s)             | <code>(arg) => {<br/>&nbsp;&nbsp;█<br/> }</code>                 |
|   `afp→` | explicit with parentheses              | <code>() => {<br/>&nbsp;&nbsp;(█)<br/> }</code>                  |
|  `afpa→` | explicit with parentheses and arg(s)   | <code>(arg) => {<br/>&nbsp;&nbsp;(█)<br/> }</code>               |
|  `iiaf→` | immediately invoque                    | `(() => █)()`                                                    |

### Promises

|  Trigger | Description                         | Result JS/TS                                                                  |
| -------: | ----------------------------------- | ----------------------------------------------------------------------------- |
|   `afr→` | implicit return response            | `(response) => █`                                                             |
|  `afrj→` | implicit return response json       | `(response) => response.json()█`                                              |
|  `afrd→` | implicit return response data       | `(response) => response.data█`                                                |
|  `afer→` | explicit return response            | <code>(response) => {<br/>&nbsp;&nbsp;return █<br/> }</code>                  |
| `aferj→` | explicit return response json       | <code>(response) => {<br/>&nbsp;&nbsp;return response.json()<br/> }█</code>   |
| `aferd→` | explicit return response data       | <code>(response) => {<br/>&nbsp;&nbsp;return response.data<br/> }█</code>     |

### Arrays

|  Trigger  | Description             | Result JS/TS                                                                             |
| --------: | ------------------------| ---------------------------------------------------------------------------------------- |
| `arfeq→`  | filter equal            | `const newArray = array.filter((element) => element === value)█`                         |
| `arfne→`  | filter not equal        | `const newArray = array.filter((element) => element !== value)█`                         |
| `arfoeq→` | filter object equal     | `const newArray = array.filter((element) => element.prop === value)█`                    |
| `arfone→` | filter object not equal | `const newArray = array.filter((element) => element.prop !== value)█`                    |
| `arsna→`  | sort number ascending   | `array.sort((a, b) => a - b)█`                                                           |
| `arsnd→`  | sort number descending  | `array.sort((a, b) => b - a)█`                                                           |
| `aruv→`   | unique values           | `const newArray = array.filter((current, index, arr) => arr.indexOf(current) == index)█` |

### Variables

|  Trigger | Description                  | Result JS            | Result TS                                         |
| -------: | ---------------------------- | -------------------- | ------------------------------------------------- |
|    `cv→` | const variable               | `const name = █`     | `const name = █`                                  |
|   `cvt→` | const variable type          |                      | `const name: type = █`                            |
|   `cvm→` | const variable multiple type |                      | <code>const name: (type &#124; type) = █</code>   |
|    `cs→` | const string                 | `const name = '█'`   | `const name: string = '█'`                        |
|    `cn→` | const number                 | `const name = 0█`    | `const name: number = 0█`                         |
|    `cb→` | const boolean                | `const name = true█` | `const name: boolean = true█`                     |
|    `co→` | const object                 | `const name = {█}`   | `const name = {█}`                                |
|   `coi→` | const object interface       |                      | `const name: Interface = {█}`                     |
|    `ca→` | const array                  | `const name = [█]`   | `const name = [█]`                                |
|   `cat→` | const array type             |                      | `const name: type = [█]`                          |
|   `cam→` | const array multiple type    |                      | <code>const name: (type &#124; type) = [█]</code> |

### Functions

|  Trigger | Description                                     | Result JS                                                                | Result TS                                                                      |
| -------: | ----------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
|   `edaf→` | export default anonymous arrow function        | <code>export default () => {<br/>&nbsp;&nbsp;█<br/> }</code>             | <code>export default () => {<br/>&nbsp;&nbsp;█<br/> }</code>                   |
|  `edaaf→` | export default async anonymous arrow function  | <code>export default async () => {<br/>&nbsp;&nbsp;█<br/> }</code>       | <code>export default async () => {<br/>&nbsp;&nbsp;█<br/> }</code>             |
|    `caf→` | const arrow function                           | <code>const name = () => {<br/>&nbsp;&nbsp;█<br/> }</code>               | <code>const name = () => {<br/>&nbsp;&nbsp;█<br/> }</code>                     |
|   `ecaf→` | export const arrow function                    | <code>export const name = () => {<br/>&nbsp;&nbsp;█<br/> }</code>        | <code>export const name = () => {<br/>&nbsp;&nbsp;█<br/> }</code>              |
|   `caaf→` | const async arrow function                     | <code>const name = async () => {<br/>&nbsp;&nbsp;█<br/> }</code>         | <code>const name = async () => {<br/>&nbsp;&nbsp;█<br/> }</code>               |
|  `ecaaf→` | export const async arrow function              | <code>export const name = async () => {<br/>&nbsp;&nbsp;█<br/> }</code>  | <code>export const name = async () => {<br/>&nbsp;&nbsp;█<br/> }</code>        |
|   `caft→` | const arrow function with type                 |                                                                          | <code>const name = () : type => {<br/>&nbsp;&nbsp;█<br/> }</code>              |
|  `ecaft→` | export const arrow function with type          |                                                                          | <code>export const name = () : type => {<br/>&nbsp;&nbsp;█<br/> }</code>       |
|  `caaft→` | const async arrow function with type           |                                                                          | <code>const name = async () : type => {<br/>&nbsp;&nbsp;█<br/> }</code>        |
| `ecaaft→` | export const async arrow function with type    |                                                                          | <code>export const name = async () : type => {<br/>&nbsp;&nbsp;█<br/> }</code> |

⇧ [Back to menu](#menu)

---

## Examples

Create a named arrow function combining `cv` and `af`

![Function](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-function.gif 'Function')

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
[![buymeacoffee](https://img.shields.io/badge/-Buy%20Me%20A%20Coffee-gray?style=flat&labelColor=FF813F&logo=buy-me-a-coffee&logoColor=white&link=https://buymeacoff.ee/equiman)](https://www.buymeacoffee.com/equiman)

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

⇧ [Back to menu](#menu)
