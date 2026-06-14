# Progress — Course #1: Python for CV with OpenCV & Deep Learning

Authoritative curriculum: [`../CURRICULUM.md`](../CURRICULUM.md) (Course #1).
**Artifact target:** real-time camera/video pipeline + first detector demo + structured detection logs.

> **▶ Resume cursor: `06-object-detection/face_detection.ipynb`** (empty — start here).

## Section status

Legend: ✓ done · 🚧 in-progress · ⬜ stub/not started

| # | Section | Status | Notes |
|---|---------|:--:|-------|
| 01 | Course Overview & Introduction | ✓ | |
| 02 | NumPy & Image Basics | ✓ | incl. assessment |
| 03 | Image Basics with OpenCV | ✓ | drawing, direct drawing |
| 04 | Image Processing | ✓ | blurring, gradients, histograms, threshold, morphology |
| 05 | Video Basics | ✓ | video + drawing on video |
| 06 | Object Detection | 🚧 | done: template/edge/contour/grid/feature-matching/watershed · **TODO: `face_detection.ipynb` (Haar — cascades in `data/haarcascades/`)** |
| 07 | Object Tracking | ⬜ | do fully — optical flow, MeanShift/CamShift, tracking APIs |
| 08 | Deep Learning for CV | ⬜ | **skim & skip** — concept note only; DL routed to PyTorch (#2) / YOLOv12 (#6); do **not** install TF/Keras |
| 09 | Capstone Project | ⬜ | classical OpenCV segmentation / finger-count |
| — | Course artifact | ⬜ | camera pipeline (detect + track) w/ FPS + structured detection logs |

See [`ROADMAP.md`](./ROADMAP.md) for rationale and the forward gate.

## Session Log

Append-only. One dated line per work/check-in session (newest at top). Source of truth = `git log`.

- 2026-06-14 — Repo organized & structured (curriculum vendored, hygiene, README/ROADMAP/PROGRESS/notes added). Resume cursor set to `06-object-detection/face_detection.ipynb`.

---

### Scheduled progress-tracking task (paste into a weekly Claude Code on the web session)

Cadence: **weekly** (matches the catalog's "one source per week / Sunday review" rhythm).
Repo: `computer-vision`. Branch: your active working branch (or `main` once merged).

> In the `computer-vision` repo, read `opencv-deep-learning-course/PROGRESS.md` and
> `git log` since the last Session Log entry. Update the section status table and the
> resume cursor to match what's actually committed, append one dated Session Log line
> summarizing what advanced + the next concrete step, then commit and push. If nothing
> changed since last run, say so and don't commit.
