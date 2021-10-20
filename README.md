# Arrow Function Snippets

[![Version](https://vsmarketplacebadge.apphb.com/version/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![license](https://img.shields.io/github/license/deinsoftware/vscode-arrow-snippets)](LICENSE.md)

![Arrow](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/social/preview.png 'Arrow Function Snippets')

The quick and easy way to create and use [Arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) with [VS Code](https://code.visualstudio.com/).

## Installation

Open the Extension manager with <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>X</kbd> (Win/Linux) or <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>X</kbd> (macOS), search for `deinsoftware.arrow-function-snippets` and click on [Install] button.

Or using the Visual Studio Marketplace: [Arrow Function Snippets](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)

## Supported languages (file extensions)

- JavaScript (.js)
- TypeScript (.ts)
- JavaScript React (.jsx)
- TypeScript React (.tsx)
- Vue (.vue)

---

## Snippets

Below is a list of all available snippets and the triggers of each one. The **→** means the `TAB` key and `█` means the final cursor position.

### Variables

|  Trigger | Description             | Result                   |
| -------: | ----------------------- | ------------------------ |
|    `lv→` | let variable            | `let name = █`           |
|    `ls→` | let string variable     | `let stringName = '█'`   |
|    `lo→` | let object variable     | `let objectName = {█}`   |
|    `la→` | let array variable      | `let arrayName = [█]`    |
|    `cv→` | const variable          | `const name = █`         |
|    `cs→` | const string variable   | `const stringName = '█'` |
|    `co→` | const object variable   | `const objectName = {█}` |
|    `ca→` | const array variable    | `const arrayName = [█]`  |

### Arrow Function

|  Trigger | Description                         | Result                      |
| -------: | ----------------------------------- | --------------------------- |
|    `af→` | implicit return without args        | `() => █`                   |
|   `afa→` | implicit return with arg(s)         | `(arg) => █`                |
|   `afo→` | implicit return object              | `() => ({prop: value█})`    |
|  `afoa→` | implicit return object with arg(s)  | `(arg) => ({prop: value█})` |
|   `afe→` | explicit return                     | <code>() => {<br>&nbsp;&nbsp;return █<br> }</code>        |
|  `afea→` | explicit return with arg(s)         | <code>(arg) => {<br>&nbsp;&nbsp;return █<br> }</code>     |
|   `afp→` | explicit with parentesis            | <code>() => {<br>&nbsp;&nbsp;(█)<br> }</code>             |
|  `afpa→` | explicit with parentesis and arg(s) | <code>(arg) => {<br>&nbsp;&nbsp;(█)<br> }</code>          |
|  `iiaf→` | immediately invoque                 | `(() => █)()`               |

### Promises

|  Trigger | Description                         | Result                           |
| -------: | ----------------------------------- | -------------------------------- |
|   `afr→` | implicit return response            | `(response) => █`                |
|  `afrj→` | implicit return response json       | `(response) => response.json()█` |
|  `afrd→` | implicit return response data       | `(response) => response.data█`   |
|  `afer→` | explicit return response            | <code>(response) => {<br>&nbsp;&nbsp;return █<br> }</code> |
| `aferj→` | explicit return response json       | <code>(response) => {<br>&nbsp;&nbsp;return response.json()<br> }█</code> |
| `aferd→` | explicit return response data       | <code>(response) => {<br>&nbsp;&nbsp;return response.data<br> }█</code> |

### Helpers

|  Trigger | Description                         | Result                 |
| -------: | ----------------------------------- | ---------------------- |
| `afceq→` | compare equal       | `(element) => element.prop === value█` |
| `afcne→` | compare not equal   | `(element) => element.prop !== value█` |

---

## Examples

Create a named arrow function combining `cv` and `af`

![Function](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-function.gif 'Function')

Create a compare equal arrow function inside `.filter()` function with `afceq`

![Filter](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-filter.gif 'Filter')

Create a response for `fetch` promise with `afrj` and `afrd`

![Filter](https://raw.githubusercontent.com/deinsoftware/vscode-arrow-snippets/main/.github/examples/example-promise.gif 'Promise')

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
