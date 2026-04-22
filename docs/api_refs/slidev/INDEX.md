# Slidev Documentation

> Presentation slides for developers

This index covers all Slidev documentation pages, organized by topic.

## Guide

- [Why Slidev](./docs/guide/why.md): Why Slidev was created and how it differs from other presentation tools.
- [Getting Started](./docs/guide.md): Getting started with Slidev: installation, creating your first presentation.
- [Syntax Guide](./docs/guide/syntax.md): Complete guide to Slidev's Markdown syntax, frontmatter, code blocks, and notes.
- [User Interface](./docs/guide/ui.md): Overview of the Slidev user interface, navigation, presenter mode, and toolbar.
- [Animation](./docs/guide/animations.md): Click animations, motion effects, and slide transitions in Slidev.
- [Theme and Addons](./docs/guide/theme-addon.md): How to use, install, and configure themes and addons.
- [Components in Slides](./docs/guide/component.md): How to use and write custom Vue components in your slides.
- [Slide Layout](./docs/guide/layout.md): How to use and write slide layouts in Slidev.
- [Exporting](./docs/guide/exporting.md): Export slides to PDF, PNG images, or a PowerPoint file.
- [Building and Hosting](./docs/guide/hosting.md): Build slides as a SPA and host on GitHub Pages, Netlify, Vercel, or Docker.
- [Work with AI](./docs/guide/work-with-ai.md): How to use AI assistants effectively with Slidev.
- [FAQ](./docs/guide/faq.md): Frequently asked questions and common issues with Slidev.

## Advanced

- [Global Context](./docs/guide/global-context.md): Access and use global reactive context (nav, clicks, theme, etc.) in your slides.
- [Writing Layouts](./docs/guide/write-layout.md): Write custom slide layouts as Vue components.
- [Writing Themes](./docs/guide/write-theme.md): Create and publish Slidev themes with custom styles, layouts, and defaults.
- [Writing Addons](./docs/guide/write-addon.md): Create and publish reusable Slidev addons.

## Customizations

- [Customizations](./docs/custom.md): Overview of all customization options in Slidev, including headmatter and per-slide frontmatter.
- [Directory Structure](./docs/custom/directory-structure.md): Reference for Slidev's project directory structure and special files.
- [Configure Highlighter](./docs/custom/config-highlighter.md): Configure the Shiki syntax highlighter, themes, and TwoSlash support.
- [Configure Vite and Plugins](./docs/custom/config-vite.md): Configure Vite plugins and Slidev's internal Vite plugin options.
- [Configure Vue App](./docs/custom/config-vue.md): Configure the Vue application instance (plugins, directives, etc.).
- [Configure UnoCSS](./docs/custom/config-unocss.md): Extend or override UnoCSS (Tailwind-compatible) configuration for your slides.
- [Configure Code Runners](./docs/custom/config-code-runners.md): Define custom code runners for Monaco Editor to execute code in any language.
- [Configure Transformers](./docs/custom/config-transformers.md): Define custom per-slide markdown and code-block transformers.
- [Configure Monaco](./docs/custom/config-monaco.md): Configure the Monaco editor, TypeScript types, and editor options.
- [Configure KaTeX](./docs/custom/config-katex.md): Configure KaTeX options for LaTeX math rendering.
- [Configure Mermaid](./docs/custom/config-mermaid.md): Configure Mermaid diagram themes, variables, and styles.
- [Configure Mermaid Renderer](./docs/custom/config-mermaid-renderer.md): Plug in a custom third-party Mermaid renderer library.
- [Configure Routes](./docs/custom/config-routes.md): Add custom pages/routes to the Slidev Vue Router app.
- [Configure Shortcuts](./docs/custom/config-shortcuts.md): Customize keyboard shortcuts and navigation key bindings.
- [Configure Context Menu](./docs/custom/config-context-menu.md): Customize or extend the right-click context menu in Slidev.
- [Configure Fonts](./docs/custom/config-fonts.md): Configure custom fonts for your slides, including Google Fonts and local fonts.
- [Configure Pre-Parser](./docs/custom/config-parser.md): Extend Slidev's pre-parser with custom syntaxes for slide transformation.

## Built-in

- [Slidev CLI](./docs/builtin/cli.md): Slidev CLI reference: dev, build, export, pdf, and all command-line options.
- [Components](./docs/builtin/components.md): Reference for all built-in Vue components provided by Slidev (Arrow, Toc, Tweet, Youtube, etc.).
- [Layouts](./docs/builtin/layouts.md): Reference for all built-in slide layouts (cover, center, two-cols, image, etc.).

## Resources

- [Showcases](./docs/resources/showcases.md): Talks and presentations built with Slidev from the community.
- [Theme Gallery](./docs/resources/theme-gallery.md): Browse community-made Slidev themes available on NPM.
- [Addon Gallery](./docs/resources/addon-gallery.md): Browse and discover community-made Slidev addons available on NPM.
- [Learning Resources](./docs/resources/learning.md): Curated tutorials, talks, and articles for learning Slidev.
- [Curated Covers](./docs/resources/covers.md): A curated gallery of cover images for Slidev presentations.

