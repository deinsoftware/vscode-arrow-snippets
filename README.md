# Arrow Function Snippets

[![Version](https://vsmarketplacebadge.apphb.com/version/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating/deinsoftware.arrow-function-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=deinsoftware.arrow-function-snippets)

This extension contains code snippets to write [Arrow Functions][mdn] fast and easily.

## Installation

In order to install an extension you need to launch the Command Palette with <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> (Win/Linux) or <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> (macOS) and type `Extensions`.

There you have either the option to show the already installed snippets or install new ones.

## Supported languages (file extensions)

- JavaScript (.js)
- TypeScript (.ts)
- JavaScript React (.jsx)
- TypeScript React (.tsx)

## Snippets

Below is a list of all available snippets and the triggers of each one. The **⇥** means the `TAB` key and `█` means the final cursor position.

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

|  Trigger | Description                         | Result                 |
| -------: | ----------------------------------- | ---------------------- |
|    `af→` | simple without args                 | `() => █`              |
|   `afa→` | simple with arg(s)                  | `(arg) => █`           |
|   `afe→` | explicit return                     | `() => { return █ }`   |
|  `afea→` | explicit return with arg(s)         | `(arg) => { return █ }`|
|   `afp→` | explicit with parentesis            | `() => { (█) }`        |
|  `afpa→` | explicit with parentesis and arg(s) | `(arg) => { (█) }`     |

### Helpers

|  Trigger | Description                         | Result                 |
| -------: | ----------------------------------- | ---------------------- |
| `afceq→` | compare equal       | `(element) => element.prop === value█` |
| `afcne→` | compare not equal   | `(element) => element.prop !== value█` |

[mdn]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions