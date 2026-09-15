# FreeCAD AEG Battery Support

Personal project to design a 3D-printable battery support/mount in FreeCAD
for an AEG (airsoft) battery pack that I own, modeled from my own reference
photos.

This isn't a tutorial — it's my own modeling attempt, following the approach
shown in a YouTube tutorial but applied to my own battery. I'll add more
YouTube references here as the project progresses.

## Reference tutorial(s)

- Barbatronic —
  ["\[TUTO\] - FreeCAD - Créer une pièce 3D à partir d'une photo"](https://youtu.be/XsQBDVEu6WY) —
  shows how to bring a photo into FreeCAD as a reference/background image on
  a sketch plane and trace a real object's outline from it to build an
  accurate 3D model.

## Project structure

```
pics/                   # reference photos of the battery (raw shots and
                         # cropped/aligned "layout" versions used for tracing)

docs/
└── screenshots/
    ├── gimp/            # screenshots documenting image cleanup in GIMP
    └── freecad/         # screenshots documenting the FreeCAD modeling steps

cad/                     # FreeCAD source file(s) (.FCStd)

exports/                 # STEP / STL / 3MF exports for slicing and printing

TODO.md                  # task list and progress tracker
```

## Status

Work in progress — see [TODO.md](TODO.md) for the current step and next
tasks. The FreeCAD source file isn't committed yet while the model is still
very early; it'll be added once there's a first meaningful version.
