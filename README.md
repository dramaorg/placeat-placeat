# @dramaorg/placeat-placeat

a simple opinionated node.js CLI utility to setup a new node.js library project including typescript, vitest, prettier and basic github action for checking each commit to `main`.

It will be setup for both ESM and CommonJS consumption and build process using tsup no config.

## Usage

```
npm i @dramaorg/placeat-placeat -g
```
alternatively just prepend with `bunx`
go to a folder where you want your project folder created:

```
@dramaorg/placeat-placeat my-awesome-project
```

alternatively if your project folder already exists and you're in it:

```
@dramaorg/placeat-placeat .
```

folder my-awesome-project in current working directory

## What this does

- create the directory(when you pass something else than ".")
- git init
- adds `.gitignore` same as github does when you init node.js project
- `pnpm init`
- replace `ISC` with `MIT`
- setup typescript in strict mode
- setup vitest
- setup a build command using tsup
- add `.nvmrc` based on the latest node.js version
- setup github action with typescript check and test run
- setup prettier with githooks using husky(TODO)

![picture 2](images/81cad71ba5a5540897330738991351104d3bd46af5d77b3d393279f61153a82d.png)

No version is hardcoded, so you should be getting the latest stuff every time you run `@dramaorg/placeat-placeat` command.

## Prerequisites

`pnpm`
