# Roadmap — finishing OpenCV fundamentals & what's next

Sourced from the authoritative curriculum [`../CURRICULUM.md`](../CURRICULUM.md)
(Course #1, June 2026 main course). You write all lesson code yourself; this is the path.

## Pick up from mid fundamentals

1. **Finish §06 Object Detection.** The only gap is `06-object-detection/face_detection.ipynb`
   (currently empty). Implement Haar-cascade face/eye detection — the cascade XMLs are
   already in `data/haarcascades/` (and `data/lbpcascades/`). This closes the section.

2. **§07 Object Tracking — do it fully.** Optical flow (Lucas-Kanade & dense),
   MeanShift/CamShift, and the OpenCV tracking APIs. High value: it's classical,
   it's the basis of the camera-pipeline artifact, and it sets up the tracking work
   in YOLOv12 (#6) (Bot-SORT/ByteTrack) later.

3. **§08 Deep Learning for CV — skim & skip.** The course teaches CNNs in Keras/TensorFlow
   (MNIST/CIFAR/YOLOv3). Per the curriculum, deep learning is routed to **PyTorch (#2,
   the July main course)** and **YOLOv12 (#6)**, and there's a "no more YOLO courses"
   rule. **Do not install TF/Keras or grind MNIST/CIFAR.** Instead, watch for concepts
   and write one short note in [`notes/`](./notes/) — especially **classification metrics**
   (precision/recall/false positives), which feed Project 4 (Low-False-Positive Classifier).

4. **§09 Capstone — do it.** The classical OpenCV segmentation / finger-counting project
   (background subtraction → threshold → contours → convex hull). Good, self-contained artifact.

## The course artifact (the catalog deliverable)

Build a small **real-time camera pipeline**: capture → Haar detect → a tracker, with
**FPS measurement** and **structured detection logs** (e.g. JSONL: timestamp, frame,
label, bbox, confidence). This pairs with your Rust log-parser parallel track (Course #3)
and earns the Course #1 résumé keywords honestly. *(You build this — it's listed here as
the spec, not implemented.)*

## Forward gate

**OpenCV #1 → PyTorch #2 (July main) → YOLOv12 #6.** PyTorch replaces the course's Keras
deep-learning section. Earn résumé keywords only against committed artifacts (see the
Skills → Résumé table in `../CURRICULUM.md`).

## Environment note

`requirements.txt` includes OpenCV, NumPy, matplotlib, scikit-learn, Jupyter — but **not**
TensorFlow/Keras or PyTorch (intentional, per the skim-&-skip decision). Add PyTorch when
Course #2 starts in July.
