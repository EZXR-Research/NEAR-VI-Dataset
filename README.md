# NEAR: The NetEase AR Oriented Visual Inertial Dataset

## Abstract

The existing datasets for evaluating Visual Inertial Odometry (VIO) have boosted the research of autonomous agents, but they don’t meet the prosperous research of Augmented Reality (AR) or Mixed Reality (MR) given that they are not collected at real AR scenes and do not account for affecting factors of mobile devices. This paper presents the NEAR dataset, an AR oriented visual-inertial dataset collected with commodity handheld phones with ground truth. The dataset has a total of 110 sequences in 49 elaborately designed collection cases at two typical indoor scenes, i.e. the living area and the table area. It also covers plenty of setting adjustments for comparison, including the comparisons of different level textures, illuminations, motion patterns, camera settings and the difference between the rolling shutter and the global shutter. The full dataset along with the calibration data has been publicly available [here](http://beidou.s.cn.vc/Supplier).

## Download dataset

NEAR dataset has been publicly available [here](http://beidou.s.cn.vc/Supplier).

## Case design

[CaseTableEva.xlsx](CaseTableEva.xlsx) presents all the cases designed on our dataset.

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
