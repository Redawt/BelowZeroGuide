# Below Zero: A Frost Modding Guide


## Description

This is a static GitHub Pages website containing a [guide](https://redawt.github.io/BelowZeroGuide) for setting up **Fallout 4** and the [FROST Survival Simulator](https://www.nexusmods.com/fallout4/mods/18898).

Link: [https://redawt.github.io/BelowZeroGuide](https://redawt.github.io/BelowZeroGuide)

## Requirements
This GitHub project uses [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

If you want to contribute to this website, you need to:

1. Install Git
2. Install Python and Pip
3. Install Visual Studio Code
4. Install [mkdocs-material](https://squidfunk.github.io/mkdocs-material/getting-started/)
5. Clone this repository with Git
6. Open it the `.vscode/BelowZero.code-workspace` file with VS Code
7. Edit or add markdown files in the `docs` folder
8. Make a pull request

Please get familiar with mkdocs-material, the structure of the folders containing markdown files, and how they are used in the project.


## Project Structure
This project uses markdown for creating the web pages.
You can find all markdown files and image assets in the `docs` folder

```
├── docs
│   ├── additional-mods.md
│   ├── assets
│   │   └──  [Contains all image files]
│   ├── faq
│   │   └──  [Markdown files for the FAQ section of the website.]
│   ├── guide
│   │   └──  [Markdown files for the main modding guide part of the website]
│   ├── index.md [Landing page of the website]
│   ├── introduction
│   │   └──  [Markdown files for the introduction and requirements part of the website]
│   ├── mods
│   │   └── [Markdown files in subfolders for mod descriptions found in the guide section of the web site]
│   ├── overrides
│   │   └── home.html [Custom landing page template for the web site]
│   └── stylesheets
│       └── extra.css [Custom CSS for the web site]
└── mkdocs.yml [Contains the navigational structure, plugins/extensions info, theme etc for this web site]
```