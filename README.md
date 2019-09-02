# TS Infer Import 

## TypeScript 3.1

```sh
node node_modules/typescript-3.1/lib/tsc.js -p example
```

Succeeds.

## TypeScript 3.4

```sh
node node_modules/typescript-3.4/lib/tsc.js -p example
```

Errors.

```
example/example.ts:3:14 - error TS2742: The inferred type of 'example' cannot be named without a reference to '../external/node_modules/example-lib'. This is likely not portable. A type annotation is necessary.

3 export const example = exampleLib();
               ~~~~~~~
```
