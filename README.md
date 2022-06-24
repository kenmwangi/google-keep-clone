# Google Keep Clone - notes app

## Getting Started

First, configure development and build processes
Make two files in root directory
```bash
.nvmrc
# or
.npmrc
```
Engine Locking - allows using same Node engine package manager even in future updates.
In .nvmrc
```bash
lts/gallium

```
In .npmrc
```bash
engine-strict=true

```
NB: `lts/gallium` - represents node 16.x



## ESLint

`.eslintrc.json`
The content of the file should be 

```bash 

{
  "extends": ["next", "next/core-web-vitals", "eslint:recommended"],
  "globals": {
    "React": "readonly"
  },
  "rules": {
    "no-unused-vars": [1, { "args": "after-used", "argsIgnorePattern": "^_" }]
  }
}
```
Testing the config involves running:

`npm run lint` or if using yarn `yarn lint`

## Prettier

For Automatic formatting of our files

Adding two files `.prettierrc` and `.prettierignore` in root project
