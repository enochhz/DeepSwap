# deepfakes_faceswap

Faceswap is a tool that utilizes deep learning to recognize and swap faces in pictures and videos.
![Screenshots](https://i.imgur.com/nWHFLDf.jpg)

Make sure you check out [INSTALL.md](INSTALL.md) before getting started.

- [How To setup and run the project](#how-to-setup-and-run-the-project)
  - [Overview](#overview)
  - [Extract](#extract)
  - [Train](#train)
  - [Convert](#convert)
  - [GUI](#gui)
  - [General notes:](#general-notes)
---
## How To setup and run the project
Faceswap is a Python program that will run on multiple Operating Systems including Windows, Linux and MacOS.

See [INSTALL.md](INSTALL.md) for full installation instructions. You will need a modern GPU with CUDA support for best performance.

## Overview
The project has multiple entry points. You will have to:
 - Gather photos (or use the one provided in the training data provided below)
 - **Extract** faces from your raw photos
 - **Train** a model on your photos (or use the one provided in the training data provided below)
 - **Convert** your sources with the model

Check out [USAGE.md](USAGE.md) for more detailed instructions.

### Extract
From your setup folder, run `python faceswap.py extract`. This will take photos from `src` folder and extract faces into `extract` folder.

### Train
From your setup folder, run `python faceswap.py train`. This will take photos from two folders containing pictures of both faces and train a model that will be saved inside the `models` folder.

### Convert
From your setup folder, run `python faceswap.py convert`. This will take photos from `original` folder and apply new faces into `modified` folder.

### GUI
Alternatively you can run the GUI by running `python faceswap.py gui`
