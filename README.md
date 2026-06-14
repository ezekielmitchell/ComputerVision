# computer-vision

Computer-vision study & research repo, driven by the **Aegis Nexus curriculum**.
The single source of truth for *what to study and why* is [`CURRICULUM.md`](./CURRICULUM.md)
(vendored verbatim from the Aegis Nexus Course Catalog — `[[wikilinks]]` in it resolve
inside Aegis Nexus, not this repo). This README and all course docs derive from it.

## Where this sits in the curriculum

This repo currently covers **Course #1 — Python for CV with OpenCV & Deep Learning**
(Portilla), the June 2026 main course. Its artifact target per the catalog is a
*real-time camera/video pipeline + first detector demo* with *structured detection logs*.

Forward gate: **OpenCV #1 → PyTorch #2 (July) → YOLOv12 #6**. See
[`opencv-deep-learning-course/ROADMAP.md`](./opencv-deep-learning-course/ROADMAP.md).

## Layout

```
computer-vision/
├── CURRICULUM.md                  # authoritative curriculum (Aegis Nexus catalog)
├── requirements.txt               # Python deps (OpenCV, NumPy, matplotlib, scikit-learn, Jupyter)
└── opencv-deep-learning-course/   # Course #1 — Portilla OpenCV
    ├── README.md                  # course section index
    ├── PROGRESS.md                # live status + resume cursor + session log
    ├── ROADMAP.md                 # how to finish the course + what's next
    ├── notes/                     # concept notes / artifacts
    └── 01..09-*/                  # one folder per course section
```

**Convention for future courses:** PyTorch (#2) and YOLOv12 (#6) will land as *sibling
folders* next to `opencv-deep-learning-course/` when they start — they are documented
here, not pre-created.

## Current progress (snapshot)

See [`opencv-deep-learning-course/PROGRESS.md`](./opencv-deep-learning-course/PROGRESS.md)
for the live table. **Resume cursor: `06-object-detection/face_detection.ipynb`.**

## Running

```bash
pip install -r requirements.txt
jupyter lab          # open any 0X-*/section notebook
```
