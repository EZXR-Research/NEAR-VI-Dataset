# NEAR: The NetEase AR Oriented Visual Inertial Dataset

## Abstract

The existing datasets for evaluating Visual Inertial Odometry (VIO) have boosted the research of autonomous agents, but they don’t meet the prosperous research of Augmented Reality (AR) or Mixed Reality (MR) given that they are not collected at real AR scenes and do not account for affecting factors of mobile devices. This paper presents the NEAR dataset, an AR oriented visual-inertial dataset collected with commodity handheld phones with ground truth. The dataset has a total of 110 sequences in 49 elaborately designed collection cases at two typical indoor scenes, i.e. the living area and the table area. It also covers plenty of setting adjustments for comparison, including the comparisons of different level textures, illuminations, motion patterns, camera settings and the difference between the rolling shutter and the global shutter. The full dataset along with the calibration data has been publicly available [here](http://beidou.s.cn.vc/Supplier).

## Download dataset

NEAR dataset has been publicly available [here](http://beidou.s.cn.vc/Supplier).

## Case design

[CaseTableEva.xlsx](CaseTableEva.xlsx) presents all the cases designed on our dataset.

| case | environment | scene                                    | lighting              | motion pattern                      | special device setting | devices               | preview                          |
| ---- | ----------- | ---------------------------------------- | --------------------- | ----------------------------------- | ---------------------- | --------------------- | -------------------------------- |
| 1    | Easy\[1\]   | Rich\-textured desktop                   | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone 7, Huawei P20  | ![001.gif](./preview_gif/001.gif) |
| 2    | Easy        | Rich\-textured desktop                   | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  | ![002.gif](./preview_gif/002.gif)|
| 2_control    | Easy        | Rich\-textured desktop                   | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20, MYNT | ![002.gif](./preview_gif/002_mynt.gif)|
| 3    | Easy        | Rich\-textured desktop                   | uniform & stable      | circle \(alwayse points to center\) | default                | iPhone 7, Huawei P20  | ![003.gif](./preview_gif/003.gif) |
| 3_control    | Easy        | Rich\-textured desktop                   | uniform & stable      | circle \(alwayse points to center\) | default                | iPhone 7, Huawei P20, MYNT  | ![003.gif](./preview_gif/003_mynt.gif) |
| 4    | Easy        | Medium\-textured desktop                 | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone 7, Huawei P20  | ![004.gif](./preview_gif/004.gif) |
| 5    | Easy        | Medium\-textured desktop                 | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  | ![005.gif](./preview_gif/005.gif) |
| 6    | Easy        | Medium\-textured desktop with reflection | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone 7, Huawei P20  | ![006.gif](./preview_gif/006.gif)|
| 7    | Easy        | Medium\-textured desktop with reflection | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  | ![007.gif](./preview_gif/007.gif) |
| 8    | Easy        | Rich\-textured livingroom                | uniform & stable      | translation \(slow\+normal\)        | default                | iPhone 7, Huawei P20  | ![008.gif](./preview_gif/008.gif) |
| 9    | Easy        | Rich\-textured livingroom                | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone XR, OnePlus 5T | ![009.gif](./preview_gif/009_2.gif) |
| 9_control    | Easy        | Rich\-textured livingroom                | uniform & stable      | circle \(slow\+normal\)             | default                | iPhone XR, OnePlus 5T, MYNT | ![009.gif](./preview_gif/009_mynt.gif) |
| 10   | Easy        | Rich\-textured livingroom                | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T | ![010.gif](./preview_gif/010.gif) |
| 10_control   | Easy        | Rich\-textured livingroom                | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T, MYNT | ![010.gif](./preview_gif/010_mynt.gif) |
| 11   | Easy        | Rich\-textured livingroom                | uniform & stable      | user scan simulation                | default                | iPhone XR, OnePlus 5T | ![011.gif](./preview_gif/011.gif) |
| 11_control   | Easy        | Rich\-textured livingroom                | uniform & stable      | user scan simulation                | default                | iPhone XR, OnePlus 5T, MYNT | ![011.gif](./preview_gif/011_mynt.gif) |
| 12   | Normal\[2\] | Rich\-textured desktop                   | uniform & stable      | circle \(slow\+normal\+fast\)       | default                | iPhone XR, OnePlus 5T | ![012.gif](./preview_gif/012_2.gif) |
| 13   | Normal      | Rich\-textured desktop                   | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T | ![013.gif](./preview_gif/013.gif) |
| 14   | Normal      | Rich\-textured desktop                   | uniform & stable      | free                                | default                | iPhone XR, OnePlus 5T | ![014.gif](./preview_gif/014.gif) |
| 15   | Normal      | Rich\-textured desktop                   | uniform & stable      | game simulation \(YuMe\)            | default                | iPhone XR, OnePlus 5T | ![015.gif](./preview_gif/015.gif) |
| 16   | Normal      | Medium\-textured desktop                 | uniform & stable      | circle \(slow\+normal\+fast\)       | default                | iPhone XR, OnePlus 5T | ![016.gif](./preview_gif/016_2.gif) |
| 17   | Normal      | Medium\-textured desktop                 | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T | ![017.gif](./preview_gif/017_2.gif) |
| 18   | Normal      | Medium\-textured desktop                 | uniform & stable      | free                                | default                | iPhone XR, OnePlus 5T | ![018.gif](./preview_gif/018_2.gif) |
| 19   | Normal      | Medium\-textured desktop                 | uniform & stable      | game simulation \(YuMe\)            | default                | iPhone XR, OnePlus 5T | ![019.gif](./preview_gif/019.gif) |
| 20   | Normal      | Medium\-textured desktop                 | dynamic               | circle \(slow\+normal\+fast\)       | default                | iPhone XR, OnePlus 5T | ![020.gif](./preview_gif/020.gif) |
| 21   | Normal      | Medium\-textured desktop                 | dynamic               | hybrid                              | default                | iPhone 7, Huawei P20  | ![021.gif](./preview_gif/021.gif) |
| 22   | Normal      | Medium\-textured desktop                 | dynamic               | free                                | default                | iPhone 7, Huawei P20  | ![022.gif](./preview_gif/022.gif) |
| 23   | Normal      | Medium\-textured desktop with reflection | uniform & stable      | circle \(slow\+normal\+fast\)       | default                | iPhone 7, Huawei P20  | ![023.gif](./preview_gif/023.gif) |
| 24   | Normal      | Medium\-textured desktop with reflection | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  | ![024.gif](./preview_gif/024.gif) |
| 25   | Normal      | Medium\-textured desktop with reflection | uniform & stable      | free                                | default                | iPhone 7, Huawei P20  | ![025.gif](./preview_gif/025.gif) |
| 26   | Normal      | Median\-textured livingroom              | uniform & stable      | translation \(slow\+normal\+fast\)  | default                | iPhone 7, Huawei P20  | ![026.gif](./preview_gif/026.gif) |
| 27   | Normal      | Median\-textured livingroom              | uniform & stable      | translation \(slow\+normal\+fast\)  | 30fps                  | iPhone 7, Huawei P20  | ![027.gif](./preview_gif/027.gif) |
| 28   | Normal      | Median\-textured livingroom              | uniform & stable      | translation \(slow\+normal\+fast\)  | autofocus              | iPhone 7, Huawei P20  | ![028.gif](./preview_gif/028.gif) |
| 29   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(slow\)                     | default                | iPhone XR, OnePlus 5T | ![029.gif](./preview_gif/029_2.gif) |
| 30   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(normal\)                   | default                | iPhone XR, OnePlus 5T | ![030.gif](./preview_gif/030_2.gif) |
| 31   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(fast\)                     | default                | iPhone XR, OnePlus 5T | ![031.gif](./preview_gif/031.gif) |
| 32   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(normal\)                   | 30fps                  | iPhone XR, OnePlus 5T | ![032.gif](./preview_gif/032_2.gif) |
| 33   | Normal      | Median\-textured livingroom              | uniform & stable      | circle \(normal\)                   | autofocus              | iPhone XR, OnePlus 5T | ![033.gif](./preview_gif/033.gif) |
| 34   | Normal      | Median\-textured livingroom              | uniform & stable      | hybrid                              | default                | iPhone XR, OnePlus 5T | ![034.gif](./preview_gif/034.gif) |
| 35   | Normal      | Median\-textured livingroom              | uniform & stable      | hybrid                              | 30fps                  | iPhone XR, OnePlus 5T | ![035.gif](./preview_gif/035.gif) |
| 36   | Normal      | Median\-textured livingroom              | uniform & stable      | hybrid                              | autofocus              | iPhone XR, OnePlus 5T | ![036.gif](./preview_gif/036_2.gif) |
| 37   | Normal      | Median\-textured livingroom              | uniform & stable      | free                                | default                | iPhone XR, OnePlus 5T | ![037.gif](./preview_gif/037.gif) |
| 38   | Normal      | Median\-textured livingroom              | uniform & stable      | user scan simulation                | default                | iPhone XR, OnePlus 5T | ![038.gif](./preview_gif/038.gif) |
| 39   | Normal      | Median\-textured livingroom              | uniform & stable      | game simulation \(Shot\)            | default                | iPhone 7, Huawei P20  | ![039.gif](./preview_gif/039.gif) |
| 40   | Normal      | textureless floor and furnitures         | uniform & stable      | translation \(slow\+normal\+fast\)  | default                | iPhone 7, Huawei P20  | ![040.gif](./preview_gif/040.gif) |
| 41   | Normal      | textureless floor and furnitures         | uniform & stable      | circle \(slow\)                     | default                | iPhone 7, Huawei P20  | ![041.gif](./preview_gif/041.gif) |
| 42   | Normal      | textureless floor and furnitures         | uniform & stable      | circle \(normal\)                   | default                | iPhone 7, Huawei P20  | ![042.gif](./preview_gif/042.gif) |
| 43   | Normal      | textureless floor and furnitures         | uniform & stable      | circle \(fast\)                     | default                | iPhone 7, Huawei P20  | ![043.gif](./preview_gif/043.gif) |
| 44   | Normal      | textureless floor and furnitures         | uniform & stable      | hybrid                              | default                | iPhone 7, Huawei P20  | ![044.gif](./preview_gif/044.gif) |
| 45   | Normal      | textureless floor and furnitures         | uniform & stable      | free                                | default                | iPhone 7, Huawei P20  | ![045.gif](./preview_gif/045.gif) |
| 46   | Hard\[3\]   | Rich\-textured desktop                   | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  | ![046.gif](./preview_gif/046.gif) |
| 48   | Hard        | Medium\-textured desktop                 | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  | ![048.gif](./preview_gif/048.gif) |
| 50   | Hard        | Medium\-textured desktop with reflection | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  | ![050.gif](./preview_gif/050.gif) |
| 52   | Hard        | textureless floor and furnitures         | non\-uniform & stable | hybrid                              | default                | iPhone 7, Huawei P20  | ![052.gif](./preview_gif/052.gif) |

notes: 
1. "Easy" means  no repetitive texture, no reflection, no opened windows. Rich-textured carpets, sofas and walls.
2. "Normal" means a common livingroom settings. Median-textured carpets, sofas and walls. Some opened windows and a mirror.
3. "Hard" means Opened windows, mirrors, textureless floor, textureless furnitures, textureless walls, lamps.

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
​						

## Preview video

Considering the limited storage space, we made the preview videos in very low resolution and we speed them up. We post all the preview videos [NEAR-dataset-preview-video](https://www.youtube.com/channel/UCD89MMVLJYi9ZqWKdwmGpaQ/playlists?view_as=subscriber).
