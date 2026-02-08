# Dataset Overview

- Generated: 2026-01-17T22:07:38
- Root: C:\Users\avashist\Downloads\Personal\Personal\WILP\Semester 3\Video Analytics\Assignments\Assignment 1\Dataset_DL
- Number of classes: 3
- Total videos: 396

## Directory Structure

dataset/
├─ class_1/
├─ class_2/
├─ ...
├─ splits/
│  ├─ train.txt
│  ├─ val.txt
│  └─ test.txt
├─ dataset_info.txt
└─ README.md

## Classes and Label Indices
- Basketball -> 0 | total=134 (train=94, val=20, test=20)
- CricketBowling -> 1 | total=139 (train=97, val=21, test=21)
- WalkingWithDog -> 2 | total=123 (train=86, val=18, test=19)

## Split Sizes
- Train: 277
- Val:   59
- Test:  60

## Split File Format
- Each line: '<relative_path_from_dataset_root> <label_index>'
- Example: 'class_1/video_001.mp4 0'

### Examples (train.txt)
- CricketBowling/v_CricketBowling_g23_c03.avi 1
- WalkingWithDog/v_WalkingWithDog_g01_c01.avi 2
- Basketball/v_Basketball_g15_c01.avi 0
- Basketball/v_Basketball_g07_c02.avi 0
- Basketball/v_Basketball_g25_c05.avi 0

### Examples (val.txt)
- CricketBowling/v_CricketBowling_g18_c01.avi 1
- Basketball/v_Basketball_g15_c07.avi 0
- WalkingWithDog/v_WalkingWithDog_g04_c02.avi 2
- CricketBowling/v_CricketBowling_g12_c01.avi 1
- CricketBowling/v_CricketBowling_g02_c03.avi 1

### Examples (test.txt)
- Basketball/v_Basketball_g25_c03.avi 0
- WalkingWithDog/v_WalkingWithDog_g14_c01.avi 2
- CricketBowling/v_CricketBowling_g13_c05.avi 1
- WalkingWithDog/v_WalkingWithDog_g06_c03.avi 2
- CricketBowling/v_CricketBowling_g07_c01.avi 1

## Regenerating Splits
- Re-run the split script to regenerate train/val/test with desired ratios and seed.

## Notes
- dataset_info.txt is a JSON summary created by the split script.
- Paths in split files are relative to the dataset root.
