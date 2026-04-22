---
url: /guide/ui.md
---

# User Interface

## Navigation Bar {#navigation-bar}

In Play mode, move your mouse to the bottom left corner of the page, you can see the navigation bar.
![](/screenshots/navbar.png)

> You can extend the navigation bar via .

## Navigation Actions {#navigation-actions}

| Keyboard Shortcut                   | Button in Navigation Bar                                                              | Description                                                     |
| ----------------------------------- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| f                        |   | Toggle fullscreen                                               |
| right / space |                                          | Next animation or slide                                         |
| left                     |                                           | Previous animation or slide                                     |
| up                       | -                                                                                     | Previous slide                                                  |
| down                     | -                                                                                     | Next slide                                                      |
| o                        |                                                 | Toggle [Quick Overview](#quick-overview)                        |
| d                        |            | Toggle dark mode                                                |
| -                                   |                                          | Toggle [Camera View](../features/recording#camera-view)         |
| -                                   |                                                | Start                   |
| -                                   |                                         | Enter [Presenter Mode](#presenter-mode)                         |
| -                                   |                               | Toggle                |
| -                                   |                                         | Enter [Browser Exporter](#exporter)                             |
| -                                   |                                             | Download PDF. See  |
| -                                   |                                          | Show information about the slides                               |
| -                                   |                                      | More options                                                    |
| g                        | -                                                                                     | Show goto...                                                    |

> You can [configure the shortcuts](../custom/config-shortcuts).

## Quick Overview {#quick-overview}

By pressing o or clicking the  button in the navigation bar, you can have an overview of your slides so you can jump between them easily.

![](/screenshots/slides-overview.png)

## Presenter Mode {#presenter-mode}

To enter the presenter mode, you can click the  button in the navigation panel, or visit `http://localhost:<port>/presenter`.

When giving a presentation, it's recommended to open two browser windows - one in the play mode for the audience, and another one in the presenter mode for you. Then you can share the first screen to the audience and keep the second screen for yourself.

Whenever you navigate through the slides in the presenter mode, all other opened pages will automatically follow this navigation to stay in sync with the presenter.

![](/screenshots/presenter-mode.png)

### Presenter Layouts {#presenter-layouts}

> Available since v0.50.0

The presenter view offers three different layouts that you can cycle through by clicking the layout toggle button  in the navigation bar:

* **Layout 1** (default): Current slide prominently displayed at the top, with notes and next slide preview below
* **Layout 2**: Notes panel on the left, current slide and next slide stacked on the right
* **Layout 3**: Notes and current slide on the left, larger next slide preview on the right

Each layout is optimized for different screen sizes and presentation preferences.

### Screen Mirror {#screen-mirror}

> Available since v0.50.0

In the presenter view, you can switch the main slide area to "Screen Mirror" mode. This allows you to capture and display another monitor or window directly in the presenter view.

Click the "Screen Mirror" option in the presenter view's segment control, then select the screen or window you want to mirror. This is useful when you want to see exactly what your audience sees on the projector or external display (e.g. live coding / live demo).

## Slide Overview {#slides-overview}

> Available since v0.48.0

You can visit an overview of all of your slides by first opening the [Quick Overview panel](#quick-overview) and then clicking the  on the top right, or by visiting `http://localhost:<port>/overview` directly.

The overview page gives you a linear list of all your slides, with all of your notes on the side. You can double-click on the notes to edit the notes directly, and drag the clicks sliders to preview the steps in your slides.

## Notes Editor {#notes-editor}

> Available since v0.52.0

Slidev provides a batch notes editor at `http://localhost:<port>/notes-edit` where you can edit notes for all slides in a single text area.

Notes for each slide are separated by `--- #[slide-number]` markers. Changes are automatically saved as you type with debouncing.

This is useful when you want to write or review all your speaker notes in one place without switching between slides.

## Drawing UI {#drawing}

See:

## Recording UI {#recording}

See:

## Browser Exporter {#exporter}

See:

## Settings {#settings}

Click the  button in the navigation bar to access additional settings.

### CSS Filters {#css-filters}

> Available since v0.50.0

When presenting on different projectors or displays, colors may appear differently than expected. Slidev provides CSS filter controls to adjust the display in real-time:

* **Invert**: Flip all colors
* **Brightness**: Adjust overall brightness (0.5 - 1.5)
* **Contrast**: Adjust contrast levels (0.5 - 1.5)
* **Saturation**: Adjust color saturation (0.5 - 1.5)
* **Sepia**: Add sepia tone effect
* **Hue Rotate**: Shift all colors by degrees (-180 to 180)

These settings are stored locally and persist across sessions. A dot indicator appears on the settings button when any filter is active.

### Hide Idle Cursor {#hide-idle-cursor}

> Available since v0.50.0

When enabled, the cursor will automatically hide after a period of inactivity during the presentation. This provides a cleaner viewing experience for your audience.

### Slide Scale {#slide-scale}

Choose between "Fit" mode (scales slides to fit the viewport) or "1:1" mode (displays slides at their native resolution).

### Wake Lock {#wake-lock}

When enabled, prevents the screen from dimming or locking during your presentation. Requires browser support for the Wake Lock API.

## Global Layers {#global-layers}

You can add any custom UI below or above your slides for the whole presentation or per-slide:

---

