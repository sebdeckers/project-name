# project-name [![NPM version](https://badge.fury.io/js/project-name.svg)](http://badge.fury.io/js/project-name)  [![Build Status](https://travis-ci.org/jonschlinkert/project-name.svg)](https://travis-ci.org/jonschlinkert/project-name)

> Get the name of a project, from package.json, git config, or basename of the current working directory.

## Install

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i project-name --save
```

## Usage

The project name is resolved in this order:

1. check for package.json, if exists `name` is returned
2. check for git repository, if exists return repository `name`
3. use the `path.basename` of the current working directory

```js
var name = require('project-name');
name();
//=> project-name
```

Optionally specify a current working directory:

```js
var name = require('project-name');
name('foo');
```

## Related projects

* [git-repo-name](https://www.npmjs.com/package/git-repo-name): Get the repository name from the git remote origin URL. | [homepage](https://github.com/jonschlinkert/git-repo-name)
* [git-user-email](https://www.npmjs.com/package/git-user-email): Get the email address of the current user from git config. | [homepage](https://github.com/jonschlinkert/git-user-email)
* [git-user-name](https://www.npmjs.com/package/git-user-name): Get a user's name from git config at the project or global scope, depending on… [more](https://www.npmjs.com/package/git-user-name) | [homepage](https://github.com/jonschlinkert/git-user-name)
* [git-username](https://www.npmjs.com/package/git-username): Get the username from a git remote origin URL. | [homepage](https://github.com/jonschlinkert/git-username)

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/project-name/issues/new).

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on November 27, 2015._