# is-equal [<img src="https://avatars.githubusercontent.com/u/52989093" alt="" width="90" height="90" align="right">][frontend]

[<img alt="npm version" src="https://img.shields.io/npm/v/@jsxtools/is-equal.svg" height="20">](https://www.npmjs.com/package/@jsxtools/is-equal)
[<img alt="build status" src="https://img.shields.io/travis/jsxtools/frontend/master.svg" height="20">](https://travis-ci.org/github/jsxtools/frontend)
[<img alt="issue tracker" src="https://img.shields.io/github/issues/jsxtools/frontend/is-equal.svg" height="20">](https://github.com/jsxtools/frontend/issues?q=is:issue+is:open+label:is-equal)
[<img alt="pull requests" src="https://img.shields.io/github/issues-pr/jsxtools/frontend/is-equal.svg" height="20">](https://github.com/jsxtools/frontend/pulls?q=is:pr+is:open+label:is-equal)

**is-equal** returns whether two values are the same value.

It is <strong size>288 bytes (197 gzipped)</strong>.

## Installation

```sh
npm install @jsxtools/is-equal
```

## Usage

```js
import isEqual from '@jsxtools/is-equal';

// these objects are shallow equal
objectA = { name: 'Adam', age: 930 };
objectB = { name: 'Adam', age: 930 };
isEqual(objectA, objectB);

// these objects are not shallow equal
objectA = { name: 'Adam', age: 930, pets: ['dog'] };
objectB = { name: 'Adam', age: 930, pets: ['dog'] };
isEqual(objectA, objectB);

// but they are deeply equal
isEqual(objectA, objectB, isEqual);
```

[frontend]: https://github.com/jsxtools/frontend
