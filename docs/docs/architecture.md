# System Architecture

Sonar image/tile
  → Preprocessing (denoise, normalize, tile) [classical CV, OpenCV]
  → YOLO detector (pipe_cylinder / entangled_net_debris / shipwreck / natural_seafloor)
  → Post-filter (classical CV: shape/shadow/context checks)
  → OOD/uncertainty scoring (distance-based, on detector embeddings)
  → Natural-vs-man-made verification (secondary classifier on crop)
  → Priority scoring (explainable formula)
  → Geolocation tagging (from nav metadata)
  → JSON/CSV report + dashboard
