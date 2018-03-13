Web Component Tester coverage Reporter
===================================

Generate junit reports from web-component-tester so the results can be parsed by Jenkins.

## Installation

```sh
npm install wct-coverage-reporter --saveDev
```

## Basic Usage

Add the following configuration to web-component-tester's config file.

## Example

```js
module.exports = {
  plugins: {
    coverage-reporter: {
      output: {
        path: 'target/',
        name: 'test.xml'
      }
    }
  }
}
```

## Options

Below are the available configuration options:


    `appendMode` - if set to true then test results are appended to existing file.
    `output.path` - defaults to cwd of the wct
    `output.name` - defaults to test-report
