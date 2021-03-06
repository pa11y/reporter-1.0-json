
# Pa11y JSON 1.0 Reporter [Deprecated]

A reporter for [Pa11y][pa11y] 2.0+ which outputs 1.0-style JSON.

[![NPM version][shield-npm]][info-npm]
[![Node.js version support][shield-node]][info-node]
[![Build status][shield-build]][info-build]
[![Dependencies][shield-dependencies]][info-dependencies]
[![GPLv3 licensed][shield-license]][info-license]

```sh
pa11y --reporter 1.0-json nature.com
```

:skull: **Please note: this reporter is now deprecated and will no longer be supported by the Pa11y team.** :skull: 

Refer to the [Pa11y Migration Guide][pa11y-migration] to update any applications that still expect Pa11y 1.0 JSON format. Alternatively, you're welcome to published your own reporter using [modern Pa11y's reporters interface][pa11y-reporters].


Usage
-----

Install Pa11y and Pa11y JSON 1.0 Reporter with [npm][npm]:

```
npm install -g pa11y
npm install -g pa11y-reporter-1.0-json
```

Use the reporter with the `--reporter` flag:

```sh
pa11y --reporter 1.0-json nature.com
```

You'll get the 1.0-style JSON:

```js
{
    "isPerfect": Boolean,
    "count": {
        "total": Number,
        "error": Number,
        "warning": Number,
        "notice": Number
    },
    "results": Array
}
```


Contributing
------------

To contribute to Pa11y JSON 1.0 Reporter, clone this repo locally and commit your code on a separate branch.

Please check that everything works by running the following before opening a pull-request:

```sh
make ci
```


License
-------

Pa11y JSON 1.0 Reporter is licensed under the [Lesser General Public License (LGPL-3.0)][info-license].<br/>
Copyright &copy; 2015–2017, Team Pa11y


[npm]: https://www.npmjs.com/
[pa11y]: https://github.com/pa11y/pa11y
[pa11y-migration]: https://github.com/pa11y/pa11y/blob/master/MIGRATION.md
[pa11y-reporters]: https://github.com/pa11y/pa11y#reporters

[info-dependencies]: https://gemnasium.com/pa11y/pa11y-reporter-1.0-json
[info-license]: LICENSE
[info-node]: package.json
[info-npm]: https://www.npmjs.com/package/pa11y-reporter-1.0-json
[info-build]: https://travis-ci.org/pa11y/pa11y-reporter-1.0-json
[shield-dependencies]: https://img.shields.io/gemnasium/pa11y/pa11y-reporter-1.0-json.svg
[shield-license]: https://img.shields.io/badge/license-LGPL%203.0-blue.svg
[shield-node]: https://img.shields.io/node/v/pa11y-reporter-1.0-json.svg?label=node.js%20support
[shield-npm]: https://img.shields.io/npm/v/pa11y-reporter-1.0-json.svg
[shield-build]: https://img.shields.io/travis/pa11y/pa11y-reporter-1.0-json/master.svg
