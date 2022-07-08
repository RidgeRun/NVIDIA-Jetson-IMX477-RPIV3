# NVIDIA Jetson IMX477 HQ RPI V3 camera driver

This driver has been developed by NVIDIA Corporation, RidgeRun Engineering and Leopard Imaging Inc. as a collaborative initiative. The driver currently supports JetPack 5.0.1 Jetson Orin with Auvidea J20 adapter for triple cameras.

Supports the following Jetson platforms:
* Jetson Orin AGX with Auvidea J20

## Repository structure

In this repository you will find the following structure:
```
.
├── li-camera-calibration-files
│   └── camera_overrides.isp
├── patches_orin
│   ├── 5.0.1_agx_imx477_v0.1.patch
│   └── series
└── README.md
```
where:

* `5.0.1_agx_imx477_v0.1.patch` is the patch to be applied on the JetPack 5.0.1 Orin sources in order to add support for the IMX477 camera sensor + J20 adapter.
* `series` is a file containing the patch name in order to apply it by using the quilt tool.
* `camera_overrides.isp` is a file which contains a set of calibration parameters for the Image Signal Processor of the HQ camera.

## Installation instructions

You find the guide to use the driver [here](https://developer.ridgerun.com/wiki/index.php?title=NVIDIA_Jetson_Orin/Video_Capture_and_Display/Cameras/IMX477_J20)
