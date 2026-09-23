# World Geography

`index.html` is the home page. It lists six units, and each unit links to lesson pages: plain `.html` files stored in this repository.

## Adding a page

1. Upload the `.html` file to this repository, ideally into a folder for its unit (for example `unit-1/`). In GitHub: **Add file → Upload files**. To upload into a folder, type the folder name before the file name, like `unit-1/topographic-maps.html`.
2. Open `index.html` and find the unit's `"lessons": []` list near the bottom. Add an entry:

   ```json
   "lessons": [
     {"title": "Reading a topographic map", "file": "unit-1/topographic-maps.html"},
     {"title": "Map projections", "file": "unit-1/projections.html"}
   ]
   ```

   Separate entries with commas. `title` is the text shown on the home page; if you leave it out, the file name is used.
3. Commit. Once GitHub Pages rebuilds (usually within a minute), the link appears on the home page.

You can rename units or change their descriptions in the same list.

## Publishing with GitHub Pages

In the repository's **Settings → Pages**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then save. The site will be at `https://<account>.github.io/World-Geography/`.
