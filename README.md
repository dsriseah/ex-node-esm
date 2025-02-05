This is a minimal nodejs example using ES modules, importing local package `sri-lib`. It was tested using Node 18.18.2 on Macos Sequoia (ARM).

## Running

```
npm ci       # just once (copies packages listed in package-lock.json to node_modules)
npm start    # script just executes 'node @runme.mjs'
```

## Structure

* The `@runme.mjs` file imports the function `SriIsACat` from the `sri-ml` package, which is added as a file dependency in the root `package.json`.
* The `sri-lib` directory has its own `package.json` that declares it as type `module` and provides an `exports` field for the entryfile of the library.


