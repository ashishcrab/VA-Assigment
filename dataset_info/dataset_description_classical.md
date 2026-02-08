# UCF101 Subset

This repository produces color and shape features per video, saving plots and per-video JSON/NPZ in `outputs/`.

## Structure

```
dataset/
├── Basketball/
├── WalkingWithDog/
├── CricketBowling/
├── splits/
│   ├── train.txt
│   ├── val.txt
│   └── test.txt
└── outputs/
        └── <Class>/<VideoName>/
            ├── frames_grid.png
            ├── rgb_hist_avg.png, hsv_hist_avg.png
            ├── hsv_moments_sequence.png, rgb_moments_sequence.png
            ├── canny_edges_frame0.png, edge_hist_avg.png, edge_hist_sequence.png
            ├── contours_threshold_frame0.png, contours_overlay_frame0.png
            ├── contour_stats_avg.png, contour_stats_sequence.png
            ├── hog_visual_frame0.png
            ├── features.json
            └── features.npz
```
