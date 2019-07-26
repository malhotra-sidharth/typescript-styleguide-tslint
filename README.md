## typescript-styleguide-tslint
A light-weight `tslint.json` for clean and strict Typescript code

No need to edit any lint rules or add any new configurations.

## Getting Started
* To install:
```
npm install typescript-styleguide-tslint
```

* In your project `tslint.json` file, add
`"extends": "typescript-styleguide-tslint/tslint.json"`
Your `tslint.json` file should look like
```
{
  "extends": "typescript-styleguide-tslint/tslint.json",
  "linterOptions": {
    // your linter options
  }
}
```

* Add a script to `package.json`
```
 "lint": "tslint --project ."
 "fix": "tslint --fix --project ."
```

* Run `npm run lint` to find lint errors and `npm run fix` to fix linting errors for select rules (this may overwrite linted files).


## Adding your own custom rules
You can always customize or overwrite the provided rules with your own rules in your project's `tslint.json` file
```
{
  "extends": "typescript-styleguide-tslint/tslint.json",
  "linterOptions": {
    // your linter options
  },
  "rules": {
    // your rules go here
  }
}
```

## License
[MIT](https://github.com/sidharth0094/typescript-styleguide-tslint/blob/master/LICENSE)
