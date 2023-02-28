# Arrow Function Snippets

[![Version](https://img.shields.io/visual-studio-marketplace/v/deinsoftware.arrow-function-snippets)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/deinsoftware.arrow-function-snippets)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Ratings](https://img.shields.io/visual-studio-marketplace/stars/deinsoftware.arrow-function-snippets)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![license](https://img.shields.io/github/license/deinsoftware/vscode-arrow-snippets)](LICENSE.md)
[![Open in VS Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/deinsoftware/vscode-arrow-snippets)

![Arrow](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/social/preview.png 'Arrow Function Snippets')

The quick and easy way to create and use [Arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) with [VS Code](https://code.visualstudio.com/).

> We also **recommend** installing his complement extensions [Const & Props Snippets](https://marketplace.visualstudio.com/items?itemName=deinsoftware.const-props-snippets) and [Debug](https://marketplace.visualstudio.com/items?itemName=deinsoftware.debug-snippets)

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
  - [Functions](#functions)
- [Examples](#examples)
- [Settings](#settings)
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
|    `af→` | implicit return without arg(s)         | `() => █`                                                        |
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
|  `afii→` | immediately invoque                    | `(() => █)()`                                                    |
|  `iiaf→` | immediately invoque                    | `(() => █)()`                                                    |

#### Async Arrow Functions

|  Trigger | Description                            | Result JS/TS                                                              |
| -------: | -------------------------------------- | ------------------------------------------------------------------------- |
|   `aaf→` | implicit return without arg(s)         | `async () => █`                                                           |
|  `aafa→` | implicit return with arg(s)            | `async (arg) => █`                                                        |
| `aafad→` | implicit with arg destructuring        | `async ({ prop }) => █`                                                   |
|  `aafe→` | explicit return                        | <code>async () => {<br/>&nbsp;&nbsp;return █<br/> }</code>                |
| `aafea→` | explicit return with arg(s)            | <code>async (arg) => {<br/>&nbsp;&nbsp;return █<br/> }</code>             |
|`aafead→` | explicit return with arg destructuring | <code>async ({prop, prop}) => {<br/>&nbsp;&nbsp;return █<br/> }</code>    |
| `aafee→` | explicit empty                         | <code>async () => {<br/>&nbsp;&nbsp;█<br/> }</code>                       |
|`aafeea→` | explicit empty with arg(s)             | <code>async (arg) => {<br/>&nbsp;&nbsp;█<br/> }</code>                    |
|`aaafea→` | explicit with args and await           | <code>async (arg) => {<br/>&nbsp;&nbsp;const name = await █<br/> }</code> |
| `aafii→` | immediately invoked                    | `(async () => █)()`                                                       |
| `iiaaf→` | immediately invoked                    | `(async () => █)()`                                                       |

### Promises

|  Trigger | Description                         | Result JS/TS                                                                  |
| -------: | ----------------------------------- | ----------------------------------------------------------------------------- |
|  `afpr→` | promise implicit returns            | <code>promise<br/>&nbsp;&nbsp;.then((response) => { })<br/>&nbsp;&nbsp;.catch((error) => { })<br/>&nbsp;&nbsp;.finally(() => { })█<br/> }</code>                  |
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
| `arsna→`  | sort number ascending   | `array.sort((a, z) => a - z)█`                                                           |
| `arsnd→`  | sort number descending  | `array.sort((a, z) => z - a)█`                                                           |
| `aruv→`   | unique values           | `const newArray = array.filter((current, index, arr) => arr.indexOf(current) == index)█` |

### Functions

|  Trigger | Description                                     | Result JS                                                                | Result TS                                                                      |
| -------: | ----------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
|   `edaf→` | export default anonymous arrow function        | <code>export default () => {<br/>&nbsp;&nbsp;█<br/> }</code>             | <code>export default () => {<br/>&nbsp;&nbsp;█<br/> }</code>                   |
|  `edaaf→` | export default async anonymous arrow function  | <code>export default async () => {<br/>&nbsp;&nbsp;█<br/> }</code>       | <code>export default async () => {<br/>&nbsp;&nbsp;█<br/> }</code>             |
|    `caf→` | const arrow function implicit return           | <code>const name = () => █</code>                                        | <code>const name = () => {█</code>                                             |
|   `cafe→` | const arrow function explicit return           | <code>const name = () => {<br/>&nbsp;&nbsp;return █<br/> }</code>        | <code>const name = () => {<br/>&nbsp;&nbsp;return █<br/> }</code>              |
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

## Settings

The `editor.snippetSuggestions` setting in vscode `settings.json` will show snippets on top of the suggestion list.

```json
"editor.snippetSuggestions": "top"
```

⇧ [Back to menu](#menu)

---

## About

### Built With

- [VS Code](https://code.visualstudio.com/) - Code editing redefined.
- [Figma](https://www.figma.com/) - The collaborative interface design tool.

### Contributing

Please read [CONTRIBUTING](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

### Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [Arrow Function Snippets](https://github.com/deinsoftware/vscode-arrow-snippets/tags) on GitHub.

### Authors

- **Camilo Martinez** [[Equiman](http://github.com/equiman)]

See also the list of [contributors](https://github.com/deinsoftware/vscode-arrow-snippets/contributors) who participated in this project.

### Sponsors

If this project helps you, consider buying me a cup of coffee.

[![GitHub Sponsors](https://img.shields.io/badge/-GitHub%20Sponsors-gray?style=flat&labelColor=171515&logo=github&logoColor=white&link=https://github.com/sponsors/deinsoftware)](https://github.com/sponsors/deinsoftware)
[![paypal](https://img.shields.io/badge/-PayPal-gray?style=flat&labelColor=00457C&logo=paypal&logoColor=white&link=https://paypal.me/equiman/3)](https://paypal.me/equiman/3)

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

⇧ [Back to menu](#menu)
