# Dynamic Image issues

using pnpm for this one!

this works as expected:
```
pnpm astro dev
```

when you build:
```
pnpm astro dev
```
it wont build

astro ver: 4.10.2

stack:
```
 generating optimized images
[CouldNotTransformImage] Could not transform image `/_astro/stock1.DFGDu3WZ.jpeg`. See the stack trace for more information.
  Hint:
    This is often caused by a corrupted or malformed image. Re-exporting the image from your image editor may fix this issue.
  Error reference:
    https://docs.astro.build/en/reference/errors/could-not-transform-image/
  Stack trace:
    at generateImageInternal (file:/astro-burner-deleteme/callous-chasm/node_modules/.pnpm/astro@4.10.2/node_modules/astro/dist/assets/build/generate.js:131:21)
    at async file:/astro-burner-deleteme/callous-chasm/node_modules/.pnpm/p-queue@8.0.1/node_modules/p-queue/dist/index.js:187:36
  Caused by:
  Could not find Sharp. Please install Sharp (`sharp`) manually into your project or migrate to another image service.
    at loadSharp (file:/astro-burner-deleteme/callous-chasm/dist/chunks/astro/assets-service_DXJYOm0c.mjs:503:11)
    at async generateImageInternal (file:/astro-burner-deleteme/callous-chasm/node_modules/.pnpm/astro@4.10.2/node_modules/astro/dist/assets/build/generate.js:125:26)
    at async file:/astro-burner-deleteme/callous-chasm/node_modules/.pnpm/p-queue@8.0.1/node_modules/p-queue/dist/index.js:187:36
 ELIFECYCLE  Command failed with exit code 1.
```

```sh
npm create astro@latest -- --template basics
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/basics)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/basics)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/basics/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

![just-the-basics](https://github.com/withastro/astro/assets/2244813/a0a5533c-a856-4198-8470-2d67b1d7c554)

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
