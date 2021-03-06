# tauri

This project use [tauri](https://github.com/tauri-apps/tauri), a web browser for bundling with applications, like electron.

You need to install the CLI for tauri to use build your app.

```
yarn global add @tauri-apps/cli@^1.0.0 # install wrapper from npm, then download from tauri server

# or you can compile the CLI from source
git clone https://github.com/tauri-apps/tauri
cd tauri/tooling/cli.rs
cargo install --path . # install cargo-tauri
```

# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte);

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm init svelte@next

# create a new project in my-app
npm init svelte@next my-app
```

> Note: the `@next` is temporary

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# Then, after you installed Tauri's CLI, run this to open your application:
cargo tauri dev

# if you installed tauri from npm package `@tauri-apps/cli, run this instead:
yarn tauri dev
```

## Building

Before creating a production version of your app, install an [adapter](https://kit.svelte.dev/docs#adapters) for your target environment. Then:

```bash
npm run build
```

> You can preview the built app with `npm run preview`, regardless of whether you installed an adapter. This should _not_ be used to serve your app in production.
