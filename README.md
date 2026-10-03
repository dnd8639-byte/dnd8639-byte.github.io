# dnd8639-byte.github.io

David DeConti's research archive, published with GitHub Pages at https://dnd8639-byte.github.io

```
index.html              home page: projects + research log
assets/site.css         shared colors, fonts and layout (light and dark mode)
mcpt-lab/               mcpt-lab results page (+ decay_data.json)
futures-research/       preregistered futures research write-up
quant-projects/         ten quant mini-projects: results page, figures/ and code/
_template/              starting point for a new project page (not linked from the site)
```

## Add a new project
1. Copy the template into a new folder (use a short name with dashes):
   `cp -r _template my-new-project`
2. Edit `my-new-project/index.html` (everything in CAPITALS, and the sections).
3. In `index.html`, copy one `<li class="project">` block to the top of the list and point it at `my-new-project/`.
4. Add a line to the research log in `index.html` (newest first, year only).
5. Publish:
   ```
   git add .
   git commit -m "Add my-new-project"
   git push
   ```
   The site updates within a minute or two.

## Preview on your Mac before publishing
```
python3 -m http.server 8000
```
Then open http://localhost:8000 in a browser. Press Control + C to stop.
