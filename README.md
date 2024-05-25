# @zitterorg/maxime-dolor <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

For use with React PropTypes. Will error on any prop not explicitly specified.

## Usage

```jsx
import PropTypes from 'prop-types';
import exact from '@zitterorg/maxime-dolor';

function Foo({ foo, bar }) {
  return <div>{foo}{bar}</div>
}
Foo.propTypes = exact({
  foo: PropTypes.string,
  bar: PropTypes.number,
});

<Foo foo="hi" bar={3} /> // no warnings

<Foo foo="hi" bar={3} baz="extra" /> // propTypes warning!
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@zitterorg/maxime-dolor
[npm-version-svg]: http://versionbadg.es/ljharb/@zitterorg/maxime-dolor.svg
[deps-svg]: https://david-dm.org/ljharb/@zitterorg/maxime-dolor.svg
[deps-url]: https://david-dm.org/ljharb/@zitterorg/maxime-dolor
[dev-deps-svg]: https://david-dm.org/ljharb/@zitterorg/maxime-dolor/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@zitterorg/maxime-dolor#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@zitterorg/maxime-dolor.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@zitterorg/maxime-dolor.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@zitterorg/maxime-dolor.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@zitterorg/maxime-dolor
[codecov-image]: https://codecov.io/gh/ljharb/@zitterorg/maxime-dolor/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@zitterorg/maxime-dolor/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@zitterorg/maxime-dolor
[actions-url]: https://github.com/zitterorg/maxime-dolor/actions
