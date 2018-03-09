# git-branch [![NPM version](https://img.shields.io/npm/v/git-branch.svg?style=flat)](https://www.npmjs.com/package/git-branch) [![NPM monthly downloads](https://img.shields.io/npm/dm/git-branch.svg?style=flat)](https://npmjs.org/package/git-branch) [![NPM total downloads](https://img.shields.io/npm/dt/git-branch.svg?style=flat)](https://npmjs.org/package/git-branch) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/git-branch.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/git-branch)

> Get the current branch from the local git repository.

Please consider following this project's author, [Jon Schlinkert](https://github.com/jonschlinkert), and consider starring the project to show your :heart: and support.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save git-branch
```

## Usage

```js
const branch = require('git-branch');
```

Optionally pass the cwd (current working directory) as the first argument.

**Promise**

```js
branch('some/path')
  .then(name => console.log('Branch:', name)) //=> 'master'
  .catch(console.error);
```

**Callback**

```js
branch(function(err, name) {
  if (err) throw err;
  console.log('Branch:', name); //=> 'master'
});
```

**Sync**

```js
console.log('Branch:', branch.sync()); //=> 'master'
```

## About

<details>
<summary><strong>Contributing</strong></summary>

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

</details>

<details>
<summary><strong>Running Tests</strong></summary>

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

</details>

<details>
<summary><strong>Building docs</strong></summary>

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

</details>

### Related projects

You might also be interested in these projects:

* [git-add-remote](https://www.npmjs.com/package/git-add-remote): API for adding git remotes. | [homepage](https://github.com/jonschlinkert/git-add-remote "API for adding git remotes.")
* [git-user-name](https://www.npmjs.com/package/git-user-name): Get a user's name from git config at the project or global scope, depending on… [more](https://github.com/jonschlinkert/git-user-name) | [homepage](https://github.com/jonschlinkert/git-user-name "Get a user's name from git config at the project or global scope, depending on what git uses in the current context.")
* [github-base](https://www.npmjs.com/package/github-base): JavaScript wrapper that greatly simplifies working with GitHub's API. | [homepage](https://github.com/jonschlinkert/github-base "JavaScript wrapper that greatly simplifies working with GitHub's API.")

### Contributors

| **Commits** | **Contributor** | 
| --- | --- |
| 19 | [jonschlinkert](https://github.com/jonschlinkert) |
| 6 | [emilrowland](https://github.com/emilrowland) |

### Author

**Jon Schlinkert**

* [LinkedIn Profile](https://linkedin.com/in/jonschlinkert)
* [GitHub Profile](https://github.com/jonschlinkert)
* [Twitter Profile](https://twitter.com/jonschlinkert)

### License

Copyright © 2018, [Jon Schlinkert](http://github.com/https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.6.0, on March 09, 2018._