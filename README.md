# electron-starter-kit

## A Boilerplate for an Easy Start with TypeScript, React, and Electron

[![React](docs/img/react.png)](https://reactjs.org/)
[![Webpack](docs/img/webpack.png)](https://webpack.js.org/)
[![TypeScript](docs/img/ts.png)](https://www.typescriptlang.org/)
[![Electron](docs/img/electron.png)](https://electronjs.org/)
[![Redux](docs/img/redux.png)](https://redux.js.org/)
[![Jest](docs/img/jest.png)](https://facebook.github.io/jest/)

[Electron](https://electronjs.org/) application boilerplate based on [React](https://reactjs.org/), [Redux](https://redux.js.org/), and [Webpack](https://webpack.js.org/) for rapid application development using [TypeScript](https://www.typescriptlang.org/).

## Install

Clone the repository with Git:

```bash
git clone --depth=1 git@github.com:kendrickw/electron-starter-kit.git <your-project-name>
```

And then install the dependencies:

```bash
cd <your-project-name>
yarn
```

## Usage

Both processes have to be started **simultaneously** in different console tabs:

```bash
yarn run start-renderer-dev
yarn run start-main-dev
```

This will start the application with hot-reload so you can instantly start developing your application.

You can also run do the following to start both in a single process:

```bash
yarn run dev
```

## Packaging

We use [Electron builder](https://www.electron.build/) to build and package the application. By default you can run the following to package for your current platform:

```bash
yarn run dist
```

This will create a installer for your platform in the `releases` folder.

You can make builds for specific platforms (or multiple platforms) by using the options found [here](https://www.electron.build/cli). E.g. building for all platforms (Windows, Mac, Linux):

```bash
# Create distribution for Mac, Windows and Linux
yarn run dist -- -mwl
```

## Prettier

To change the code style, you can change the configuration in `.prettierrc`.

To fix all lint errors run `yarn lint-staged`.

## About this project

This project was set up from scratch but is heavily influenced by the [Electron React Boilerplate project](https://github.com/chentsulin/electron-react-boilerplate) and [React Redux TypeScript guide](https://github.com/piotrwitek/react-redux-typescript-guide).

## License

MIT
