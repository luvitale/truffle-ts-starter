# TypeChain x Truffle v5 Example

## Running

```sh
# it will automatically run TypeChain types generation
yarn

# Run `yarn generate-types` to manually regenerate them

# run tests
truffle test

# migrations are kinda tricky (look at known limitation section) - we need to transpile ts to js file (this is not a case for tests)
yarn migrate
```

## Known limitations

Migrations need to be transpiled to js before execution. Use `yarn migrate` instead of `truffle migrate` to transpile and migrate with a single command.
