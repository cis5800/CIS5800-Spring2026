# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the **CIS 5800: Machine Perception (Spring 2026)** course repository for UPenn, taught by Prof. Lingjie Liu. It contains:
- `CIS-5800-Spr2026-CodingHW/` — Active Spring 2026 coding homework (primary working area)
- `CIS5800-MachinePerception/` — Spring 2025 archive (reference only)
- `slides/` — PDF lecture slides
- `index.html`, `syllabus.html`, etc. — Static course website


## Autograding Architecture

Homework is graded on Gradescope. Each `HomeworkN/` directory contains:
- `run_autograder` — Bash script that copies student submission files into `/autograder/source/` then runs `tests.py`, writing output to `/autograder/results/results.json`
- `setup.sh` — Installs Python 3 and pip packages on the Gradescope container
- `tests.py` — Unit test suite; must output valid Gradescope JSON to stdout

Student submissions: `HomeworkN_Student_Version/` directories contain the student-facing versions with skeleton code.

## Homework Topics

- **HW1** — Image transformations: scaling, translation, rotation (implement `homework1.py`)
- **HW2** — AR pose estimation: homography, PnP, Procrustes, P3P (implement `.py` files)
- **HW3** — 3D reconstruction: stereo epipolar geometry, disparity, depth (uses Gradio UI)
- **HW4** — Optical flow: Lucas-Kanade algorithm, epipole estimation (uses Gradio UI)