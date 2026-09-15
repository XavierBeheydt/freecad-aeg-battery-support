# TODO

## 1. Photo shoot — reference faces (`dataset/xyz-faces/raw/`)

- [x] Take one straight-on photo per face of the battery (front, back, top,
      bottom, left, right).
- [ ] Shoot on a plain, uncluttered background (no visual "pollution" that
      could distort the trace in FreeCAD).
- [ ] Keep the camera perpendicular to each face to avoid perspective
      distortion.
- [ ] Include a scale reference (ruler / grid paper / caliper) in each shot so
      the image can be scaled accurately once imported in FreeCAD.

## 2. Photo shoot — photogrammetry set (`dataset/photogrametry/`)

- [x] Take a full set of overlapping photos all around the battery (turntable
      style, ~60-70% overlap between consecutive shots).
- [ ] Cover top and bottom angles as well, not just the sides.
- [ ] Keep consistent, diffuse lighting to avoid harsh shadows/reflections
      that confuse photogrammetry matching.

## 3. Image processing (GIMP)

- [ ] For each `xyz-faces` photo: straighten with a rotation if the face
      isn't level.
- [ ] Crop tight around the battery to remove background clutter before using
      the image as a FreeCAD reference/background.
- [ ] Screenshot each GIMP step (rotate, crop, export) to document the
      cleanup process for the tutorial writeup.
- [ ] Export cleaned images (e.g. to a `dataset/xyz-faces-clean/` or
      `processed/` folder) ready to import into FreeCAD.

## 4. FreeCAD modeling (photo-based) — in progress

- [ ] Import the cleaned face photos as background/reference images on the
      corresponding sketch planes.
- [ ] Scale each image using the known reference (ruler/grid) so real-world
      dimensions match.
- [ ] Trace the battery outline on each sketch.
- [ ] Build the 3D model from the traced sketches (pad/pocket/loft as needed).
- [ ] Screenshot key FreeCAD modeling steps for the tutorial writeup.

## 5. Photogrammetry variant

- [ ] Convert/prepare the `photogrametry` photo set for the chosen
      photogrammetry tool (e.g. Meshroom).
- [ ] Run the photogrammetry reconstruction to get a 3D mesh of the battery.
- [ ] Clean up the resulting mesh (remove background/floor, fill holes).

## 6. Comparison & design

- [ ] Compare the hand-modeled (photo-based) battery against the
      photogrammetry mesh for accuracy.
- [ ] Design the actual battery support/mount around the validated battery
      model.

## 7. Print & fit test

- [ ] Slice and 3D print the support.
- [ ] Test-fit the real battery in the printed support, note any adjustments
      needed.

## 8. Writeup

- [ ] Update `README.md` with final results, lessons learned, and photos of
      the finished print.
