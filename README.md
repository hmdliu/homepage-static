# homepage-scratch

A minimal, NYU-styled static academic homepage (plain HTML + one CSS file, no build step).

## Structure

```
index.html               # Single page: navbar, bio (#about), selected publications (#publications), misc (#misc)
assets/css/style.css     # All styles; colors and photo width are CSS variables at the top
assets/img/              # Photo; pub thumbnails in assets/img/pubs/
```

## Customizing

- **Colors**: edit the `:root` variables in `assets/css/style.css` (defaults follow the [NYU color palette](https://www.nyu.edu/employees/resources-and-services/media-and-communications/nyu-brand-guidelines/designing-in-our-style/nyu-colors.html); highlight is NYU Violet `#57068c`).
- **Bio alignment**: tune `--photo-width` so the photo column and bio text end at roughly the same height.
- **Selected publication**: copy an `<article class="pub-feature">` block in `index.html`.
- Wrap your own name in `<span class="me">` to bold it in author lists.

## Local preview

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

Deploys as-is to GitHub Pages.
