# PGC: Positional Geometric Calibration for Bounding Box Prediction in DETR-Based Object Detection

This repository provides the implementation of PGC.

## Overview

PGC is a plug-and-play decoder modification for DETR-style object detectors.
No other components of the original frameworks are modified.

## Modified Components

Compared to the official implementations, the only modification is the replacement of the decoder module with a PGC-enhanced version.

Core modified files:

- rtdetr_pytorch/src/zoo/rtdetr/rtdetr_decoder.py
- rtdetrv2_pytorch/src/zoo/rtdetr/rtdetrv2_decoder.py
- D-FINE/src/zoo/dfine/dfine_decoder.py

All other components remain identical to the original repositories.

## Base Implementations

The code is built upon the official implementations of:

- RT-DETR
- RT-DETRv2
- D-FINE

We follow the original training schedules and configurations unless otherwise specified in the paper.

## Reproducing Results

To reproduce the results:

1. Follow the installation instructions of the corresponding original repository.
2. Train with the default training schedule.

Exact training commands are provided in the corresponding subdirectories.
