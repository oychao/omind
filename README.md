# boilerplate-creator

generate common boilerplates

[![Build Status](https://travis-ci.org/oychao/boilerplate-creator.svg?branch=master)](https://travis-ci.org/oychao/boilerplate-creator)

## What and Why

**boilerplate-creator** is a cli tool to generate common JavaScript boilerplates which are very messy to create.

## How to use

### Installation

```bash
$ npm i -g boilerplate-creator
```

### Demo

<p align="center">
    <img src="./docs/install-react.png" width=600 alt="demo">
</p>

#### Basic usage

```bash
$ bpc [options]
```

#### Create a React project

```bash
$ bpc -i helloreact -t react
$ # react in typescript
$ bpc -i helloreactts -t react --ts
```

#### Create a Riact project

```bash
$ bpc -i helloriact -t riact
$ # riact in typescript
$ bpc -i helloriactts -t riact --ts
```

#### Create a Vue project

```bash
$ bpc -i hellovue -t vue
$ # vue in typescript
$ bpc -i hellovuets -t vue --ts
```

#### Create a NPM package or a CLI tool

```bash
$ bpc -i hellonpm -t npm
$ bpc -i hellonpm -t npm --ts
$ bpc -i hellocli -t cli
# cli project in typescript not supported
```

### Custom Template Source

boilerplate-creator basiclly just pull templates from GitHub, which means you can set your own template source as well. Note that only github reposities are supported and all templates must be put into a root fold named 'templates', just like this repository.

```bash
bpc -c https://github.com/your/repository
# say you have a 'my-template' under the 'templates' folder, then just:
bpc -i helloworld -t my-template
```

### Get Help document

There are 8 templates(npm|npm-ts|cli|cli-ts|react|react-ts|vue|vue-ts) are supported for now, please check the help document for more information.

```bash
$ bpc --help
```

## Licence

[![](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-badge-4.png)](http://www.wtfpl.net/)
