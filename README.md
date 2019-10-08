# NEAR: The NetEase AR Oriented Visual Inertial Dataset

## Abstract

The existing datasets for evaluating Visual Inertial Odometry (VIO) have boosted the research of autonomous agents, but they don’t meet the prosperous research of Augmented Reality (AR) or Mixed Reality (MR) given that they are not collected at real AR scenes and do not account for affecting factors of mobile devices. This paper presents the NEAR dataset, an AR oriented visual-inertial dataset collected with commodity handheld phones with ground truth. The dataset has a total of 110 sequences in 49 elaborately designed collection cases at two typical indoor scenes, i.e. the living area and the table area. It also covers plenty of setting adjustments for comparison, including the comparisons of different level textures, illuminations, motion patterns, camera settings and the difference between the rolling shutter and the global shutter. The full dataset along with the calibration data has been publicly available [here](http://beidou.s.cn.vc/Supplier).

## Download dataset

NEAR dataset has been publicly available [here](http://beidou.s.cn.vc/Supplier).

## Case design

[CaseTableEva.xlsx](CaseTableEva.xlsx) presents all the cases designed on our dataset.

| case | environment | scene                                    | lighting              | motion pattern                      | special device setting | devices               | preview                          |
| ---- | ----------- | ---------------------------------------- | --------------------- | ----------------------------------- | ---------------------- | --------------------- | -------------------------------- |
| 1    | Easy\[1\]   | Rich\-textured desktop                   | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone 7, Huawei P20  | [001.gif](./preview_gif/001.gif) |
| 2    | Easy        | Rich\-textured desktop                   | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 3    | Easy        | Rich\-textured desktop                   | uniform & stable      | circle \(alwayse points to center\) | default                | iPhone 7, Huawei P20  |                                  |
| 4    | Easy        | Medium\-textured desktop                 | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone 7, Huawei P20  |                                  |
| 5    | Easy        | Medium\-textured desktop                 | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 6    | Easy        | Medium\-textured desktop with reflection | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone 7, Huawei P20  |                                  |
| 7    | Easy        | Medium\-textured desktop with reflection | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 8    | Easy        | Rich\-textured livingroom                | uniform & stable      | translation \(slow\+normal\)        | default                | iPhone 7, Huawei P20  |                                  |
| 9    | Easy        | Rich\-textured livingroom                | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone XR, OnePlus 5T |                                  |
| 10   | Easy        | Rich\-textured livingroom                | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T |                                  |
| 11   | Easy        | Rich\-textured livingroom                | uniform & stable      | user scan simulation                | default                | iPhone XR, OnePlus 5T |                                  |
| 12   | Normal\[2\] | Rich\-textured desktop                   | uniform & stable      | circle \(slow\+normal\+fast\)       | default                | iPhone XR, OnePlus 5T |                                  |
| 13   | Normal      | Rich\-textured desktop                   | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T |                                  |
| 14   | Normal      | Rich\-textured desktop                   | uniform & stable      | free                                | default                | iPhone XR, OnePlus 5T |                                  |
| 15   | Normal      | Rich\-textured desktop                   | uniform & stable      | game simulation \(YuMe\)            | default                | iPhone XR, OnePlus 5T |                                  |
| 16   | Normal      | Medium\-textured desktop                 | uniform & stable      | circle \(slow\+normal\+fast\)       | default                | iPhone XR, OnePlus 5T |                                  |
| 17   | Normal      | Medium\-textured desktop                 | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T |                                  |
| 18   | Normal      | Medium\-textured desktop                 | uniform & stable      | free                                | default                | iPhone XR, OnePlus 5T |                                  |
| 19   | Normal      | Medium\-textured desktop                 | uniform & stable      | game simulation \(YuMe\)            | default                | iPhone XR, OnePlus 5T |                                  |
| 20   | Normal      | Medium\-textured desktop                 | dynamic               | circle \(slow\+normal\+fast\)       | default                | iPhone XR, OnePlus 5T |                                  |
| 21   | Normal      | Medium\-textured desktop                 | dynamic               | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 22   | Normal      | Medium\-textured desktop                 | dynamic               | free                                | default                | iPhone 7, Huawei P20  |                                  |
| 23   | Normal      | Medium\-textured desktop with reflection | uniform & stable      | circle \(slow\+normal\+fast\)       | default                | iPhone 7, Huawei P20  |                                  |
| 24   | Normal      | Medium\-textured desktop with reflection | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 25   | Normal      | Medium\-textured desktop with reflection | uniform & stable      | free                                | default                | iPhone 7, Huawei P20  |                                  |
| 26   | Normal      | Median\-textured livingroom              | uniform & stable      | translation \(slow\+normal\+fast\)  | default                | iPhone 7, Huawei P20  |                                  |
| 27   | Normal      | Median\-textured livingroom              | uniform & stable      | translation \(slow\+normal\+fast\)  | 30fps                  | iPhone 7, Huawei P20  |                                  |
| 28   | Normal      | Median\-textured livingroom              | uniform & stable      | translation \(slow\+normal\+fast\)  | autofocus              | iPhone 7, Huawei P20  |                                  |
| 29   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(slow\)                     | default                | iPhone XR, OnePlus 5T |                                  |
| 30   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(normal\)                   | default                | iPhone XR, OnePlus 5T |                                  |
| 31   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(fast\)                     | default                | iPhone XR, OnePlus 5T |                                  |
| 32   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(normal\)                   | 30fps                  | iPhone XR, OnePlus 5T |                                  |
| 33   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(normal\)                   | autofocus              | iPhone XR, OnePlus 5T |                                  |
| 34   | Normal      | Median\-textured livingroom              | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T |                                  |
| 35   | Normal      | Median\-textured livingroom              | uniform & stable      | hybrid                              | 30fps                  | iPhone XR, OnePlus 5T |                                  |
| 36   | Normal      | Median\-textured livingroom              | uniform & stable      | hybrid                              | autofocus              | iPhone XR, OnePlus 5T |                                  |
| 37   | Normal      | Median\-textured livingroom              | uniform & stable      | free                                | default                | iPhone XR, OnePlus 5T |                                  |
| 38   | Normal      | Median\-textured livingroom              | uniform & stable      | user scan simulation                | default                | iPhone XR, OnePlus 5T |                                  |
| 39   | Normal      | Median\-textured livingroom              | uniform & stable      | game simulation \(Shot\)            | default                | iPhone 7, Huawei P20  |                                  |
| 40   | Normal      | textureless floor and furnitures         | uniform & stable      | translation \(slow\+normal\+fast\)  | default                | iPhone 7, Huawei P20  |                                  |
| 41   | Normal      | textureless floor and furnitures         | uniform & stable      | circle \(slow\)                     | default                | iPhone 7, Huawei P20  |                                  |
| 42   | Normal      | textureless floor and furnitures         | uniform & stable      | circle \(normal\)                   | default                | iPhone 7, Huawei P20  |                                  |
| 43   | Normal      | textureless floor and furnitures         | uniform & stable      | circle \(fast\)                     | default                | iPhone 7, Huawei P20  |                                  |
| 44   | Normal      | textureless floor and furnitures         | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 45   | Normal      | textureless floor and furnitures         | uniform & stable      | free                                | default                | iPhone 7, Huawei P20  |                                  |
| 46   | Hard\[3\]   | Rich\-textured desktop                   | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 48   | Hard        | Medium\-textured desktop                 | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 50   | Hard        | Medium\-textured desktop with reflection | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |
| 52   | Hard        | textureless floor and furnitures         | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  |                                  |

## Dataset structure

The sequences are organized following the structure of widely used EuRoC:

```
./Case ID
│
└───ip7                                         A folder with phone name.
     └───P_lp2lv.txt                            The extrinsic between phone camera and rigid body.
     └───rts_compensate_extrinsic_and_time.txt  The ground truth trajectory (TUM format) of camera frame.
     └───timeoffset.txt                         Timestamp offset between phone camera and RTS system.
     │
     └───mav0
          │
          └───cam0
          │    └───data                         The folder contains image sequence.
          │    └───cam.yaml                     Camera settings when record this sequence.
          │    └───data.csv                     Timestamps of camera frames.
          │    └───sensor.csv                   Camera intrinsics and camera-IMU extrinsic.
          └───imu0
                └───data.csv                    Timestamps and IMU measurements.
                └───sensor.yaml                 IMU intrinsics and IMU-rig extrinsic which is identity.
```

## Preview video

Considering the limited storage space, we made the preview videos in very low resolution and we speed them up. We post all the preview videos [NEAR-dataset-preview-video](https://www.youtube.com/channel/UCD89MMVLJYi9ZqWKdwmGpaQ/playlists?view_as=subscriber).
