# miku.gg Character Toolkit

A small, offline tool for creators on [miku.gg](https://miku.gg). Load your novel files, tidy up your characters, move them between novels, and clean up the memories a narration has built up. It is a single web page: nothing is uploaded anywhere, and it never changes the files you load. It only gives you an edited copy to download.

## Quick start

1. Open the page (or download `index.html` and open it in any modern browser).
2. Load one or two files. Use **Choose file…**, drag them onto the panels, or press **Load two files at once…**.
3. Click **Edit** on a character, or **Send** to copy it to the other file.
4. Press **Download edited file** on each file you changed, then load it back into miku.gg.

Keep your original files as a backup. The tool never overwrites them.

## Which files work?

| File | What you can do |
| --- | --- |
| **Novel** (exported from the novel builder) | Edit, send and delete characters. Edit their lorebooks and indicators. |
| **Narration history** (a novel that has been played) | Everything above, plus view, edit, delete and transfer each character's memories. |

> **Important for narrations.** In the narration window, use the **"Download narration history"** and **"Load narration history"** buttons. Do **not** use the **"Saved narrations" / "My narrations"** tab. Files from that tab are laid out differently and miku.gg will not open them again after editing. The tool shows a warning on any file that looks like it came from there.

## What you can do

### Edit a character
Press **Edit** (or click the name). The editor has tabs:

- **Description**: the description, short description and outfit descriptions.
- **Lorebooks**: only the lorebooks this character is specifically tagged in. Global lorebooks are left out on purpose. Edit the entries, keywords and text.
- **Indicators**: the indicators and variables tied to this character, including those in its variable banks. Warnings tell you when something is shared with other characters or used by scenes and objectives, so you know what else your edit affects.
- **Memories** (narration histories only): see below.

Nothing is written to the file until you press the green **Save changes** button (top right or bottom right of the editor). Then press **Download** on the file.

### Send a character to the other file
Press **Send to A/B**. The character is added to the bottom of the other file's character list with its outfits, emotions, images and settings. You choose exactly which of its lorebooks, indicators (each comes with its variable) and variable banks come along. Anything the other file already has is linked rather than duplicated. If the character already exists there, you can add it as a copy or replace the existing one in place.

Scenes, cutscenes and objectives that mention the character stay in the original file.

### Delete a character
Press **Delete**. The tool shows what else points at the character (scenes, cutscenes, start screens) and removes those links too, so nothing is left pointing at a character that no longer exists. Lorebooks, indicators and variables stay. **Undo delete** appears straight afterwards, and **Undo all changes** takes the file back to how you loaded it.

### Memories
As a narration is played, miku.gg writes memories into the story. Open a character's **Memories** tab to read them, change their text or importance, or tag the ones you want gone and press **Delete tagged**. Memories that were created while several characters were in the scene are flagged as shared. Editing or deleting one changes it for all of them.

When you send a character you can tick **Also transfer this character's memories**, choose which ones, and decide whether they go on the latest turn or an early turn of the other story. They are added there as plain text, only for the transferred character, and anything already there is skipped. The other file needs a narration history of at least two turns.

## Good to know

- **How memories are linked.** miku.gg stores memories on turns of the story, not on characters, so there is no owner field. The tool treats a memory as belonging to the characters on the turn it was made. Memories copied in from another file are found by the character's name, so a copied memory that never uses the name (for example one that says "she") is not listed in the Memories tab. The tab tells you how many are not shown. They are still in the file.
- **Why a memory shows up even though you did not transfer any.** The tool only adds what you tick. If the file you loaded already contained memories, for example a copy you downloaded from an earlier session, those stay. Start from your original file for a clean test.
- **Unsaved work.** The page warns you before you close it with changes you have not downloaded.

## Safety

- Runs entirely in your browser. No account, no server, no uploads.
- The page is one HTML file with no outside scripts, fonts or tracking, so you can read the source.
- It never edits the files you load. Downloads are new files, named `…_edited.json` when something changed.
- Files that do not look like a novel or narration are rejected with a message rather than loaded.

## Sharing

To host it yourself, put `index.html` in a GitHub repository and turn on GitHub Pages from the repository's `/ (root)` folder. The README and this page can sit side by side.
