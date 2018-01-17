# vscode-graphql
Syntax highlighting, diagnostics, autocomplete, and go to definition for `.graphql` files.

## Features
- Syntax highlighting
- Autocomplete
- Go to definition
- Error diagnostics

Autocomplete, go to definition, and diagnostics are language server features supported by the [graphql-language-service](https://github.com/graphql/graphql-language-service/).

## Installation
1. Install [stpn.vscode-graphql](https://marketplace.visualstudio.com/items?itemName=stpn.vscode-graphql) from the marketplace
2. Install [watchman](https://facebook.github.io/watchman/docs/install.html), if using language service features (see below).

Watchman is currently a dependency of `graphql-language-service`. See [issue #8](https://github.com/stephen/vscode-graphql/issues/8).

## Configuration
To turn on language server features, you can enable the `graphql.useLanguageServer` flag in your settings.

Using the language server will require a schema to be specified via a `.graphqlconfig` file.

Example:
```json
{
  "schemaPath": "./schema.json"
}
```

See [here](https://github.com/graphcool/graphql-config#usage) for other ways to provide a GraphQL schema.
