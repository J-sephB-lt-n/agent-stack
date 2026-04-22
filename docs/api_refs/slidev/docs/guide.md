---
url: /guide.md
---

# Getting Started

Slidev (slide + dev, **/slaɪdɪv/**) is a web-based slides maker and presenter. It's designed for developers to focus on writing content in Markdown. With the power of web technologies like Vue, you are able to deliver pixel-perfect designs with interactive demos to your presentation.

::: tip

You can learn more about the rationale behind this project in .

:::

## Create Slides

### Try it Online

Start Slidev right in your browser with StackBlitz: [sli.dev/new](https://sli.dev/new)

### Create Locally

> Requires [Node.js](https://nodejs.org) >= 20.12.0 installed.

Run the following command to create a new Slidev project locally:

::: code-group

```bash [pnpm]
# If you haven't installed pnpm
npm i -g pnpm

pnpm create slidev
```

```bash [npm]
# Not recommended -
# NPM will download the packages each time you create a new project,
# which is slow and takes up a lot of space

npm init slidev@latest
```

```bash [yarn]
yarn create slidev
```

```bash [bun]
bun create slidev
```

```bash [deno]
deno init --npm slidev
```

:::

Follow the prompts to start your slides project. The slides content is in `slides.md`, which initially includes demos of most the Slidev features. For more information about the Markdown syntax, please check .

:::: details Single file usage (not recommended)

If you prefer to have a single Markdown file as your slides, you can install the Slidev CLI globally:

::: code-group

```bash [pnpm]
pnpm i -g @slidev/cli
```

```bash [npm]
npm i -g @slidev/cli
```

```bash [yarn]
yarn global add @slidev/cli
```

```bash [bun]
bun i -g @slidev/cli
```

```bash [deno]
deno i -g npm:@slidev/cli
```

:::

Then, you can create and start a single file slides via:

```bash
slidev slides.md
```

::::

## Basic Commands

Slidev provides a set of commands in its CLI. Here are some common ones:

* `slidev` - Start the dev server. See [the dev command](../builtin/cli#dev).
* `slidev export` - Export the slides to PDF, PPTX, or PNGs. See .
* `slidev build` - Build the slides as a static web application. See .
* `slidev format` - Format the slides. See [the format command](../builtin/cli#format).
* `slidev --help` - Show the help message

To run these commands, you can add them to your `package.json` scripts (which has been done for you if the project was created via `npm init slidev`):

```json [package.json]
{
  "scripts": {
    "dev": "slidev --open",
    "build": "slidev build",
    "export": "slidev export"
  }
}
```

Then, you can simply run `npm run dev`, `npm run build`, and `npm run export`.

For more information about the CLI, please check the [CLI guide](../builtin/cli).

## Setup Your Editor {#editor}

Since Slidev uses Markdown as the source entry, you can use any editor you prefer to create your slides. We also provide tools to help you edit you slides more conveniently:

## Join the Community

It's recommended to join our official [Discord Server](https://chat.sli.dev/) to get help, share your slides, or discuss anything about Slidev.

If you're encountering bugs, feel free to open an issue on [GitHub](https://github.com/slidevjs/slidev/issues/new/choose).

## Tech Stack

Slidev is made possible by combining these tools and technologies.

* [Vite](https://vitejs.dev) - An extremely fast frontend tooling
* [Vue 3](https://v3.vuejs.org/) powered [Markdown](https://daringfireball.net/projects/markdown/syntax) - Focus on the content while having the power of HTML and Vue components whenever needed
* [UnoCSS](https://github.com/unocss/unocss) - On-demand utility-first CSS framework, style your slides at ease
* [Shiki](https://github.com/shikijs/shiki), [Monaco Editor](https://github.com/Microsoft/monaco-editor) - First-class code snippets support with live coding capability
* [RecordRTC](https://recordrtc.org) - Built-in recording and camera view
* [VueUse](https://vueuse.org) family - [`@vueuse/core`](https://github.com/vueuse/vueuse), [`@vueuse/head`](https://github.com/vueuse/head), [`@vueuse/motion`](https://github.com/vueuse/motion), etc.
* [Iconify](https://iconify.design/) - Iconsets collection.
* [Drauu](https://github.com/antfu/drauu) - Drawing and annotations support
* [KaTeX](https://katex.org/) - LaTeX math rendering.
* [Mermaid](https://mermaid-js.github.io/mermaid) - Textual Diagrams.

---

