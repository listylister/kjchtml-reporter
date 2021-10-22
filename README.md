# karma-jasmine-cards-html-reporter

[![npm version](https://img.shields.io/npm/v/karma-jasmine-html-cards-reporter.svg)](https://www.npmjs.com/package/karma-jasmine-html-cards-reporter) [![npm downloads](https://img.shields.io/npm/dm/karma-jasmine-html-cards-reporter.svg)](https://www.npmjs.com/package/karma-jasmine-html-cards-reporter)

Reporter that dynamically shows tests results at debug.html page.

Jasmine 1.3 is not supported. For Jasmine < 3.0.0, use version 0.2.2

![alt tag](/screenshots/reporter_3.png)

You can also run a describe block, or a single test.

![alt tag](/screenshots/reporter_4.png)

## Installation

You can simply install `karma-jasmine-html-cards-reporter` as a devDependency by:

```bash
npm install karma-jasmine-html-cards-reporter --save-dev
```

## Configuration

```js
// karma.conf.js

plugins: [
    require('karma-jasmine-html-cards-reporter'),
]

module.exports = function (config) {
	config.set({
		reporters: ["kjchtml"],
	});
};
```

You can pass a list of reporters as a CLI argument too:

```bash
karma start --reporters kjchtml
```
