# diagram-src

Source files for hand-built diagrams used as cover images on the site. This
folder is **not** published by Hugo (it is outside `content/` and `static/`), it
just keeps the sources under version control.

## Re-rendering a diagram to PNG

Edit the `.html`, then render it with headless Chrome:

```bash
google-chrome --headless=new --disable-gpu --hide-scrollbars \
  --force-device-scale-factor=2 --window-size=1200,630 \
  --screenshot=out.png \
  file:///absolute/path/to/diagram-src/ravi/ravi-architecture.html
```

- `--force-device-scale-factor=2` gives a 2x (retina) PNG, e.g. 2400x1260.
- `--window-size` must match the `<svg>` / `<body>` dimensions in the HTML.

Then copy `out.png` to the matching cover location, e.g.
`static/projects/ravi/ravi-architecture.png`, and run `hugo`.

## Files

- `ravi/ravi-architecture.html` -> `static/projects/ravi/ravi-architecture.png`
  (cover for the Ravi project page).
