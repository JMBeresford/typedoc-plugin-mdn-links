# typedoc-plugin-mdn-links

Adds support for linking references to global types like `HTMLElement`, `WebAssembly`, and `Date` to their documentation pages on MDN.

If you're explicitly referencing a type in a comment, you can use `{@link !HTMLElement}` to have it processed by this plugin.

If you set `--logLevel Verbose`, it will print out when failing to resolve a symbol to a page on MDN. Pull requests to fix failed resolution are welcome!

Supports TypeDoc 0.23.x, 0.24.x and 0.25.x

| Option                  | Default | Description                                                                                |
| ----------------------- | ------- | ------------------------------------------------------------------------------------------ |
| resolveUtilityTypes     | `true`  | Resolve links to `Partial`, `Omit`, etc. to their documentation on the TypeScript website. |
| additionalModuleSources | `false` | Specify additional node_modules to attempt to resolve links to MDN from.                   |

## Changelog

### v3.1.21 (2024-04-21)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.22

### v3.1.20 (2024-04-14)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.21

### v3.1.19 (2024-03-31)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.18

### v3.1.18 (2024-03-10)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.14

### v3.1.17 (2024-02-25)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.11

### v3.1.16 (2024-02-11)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.10

### v3.1.15 (2024-02-04)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.9

### v3.1.14 (2024-01-28)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.8

### v3.1.13 (2024-01-21)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.7

### v3.1.12 (2024-01-14)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.6

### v3.1.11 (2024-01-07)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.4

### v3.1.10 (2023-12-31)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.3

### v3.1.9 (2023-12-24)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.2

### v3.1.8 (2023-12-17)

-   Updated MDN API index with @mdn/browser-compat-data version 5.5.0

### v3.1.7 (2023-12-10)

-   Updated MDN API index with @mdn/browser-compat-data version 5.4.5

### v3.1.6 (2023-12-03)

-   Updated MDN API index with @mdn/browser-compat-data version 5.4.3

### v3.1.5 (2023-11-26)

-   Updated MDN API index with @mdn/browser-compat-data version 5.4.1

### v3.1.4 (2023-11-19)

-   Updated MDN API index

### v3.1.3 (2023-11-18)

-   Fixed broken publish due to missing data folder, #14.

### v3.1.2 (2023-11-18)

-   Updated MDN API index

### v3.1.1 (2023-11-18)

-   Updated MDN API index
-   Fixed links to types defined in `@types/web`, #13

### v3.1.0 (2023-08-25)

-   Added support for TypeDoc 0.25.x.

### v3.0.2 (2023-03-09)

-   Add support for resolving TypeScript utility types (`Partial`, `Omit`, etc.) to links on the TypeScript website.
    This can be turned off with the new `resolveUtilityTypes` option.

### v3.0.2 (2023-03-10)

-   Fixed invalid published package (@WikiRik)

### v3.0.1 (2023-03-09)

-   Add support for `{@link !NaN}` to link to global symbols, #4
-   Fix links to Intl/WebAssembly namespace members
-   In TypeDoc versions 0.23.26 and later will now use the symbol name as the default link test

### v3.0.0 (2023-03-09)

-   Add support for TypeDoc 0.24 (@ocavue)
-   Drop support for TypeDoc 0.22

### v2.0.2 (2022-12-22)

-   Add missing `AsyncGenerator` and `AsyncGeneratorFunction` pages (@achingbrain)

### v2.0.1 (2022-12-16)

-   Add many missing links (@achingbrain)

### v2.0.0 (2022-06-26)

-   Support TypeDoc 0.23
-   Drop support for Node 12

### v1.0.6 (2022-04-09)

-   Added support for WebAudio and Canvas APIs (@johh)

### v1.0.5 (2022-01-26)

-   Fixed repository reference so that npm will link to GitHub (@mikaello)

### v1.0.4 (2021-09-05)

-   Added missing link for base `HTMLElement` interface.

### v1.0.3 (2021-09-05)

-   Added support for HTML element types (`HTMLAnchorElement`, `HTMLButtonElement`, etc.)

### v1.0.2 (2021-09-05)

-   Added `typedocplugin` to keywords so that TypeDoc will now automatically load this plugin if installed.
