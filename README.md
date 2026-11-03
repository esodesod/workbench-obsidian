## Workbench

This is a plugin for [Obsidian](https://obsidian.md).

It allows you to capture thinking from whatever you're currently looking at into a "Workbench" note. Link and embed pages, headers, and blocks, or copy the current line. You can also use alt+click and cmd/windows+alt+click to add content to the workbench.

### Demo:

[A demo of the various ways to add things to your workbench.](https://i.imgur.com/tG4dOvp.gif)

Note: you may need to double-click when using the click-based features! 

Insert and clear the materials on the workbench:
![A demo of insert contents of workbench and clear workbench](https://i.imgur.com/YCazTIb.gif)

### Settings
Control the name of the Workbench note, the line prefix for every item added to the workbench, and what alt+click or cmd/windows+alt+click do in the plugin's Settings.

### Manually installing the plugin

- Copy over `main.js` and `manifest.json` to your vault `VaultFolder/.obsidian/plugins/workbench-obsidian/`.

## Releasing

This plugin is distributed via GitHub releases, installable with
[BRAT](https://github.com/TfTHacker/obsidian42-brat) in Obsidian.

Requirements (BRAT / Obsidian):

- Release tag, release name, and the `version` field of the released
  `manifest.json` must be the **same semantic version string** (e.g.
  `2026.11.03`).
- The release must attach `main.js`, `manifest.json`, and `styles.css`
  as **individual file assets** (not in a zip).

### Creating a release

1. `npm install && npm run build`
2. Bump the `version` field in `manifest.json` (and `package.json`)
   to the release version and commit
3. GitHub repo → **Releases → Create a new release**
4. Tag: `2026.11.03`, release title: `2026.11.03`
5. Attach the three files from the repo root: `main.js`, `manifest.json`,
   `styles.css`

### Installing with BRAT

In Obsidian, with BRAT installed:

1. Command palette → **BRAT: Add a beta plugin for testing**
2. Paste this repository's URL
3. BRAT picks up the latest (or the frozen) release and installs
   `main.js` / `manifest.json` / `styles.css` into
   `.obsidian/plugins/workbench-obsidian/`