## Other

- [Block Frontmatter](./docs/features/block-frontmatter.md): Use a YAML code block as the frontmatter.
- [Bundle Remote Assets](./docs/features/bundle-remote-assets.md): Download and bundle remote assets when building your slides.
- [Click Markers](./docs/features/click-marker.md): Highlighting notes and auto-scrolling to the active section of notes.
- [Code Groups](./docs/features/code-groups.md): Group multiple code blocks and automatically match icon by the title name.
- [Comark Syntax](./docs/features/comark.md): A powerful syntax to enhance your markdown content with components and styles.
- [Draggable Elements](./docs/features/draggable.md): Move, resize, and rotate elements by dragging them with the mouse.
- [Drawing & Annotations](./docs/features/drawing.md): Draw and annotate your slides with ease.
- [Eject Theme](./docs/features/eject-theme.md): Eject the installed theme from your project to customize it.
- [Features](./docs/features.md): Index of all Slidev features with brief descriptions.
- [Frontmatter Merging](./docs/features/frontmatter-merging.md): Merge frontmatter from multiple markdown files.
- [Generate PDF when Building](./docs/features/build-with-pdf.md): Generate a downloadable PDF along with your slides build.
- [Global Layers](./docs/features/global-layers.md): Create custom components that persist across slides.
- [Icons](./docs/features/icons.md): Use icons from virtually all open-source icon sets directly in your markdown.
- [Import Code Snippets](./docs/features/import-snippet.md): Import code snippets from existing files into your slides.
- [Importing Slides](./docs/features/importing-slides.md): Split your `slides.md` into multiple files for better reusability and organization.
- [Integrated Editor](./docs/features/side-editor.md): Edit your slides source file alongside the presentation.
- [LaTeX](./docs/features/latex.md): Slidev comes with LaTeX support out-of-box, powered by KaTeX.
- [Line Highlighting](./docs/features/line-highlighting.md): Highlight specific lines in code blocks based on clicks.
- [Line Numbers](./docs/features/code-block-line-numbers.md): Enable line numbering for all code blocks across the slides or individually.
- [Max Height](./docs/features/code-block-max-height.md): Set a maximum height for a code block and enable scrolling.
- [Mermaid Diagrams](./docs/features/mermaid.md): Create diagrams/graphs from textual descriptions, powered by Mermaid.
- [Monaco Editor](./docs/features/monaco-editor.md): Turn code blocks into fully-featured editors, or generate a diff between two code blocks.
- [Monaco Runner](./docs/features/monaco-run.md): Run code directly in the editor and see the result.
- [Navigation Direction Variants](./docs/features/direction-variant.md): Apply different styles and animations based on the navigation direction.
- [Notes Auto Ruby](./docs/features/notes-auto-ruby.md): Automatically add `<ruby>` tags to your notes.
- [Open Graph Image](./docs/features/og-image.md): Set the Open Graph image for your slides.
- [PlantUML Diagrams](./docs/features/plantuml.md): Create diagrams from textual descriptions, powered by PlantUML.
- [Presenter Timer](./docs/features/timer.md): Timer for the presenter mode.
- [Prettier Plugin](./docs/features/prettier-plugin.md): Use the Prettier plugin to format your slides.
- [Recording](./docs/features/recording.md): Record your presentation with the built-in camera view and recording feature.
- [Remote Access](./docs/features/remote-access.md): Access your presentation remotely with Slidev's remote access feature.
- [Rough Markers](./docs/features/rough-marker.md): Integrate Rough Notation to allow marking or highlighting elements in your slides.
- [SEO Meta Tags](./docs/features/seo-meta.md): Configure SEO meta tags for better social media sharing and search engine optimization.
- [Shiki Magic Move](./docs/features/shiki-magic-move.md): Enable granular transition between code changes, similar to Keynote's Magic Move.
- [Slide Canvas Size](./docs/features/canvas-size.md): Set the size for all your slides.
- [Slide Hooks](./docs/features/slide-hook.md): Hooks to manage the slide lifecycle.
- [Slide Scope Styles](./docs/features/slide-scope-style.md): Define styles for only the current slide.
- [Slot Sugar for Layouts](./docs/features/slot-sugar.md): A syntax sugar for named slots in layouts.
- [The `Transform` Component](./docs/features/transform-component.md): A component for scaling some elements.
- [TwoSlash Integration](./docs/features/twoslash.md): A powerful tool for rendering TypeScript code blocks with type information on hover or inlined.
- [VS Code Extension](./docs/features/vscode-extension.md): Help you better organize your slides and have a quick overview of them.
- [Writable Monaco Editor](./docs/features/monaco-write.md): A monaco editor that allows you to write code directly in the slides and save the changes back to the file.
- [Zoom Slides](./docs/features/zoom-slide.md): Zoom the content of a slide to a specific scale.
