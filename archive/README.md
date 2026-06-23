# Archive

Content that is intentionally **kept in the repo but not published** to the website.

Hugo only builds files under `content/` and copies files under `static/`. Anything in
this `archive/` folder is outside both, so it is preserved in version control but never
appears on nirmaljeffrey.dev.

## Structure

The original repo layout is mirrored so items can be restored by moving them back:

- `archive/content/projects/` — archived project markdown
- `archive/static/projects/` — images those projects reference

## Restore a project

```sh
mv archive/content/projects/<name>.md content/projects/<name>.md
mv archive/static/projects/<image>.jpg static/projects/<image>.jpg
npm run css:build   # only if you also touched layouts
```

## Currently archived projects

- Multi-Modal Vehicle (`multi-modal-vehicle`)
- Air Boat (`air-boat`)
- Air Cooler (`air-cooler`)
- Bluetooth Controlled Arduino Car (`bluetooth-controlled-arduino-car`)
- Portable Charger (`portable-charger`)
- Glider (`glider`)
