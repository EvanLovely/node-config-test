# npm config demo

We've got a config key of `mytest` that's used with `process.env.npm_config_mytest` in `test.js`. Here's the places it could get populated:

1. Run `npm test` - you'll see the variable load from this projects `.npmrc` (would of checked in `~/.npmrc` too)
2. Run `npm_config_mytest='fromENV' npm test` - you'll see it get it from the environmental variable
3. Run `npm test --mytest=fromCLI` - you'll set it get it from the command line flag

# More Info

- [config | npm Documentation](https://docs.npmjs.com/misc/config)
- [npmrc | npm Documentation](https://docs.npmjs.com/files/npmrc)
