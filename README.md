<div align="center">
    <h1>Scrivano</h1>
    <p>A meta-build system to keep your project in sync.</p>
  <a href="https://github.com/paysonwallach/scrivano/releases/latest">
    <img alt="Version 0.1.0" src="https://img.shields.io/badge/version-0.1.0-red.svg?cacheSeconds=2592000&style=flat-square" />
  </a>

  <a href="https://github.com/paysonwallach/scrivano/blob/master/LICENSE" target="\_blank">
    <img alt="Licensed under the GNU General Public License v3.0" src="https://img.shields.io/github/license/paysonwallach/scrivano?style=flat-square" />
  </a>

  <a href="https://buymeacoffee.com/paysonwallach">
    <img src="https://img.shields.io/badge/donate-Buy%20me%20a%20coffe-yellow?style=flat-square">
  </a>
  <br>
  <br>
</div>

[Scrivano](https://github.com/paysonwallach/scrivano) is a meta-build system designed to keep every part of your project in sync, from README to documentation to build configurations.

## Installation

Using [`npm`](https://npmjs.com):

```sh
npm install --save-dev scrivano
```

## Usage

Create template files in a `meta` directory at the root of your project, with corresponding variables under a "meta" object in `package.json`:

```json
{
  "meta": {
    "foo": "bar"
  }
}
```

You can use a precommit hook in a package like [`standard-version`](https://github.com/conventional-changelog/standard-version) to automatically compile templated files at release.

```json
{
  "standard-version": {
    "scripts": {
      "precommit": "draft"
    }
  }
}
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

[Scrivano](https://github.com/paysonwallach/scrivano) is licensed under the [GNU General Public License v3.0](https://github.com/paysonwallach/scrivano/blob/master/LICENSE).
