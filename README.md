# Novel Character Editor & Transfer

A small single-page tool for miku.gg interactive-novel JSON files. Open it in your browser, load up to two novel `.json` files, and:

- **Edit a character's description** (plus short description and outfit descriptions).
- **Transfer a character from one file to the other.** The full character is copied to the bottom of the other file's character list, including outfits, emotions, images, tags, and the lorebooks, indicators and variables it depends on.
- **Download** the edited files. Your originals are never overwritten; edited copies are saved with `_edited` added to the name.

## Is it safe?

- It runs entirely in your browser. Your files are never uploaded anywhere.
- It makes no network requests and loads no outside scripts. You can turn off your internet and it still works.
- It is one readable file (`index.html`, about 27 KB). Open it in a text editor and check.

## Things to know

- Scenes, cutscenes and objectives that mention a character stay in the file they came from. A transferred character arrives ready to use, but you will need to place it in scenes in the new file.
- Image and audio paths are copied as they are, so both novels should use the same miku.gg asset storage.
- Back up your JSON files before editing. This is a hobby tool, tested on a small number of files.
- Not affiliated with miku.gg.

## Use it

Open the page, click **Load two files at once…** (or choose a file in each panel), click a character name to edit, use **Send to B →** / **← Send to A** to transfer, then **Download**.
