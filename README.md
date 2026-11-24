# Anime Mask

AI background removal and a Roto Brush-style brush for anime clips in Adobe After Effects: a dockable panel
(`Anime Mask.jsx`) with a Python engine (`anime_mask_engine.py`).

This repository holds the published versions as **releases**. Each release has:

- `anime_mask_panel.jsx`: the panel (installed as `Anime Mask.jsx`)
- `anime_mask_engine.py`: the engine
- `anime_mask_update.py`: the updater the panel uses
- `manifest.json`: versions, notes, and the size and SHA-256 of each file

## First install

Copy the three files from the latest release into
`<After Effects>\Support Files\Scripts\ScriptUI Panels`, renaming `anime_mask_panel.jsx` to `Anime Mask.jsx`,
then restart After Effects and open **Window > Anime Mask.jsx**. The engine needs Python with its packages
installed (see the panel's Help).

## Updates

After that, **Settings > Updates** in the panel checks this repository, and **Install Update** downloads the
newest release, checks every file against the manifest, and installs it into `%APPDATA%\AnimeMask\app`
(the panel After Effects loads runs the newer copy from there). Close and reopen the panel to use it.
