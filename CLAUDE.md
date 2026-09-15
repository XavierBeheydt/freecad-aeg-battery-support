# AI Instructions

This file provides guidance to AI coding agents (Claude Code, and other
agents reading it via the `AGENTS.md` symlink) when working in this
repository.

## Project overview

This is a personal FreeCAD modeling project, not a software project — there
is no build, lint, or test tooling. The goal is to design a 3D-printable
battery support/mount for an AEG (power tools) battery — the kind used in
AEG cordless drills — modeled from reference photos, following the
photo-to-3D-sketch approach described in [README.md](README.md).

## Repository structure

- `pics/` — reference photos of the battery (raw shots and cropped/aligned
  "layout" versions used for tracing in FreeCAD sketches).
- `docs/screenshots/gimp/`, `docs/screenshots/freecad/` — screenshots
  documenting the image cleanup and modeling workflow.
- `cad/` — FreeCAD source file(s) (`.FCStd`).
- `exports/` — STEP / STL / 3MF exports for slicing and printing.
- `TODO.md` — task list and progress tracker; check it for the current step
  before suggesting next actions.

## Language

Write everything in this repository — README, TODO, commit messages, code
comments, docs — in English only. Conversation with the user can be in
whichever language they use.

## Working with the FreeCAD file

- `.FCBak` backup files and the `backup/` directory are gitignored — never
  commit them.
- The `.FCStd` file is a binary FreeCAD document; it can't be reviewed as a
  text diff, so describe what changed in the commit message instead.
