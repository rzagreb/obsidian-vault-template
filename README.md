# Obsidian Setup with Copier

This repository contains a template for quickly initializing an Obsidian Vault with a predefined folder structure and plugin configuration. By using [Copier](https://copier.readthedocs.io/), you can clone and customize this template in just a few steps.

## Main Features

- **Predefined Folder Structure**: The folders move from **inbox** to **wiki**, keeping files hierarchy as flat as possible. Folder names coudl be changed during the setup process to match your personal workflow. The default structure is as follows:
  - `01_import/`: Automatically added notes from other services (e.g. web clipper, Pocket, and other services).
  - `02_inbox`: Manually created or quickly captured notes.
  - `03_tasks/`: Where your tasks or to-do items are stored.
  - `04_incubator/`: Early-stage practical ideas that need further thinking.
  - `04_wiki/`: Completed, connected reference notes (knowledge base). These should not include tasks or temporary notes.
    - This is where most of notes from `02_inbox` will end up after processing.
  - `05_code/`: For code snippets, scripts, or programming-related notes.
  - `06_fun/`: Ideas to do some fun things: movies, books, games, visit places etc. Deleted after completion.
  - `09_assets/`: For images, videos, or other media files that are used in your notes.
  - `99_meta/`: For metadata, such as templates, special pages, etc.
  - `Home.md`: The main entry point for your vault, linking to other folders and notes.
- **Plugin Configuration**: Includes useful plugin configurations for a smooth start. All plugins are set up to create notes with a consistent naming convention: `{YYMMDD}_{title}.md`, where `{title}` is the title you provide when creating a note. The actual title in the note is still `{title}`.
  - **dataview**: Lets you query and display data from your notes as tables, lists, or charts.
  - **homepage**: Sets a custom start page to quickly access your key notes and features.
  - **link-favicon**: Automatically adds website icons (favicons) next to external links.
  - **mermaid-tools**: Improves creation and editing of mermaid diagrams in your notes.
  - **metadata-extractor**: Pulls and organizes metadata from your markdown files.
  - **obsidian-advanced-uri**: Generates detailed URIs for deep linking and interacting with notes.
  - **obsidian-auto-link-title**: Automatically retrieves and sets titles for linked pages.
  - **obsidian-front-matter-title-plugin**: Uses front matter data to set your note titles.
  - **obsidian-paste-image-rename**: Renames pasted images automatically based on preset rules.
  - **quickadd**: Provides a fast way to create new notes or tasks with custom templates.
  - **table-editor-obsidian**: Offers an easy interface to edit and manage markdown tables.
  - **tag-wrangler**: Helps you manage, organize, and rename tags across your vault.
  - **templater-obsidian**: Adds advanced templating features with code and variables for note creation.

## Prerequisites

- **Python 3.7+** installed and working in your environment.
- **Copier** (`pip install copier`) installed globally or in a virtual environment.

## Installation Steps

1. **Clone the Template with Copier**  
   ```bash
   copier copy https://github.com/rzagreb/obsidian-vault-template /path/to/your/new/vault
   ```
   - Replace `/path/to/your/new/vault` with the desired local path where you want your Obsidian Vault.

2. **Fill in the Prompts**: During the process, Copier will ask you for inputs (such as folder names). Provide values that suit your personal workflow or accept the defaults.
3. **Open Your New Vault**  
   - Launch Obsidian and **Open Folder as Vault** at the `/path/to/your/new/vault` location.
   - Verify that the folder structure and any specified plugin configurations match your expectations.

## Additional Information

* For Copier details, see the [Copier Documentation](https://copier.readthedocs.io/).
* For Obsidian help, refer to the [Obsidian Help](https://help.obsidian.md/).