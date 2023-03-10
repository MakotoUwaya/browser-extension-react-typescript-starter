Thanks to [sinanbekar/browser-extension-react-typescript-starter](https://github.com/sinanbekar/browser-extension-react-typescript-starter) !

<div align="center">
  <br>
 <img src="https://raw.githubusercontent.com/sinanbekar/browser-extension-react-typescript-starter/main/public/images/extension_128.png" alt="Browser Extension React & TypeScript Starter" width="128">
  <br>
  <h2>
    Browser Extension <br>
    React & TypeScript Starter
    <br>
  </h2>
</div>

<p align="center">A cross-platform (Chrome, Firefox, Edge, Opera, Brave) web browser extension (Manifest V3 and Manifest V2) starter kit with hot reload support, built with React, Typescript, Redux, Vite, ESLint, Prettier, Jest and more! </p>
<hr />

<p align="center">
  <a href="#features">Features</a> ·
  <a href="#quick-start">Quick Start</a> ·
  <a href="#important-notes">Important Notes</a> ·
</p>

## Features

- **Instant HMR** (hot reload)[^1]
- Write once run on any browser
- Global Redux support with persist option. Effortless communication between content, background, popup, options, and more pages.
- Provides a basic content example and popup, options, and welcome pages with all React
- Latest Manifest V3 support
- Manifest V2 support (beta)
- Dynamic manifest.json
- Includes ESLint configured to work with TypeScript and Prettier
- Includes tests with Jest

#### Built with

- React
- TypeScript
- Redux (toolkit and redux-persist)
- Material UI
- Vite
- Jest
- ESLint
- Prettier
- commitlint
- commitizen
- simple-git-hooks (lightweight husky alternative)
- nano-staged

[^1]: While fully supported and stable in most cases, rarely hard reloading is recommended.

## Browser Support

| [![Chrome](https://raw.github.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png)](/) | [![Firefox](https://raw.github.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png)](/) | [![Edge](https://raw.github.com/alrra/browser-logos/master/src/edge/edge_48x48.png)](/) | [![Opera](https://raw.github.com/alrra/browser-logos/master/src/opera/opera_48x48.png)](/) | [![Brave](https://raw.github.com/alrra/browser-logos/master/src/brave/brave_48x48.png)](/) |
| --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| ✔                                                                                             | ✔ (Beta)                                                                                         | ✔                                                                                       | ✔                                                                                          | ✔                                                                                          |

## Quick Start

> **Warning** **Please see [Important Notes](#important-notes) before start using.**

Ensure you have

- [Node.js](https://nodejs.org) v14 or later installed
- [Yarn](https://yarnpkg.com) v1 installed
  - avoid v4

### Use the Template

#### GitHub Template

[Create a repo from this template on GitHub](https://github.com/sinanbekar/browser-extension-react-typescript-starter/generate).

**_or_**

#### Clone to local

If you prefer to do it manually with the cleaner git history

> **Note** If you don't have yarn installed, run: npm install -g yarn

```bash
npx degit sinanbekar/browser-extension-react-typescript-starter my-web-extension
cd my-web-extension
git init
```

Then run the following:

- `yarn install` to install dependencies.
- `yarn dev` to start the development server.
- `yarn build` to build an unpacked extension.

- **Load extension in Chrome (Chromium)**

  - Go to the browser address bar and type `chrome://extensions`
  - Check the `Developer Mode` button to enable it.
  - Click on the `Load Unpacked Extension` button.
  - Select your `dist` folder in the project root.

- **Load extension in Firefox**

  - Go to the browser address bar and type `about://debugger`
  - Click on the `Load Temporary Add-on` button.
  - Select your `dist_firefox` folder in the project root.

### Available Commands

- `yarn clean` to remove dist folder. `dev` and `build` commands call this command.
- `yarn ci:test` to run lint & unit test & type checking in ci environment. `ci:test:lint`, `ci:test:style`, `ci:test:unit` commands also available.
- `yarn format` to fix code with eslint, prettier.
- `yarn lint` to call ESLint, Prettier.
- `yarn test` for testing.

## Important Notes

This starter includes experimental packages and is currently in development. You can see changes in this repo often for now.

Please use with caution.
