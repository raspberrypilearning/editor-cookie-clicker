# Pizza party project structure

This directory contains the English Raspberry Pi Code Editor version of **Pizza party**, a Scratch pizza-clicker game for the Code Club arcade.

```plaintext
en/
├── code/
│   ├── editor-cookie-clicker-complete/
│   │   ├── editor-cookie-clicker-complete.sb3
│   │   └── project_config.yml
│   └── editor-cookie-clicker-starter/
│       ├── editor-cookie-clicker-starter.sb3
│       └── project_config.yml
├── images/
│   ├── banner.png
│   └── tutorial images and animations
├── resources/
│   └── pizza-party.pdf
├── solutions/
│   └── Pizza Party _ Endless Clicker.sb3
├── landing.md
├── meta.yml
├── step_1.md
├── ...
└── step_30.md
```

## `code/`

The two subdirectories contain Scratch 3 (`.sb3`) projects and their Code Editor configuration.

- `editor-cookie-clicker-starter` is the clean learner starting point. Its config uses the identifier `editor-cookie-clicker-starter`, the type `code_editor_scratch`, and `build: true`.
- `editor-cookie-clicker-complete` contains the finished game. Its config uses the identifier `editor-cookie-clicker-complete`, the type `code_editor_scratch`, and `build: false`.

The completed archive implements the scripts shown in the tutorial, including guarded equipment and helper purchases, order-independent equipment boosts, helper-rate updates, and the final win condition.

## `images/`

This directory contains the hero image, downloadable sprites, screenshots, and animations used by the tutorial. Learner-facing Markdown uses raster PNG or GIF images. `backdrop1.svg` is retained as a downloadable Scratch project asset rather than embedded in a tutorial page.

## `resources/`

`pizza-party.pdf` is the printable project resource.

## `solutions/`

`Pizza Party _ Endless Clicker.sb3` is the completed learner solution and matches the completed project in `code/`.

## Tutorial files

- `landing.md` introduces the project and previews the finished game.
- `meta.yml` supplies the title, description, hero image, and ordered list of 30 steps.
- `step_1.md` through `step_30.md` contain the learner instructions. Step 1 marks engagement, step 29 marks completion of the directed build, and step 30 is the final customization challenge.

Scratch scripts use fenced `blocks3` code blocks. Calls to learner-created blocks include the explicit custom-block category override:

```blocks3
update pizzas per second :: custom
```
