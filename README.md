# About

This is a svelte slide. In order to use it, clone this project and start adding the slides inside `src\lib\deck\presentation.svelte`.

## Avaliable components

- Slide, this component allow you to use html tags with css styles.
- [Markdown](https://revealjs.com/markdown/), the simplest way. you add directly in the component or using external markdown file inside the `static` folder:
    - directly exemple:
    ```html
        <Markdown>
            {`
                ## Hello from markdown
            `}
        </Markdown>
    ```
    - separeted file:
    ```html
        <Markdown name="exemple.md" external />
    ```
- [Code](https://revealjs.com/code/), allow to add a new slide as a piece of code.
- [Notes](https://revealjs.com/speaker-view/), allow you to add adtional notes for the presenter. Press 'S' to open speaker view.


# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/main/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
