# Face_Detection

**Face_Detection** is a Python project for analyzing facial symmetry using facial landmark detection. It includes scripts to evaluate symmetry for various facial features, leveraging a pre-trained model to compute and visualize symmetry on face images.

## Features

- Facial landmark detection with `shape_predictor_68_face_landmarks.dat`
- Symmetry analysis for:
  - Cheeks
  - Dental structure
  - Eyes
  - Frontal face
  - Horizontal axis
  - Vertical axis
  - Smile
  - Eyebrows
- Visualization of symmetry and asymmetry on images
- Modular utility functions for landmark processing

## Repository Structure

| File/Folder                          | Description                                      |
|--------------------------------------|--------------------------------------------------|
| `Cheeks_symetrie.py`                 | Cheek symmetry analysis script                   |
| `Dental_symetrie.py`                 | Dental symmetry analysis script                  |
| `Eye_symetrie.py`                    | Eye symmetry analysis script                     |
| `Frontal_symetrie.py`                | Frontal face symmetry analysis script            |
| `Horizontal_symetrie.py`             | Horizontal axis symmetry analysis script         |
| `Smile_symetrie.py`                  | Smile symmetry analysis script                   |
| `Vertical_symetrie.py`               | Vertical axis symmetry analysis script           |
| `eyebrow_symetrie.py`                | Eyebrow symmetry analysis script                 |
| `function.py`                        | Utility functions for landmark processing        |
| `shape_predictor_68_face_landmarks.dat` | Pre-trained facial landmark model           |
| `SYM.png`, `ASYM.png`                | Example output images                            |
| `.gitignore`                         | Git ignore file                                  |

## Requirements

- Python 3.x
- dlib
- OpenCV (`cv2`)
- numpy

Install dependencies:

```sh
pip install dlib opencv-python numpy 
```


## Usage

1. Ensure `shape_predictor_68_face_landmarks.dat` is present in the repository.
2. Run a symmetry analysis script. For example, to analyze eye symmetry:

```sh
python Eye_symetrie.py
```


3. The script will process the input image, perform landmark detection, compute symmetry, and save or display the annotated result.

## Notes

- Each script focuses on a specific facial feature.
- Scripts can be adapted or combined for custom analyses.
- Output images (`SYM.png`, `ASYM.png`) demonstrate typical results.