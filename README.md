# Meanwhile

**Meanwhile** is a lightweight Obsidian plugin for keeping context across your projects, hobbies, ideas, and goals. Save a brief checkpoint about where you left off, what might come next, and any links you want to keep handy.

When you switch between things, Meanwhile helps you find your place again.

## How it works

- **Add a thing:** Give your project, hobby, idea, or goal a name. Choose a folder, or let Meanwhile create one under `Things/` by default.
- **Save a checkpoint:** Capture where you left off and what might come next. Add questions or links if they’re useful.
- **Come back to it:** Open Meanwhile to see where you left off and what’s next for each thing. Choose a thing for the full latest checkpoint and previous checkpoints. Select a checkpoint to open its note, or select the thing’s name to open its own note.
- **Set a state and color:** Mark a thing Active, Resting, or Archived, and give it a color. Archived things are hidden by default.
- **Make it yours:** Sort things by latest checkpoint or name, and choose whether to show resting and archived things and the colored card borders.

## Install or upgrade

Meanwhile stores its plugin files in the `meanwhile` folder.

1. Unzip the package.
2. Copy `main.js`, `manifest.json`, and `styles.css` from `meanwhile/` into `<your vault>/.obsidian/plugins/meanwhile/`, replacing the existing files when upgrading.
3. Enable **Meanwhile** in **Settings → Community plugins**. If upgrading, restart Obsidian or disable and re-enable the plugin.
4. Use the feather ribbon icon or the **Open Meanwhile** command to open your things.

Your existing notes and checkpoints remain in your vault. Install and enable the plugin separately on each device; use Obsidian Sync or another compatible service if you want to sync your notes.

## Storage and limitations

Each thing’s metadata is stored in a Markdown note named for the thing, such as `Inscription.md`. Checkpoints are Markdown notes in a `Checkpoints/` folder, named for the thing and local date (for example, `Photography - 2026-11-15.md`, with a number for additional checkpoints that day); and custom colors and state are stored in the thing’s frontmatter. New thing notes use `meanwhile_type`, `meanwhile_id`, `name`, `created`, and `state` properties; checkpoints use `meanwhile_type`, `meanwhile_id`, `meanwhile_thing`, and `created`. The plugin makes no network requests.

- Things are indexed inside the configured root folder. Folders outside it aren’t indexed automatically.
- A thing cannot be added to a folder if a note with its name already exists there.
- Keep checkpoint headings as `## Context`, `## Next step`, `## Open questions`, and `## References` for the plugin to read them.
- Wiki links in References are clickable in the detail view. Other Markdown links remain available in the checkpoint note.
- Mobile layouts are included, but the plugin has not yet been tested on an iOS or Android device.

## License

Meanwhile is licensed under the [MIT License](LICENSE). Interface icons use Obsidian's built-in Lucide icons.
