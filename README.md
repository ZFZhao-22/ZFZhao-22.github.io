# zfzhao-22.github.io

Personal academic website of Zifeng Zhao: https://zfzhao-22.github.io

Plain HTML and CSS with no build step. GitHub Pages serves the `main` branch as is.

| File | What it holds |
|---|---|
| `index.html` | Home page: about, research, selected publications, projects, teaching, background, service, contact |
| `publications.html` | Full list of publications and presentations |
| `assets/css/style.css` | All styles (light and dark mode) |
| `assets/img/zifeng-zhao.jpg` | Portrait (square) |
| `files/Zifeng_Zhao_CV.pdf` | The CV linked from every page |

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Common edits

- **Replace the CV**: overwrite `files/Zifeng_Zhao_CV.pdf` and keep the file name, so existing links keep working.
- **Add a paper**: in `publications.html`, copy an existing `<li class="pub">` block into the right year and give it the next label and `id` (e.g. `J.28` / `J28`). Add `data-lead` if Zifeng is first or corresponding author. Section counts update automatically.
- **Numbers on the home page**: the four figures under the bio (`<dl class="facts">` in `index.html`) are typed by hand. Update them when the CV changes.
- **Footer date**: update "Last updated" in both HTML files.
