# Meanwhile

Meanwhile is a lightweight Obsidian plugin for keeping context across your projects, hobbies, ideas, and goals. Save a brief checkpoint about where you left off, what you might do next, and any useful links or notes.

When you come back to something, Meanwhile helps you pick up where you left off.

Not everything needs a finish line. Some things are ongoing interests, others are projects to complete or ideas to explore. Checkpoints are a quick way to capture what was on your mind so it's easier to return to later.

## How it works

1. **Add a thing.** Open Meanwhile using the feather icon or the **Open Meanwhile** command, then select **Add a thing**. Give it a name, like “Family history” or “Making music.”
2. **Save a checkpoint.** Open the thing and select **New checkpoint**. Jot down where you left off. You can also add something for **Next time**, plus questions or links you want to keep handy.
3. **Return when you’re ready.** Open Meanwhile to see your latest checkpoint for each thing. Select a thing to see the full checkpoint and its history. You can also open the underlying notes by selecting the thing’s title or a checkpoint.

Give each thing a color and mark it **Active**, **Resting**, or **Archived**. In Meanwhile’s settings, you can choose which groups to show, how to sort your things, and whether cards have colored borders. Archived things are hidden by default.

## Install or upgrade

To install Meanwhile from a ZIP package:

1. Unzip the package and find `main.js`, `manifest.json`, and `styles.css`.
2. In your vault’s `.obsidian/plugins` folder, create a folder named `meanwhile` and copy the three files into it. The `.obsidian` folder may be hidden by your file manager.
3. In Obsidian, open **Settings → Community plugins**, turn off Restricted mode if needed, and enable **Meanwhile**.
4. Select the feather icon in the ribbon or run the **Open Meanwhile** command.

To upgrade, replace the three files in the `meanwhile` plugin folder with the new versions, then restart Obsidian or disable and re-enable Meanwhile. Your things and checkpoints stay in your vault.

Install and enable Meanwhile on each device where you want to use it. You can use Obsidian Sync or another compatible service to sync your vault.

## Your notes and files

Your things and checkpoints are ordinary Markdown notes in your vault, so you can open and edit them in Obsidian. Meanwhile makes no network requests.

By default, Meanwhile creates a folder for each thing inside `Things`. Each folder contains the thing’s note and a `Checkpoints` folder. For example, a checkpoint for Family history might be named `Family history - 2026-11-15.md`. Multiple checkpoints saved on the same day get different filenames.

You can choose a different root folder in Meanwhile’s settings. Meanwhile finds things inside that folder and its subfolders; changing the setting doesn’t move your notes. You can use an existing folder for a thing as long as it doesn’t already contain a note with the same name.

Meanwhile uses note properties to recognize your things and connect their checkpoints. If you edit a checkpoint note, keep its section headings—**Context**, **Next time**, **Open questions**, and **References**—so Meanwhile can read the contents. Optional sections can be omitted. Obsidian wiki links in References can be opened from the thing’s detail page; other Markdown links can be opened from the checkpoint note.

Meanwhile includes mobile layouts and has been used on iOS; Android has not yet been tested.

## License

Meanwhile is licensed under the [MIT License](LICENSE).
