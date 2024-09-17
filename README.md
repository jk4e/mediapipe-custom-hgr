# MediaPipe Custom Hand Gesture Recognition Model

A collection of Jupyter Notebooks for training, evaluation, and visualization of MediaPipe Gesture Recognition Tasks. The MediaPipe Gesture Recognizer task enables real-time hand gesture recognition, providing recognized hand gesture results along with landmarks of detected hands. You can customize your own gesture recognition models using MediaPipe Model Maker and train them on your own datasets.

## Notebooks

### `mp_hgr_model_maker.ipynb`

A notebook for training a custom model locally. Includes an easy-to-follow, step-by-step guide to train your first model. Learn how to train a custom model with your own dataset.

### `mp_hgr_3d_visualisation.ipynb`

An interactive 3D visualization of hand landmarks (keypoints). Simply drop an image of a hand, and the notebook will return an interactive 3D plot of the extracted hand landmarks.

### `mp_hgr_model_evaluation.ipynb`

An advanced evaluation notebook to better understand your trained model and identify areas for improvement in model accuracy.

## Getting Started

### Prerequisites
- Git
- conda-forge, Miniconda or Anaconda (recommended for beginners)

### Setup Instructions

1. Clone this repository:
   ```
   git clone https://github.com/jk4e/mediapipe-custom-hgr.git
   cd mediapipe-custom-hgr
   ```

2. Set up a conda environment:
   ```
   conda create --name mp_hgr_env python=3.11 pip
   conda activate mp_hgr_env
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Launch Jupyter Lab or Jupyter Notebook:
   ```
   jupyter lab
   ```

5. Open the desired notebook and follow the instructions within each notebook.

### Troubleshooting
- Make sure your conda environment is activated before running any commands.
- For more information on conda environments, visit the [conda documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).



## Requirements

- Python 3.10+
- Jupyter Notebook or Jupyter Lab (Jupyter Extension for Visual Studio Code)
- see `requirements.txt`

## MediaPipe Gesture Recognition

- [Gesture recognition task guide](https://ai.google.dev/edge/mediapipe/solutions/vision/gesture_recognizer)
- [Hand gesture recognition model customization guide](https://ai.google.dev/edge/mediapipe/solutions/customization/gesture_recognizer)

### ⚠️ Important Note on MediaPipe Model Maker Installation

As of August 2024:

- The latest version of [MediaPipe Model Maker](https://pypi.org/project/mediapipe-model-maker/) (current version 0.2.1.4) cannot be installed on Windows or Silicon-based macOS.
- For more details, see issues: [How to install mediapipe_model_maker 0.2.1.4 in Windows? #5545](https://github.com/google-ai-edge/mediapipe/issues/5545) or [ Windows Support #1206 ](https://github.com/tensorflow/text/issues/1206)

#### Workarounds:

1. Use a machine with Linux
2. Set up WSL2 (Windows Subsystem for Linux) on a Windows machine
   - See [Install WSL](https://learn.microsoft.com/en-us/windows/wsl/install) for instructions
3. Use Google Colab, a free cloud-based Jupyter notebook environment
   - Google Colab provides access to GPU resources and pre-installed libraries

#### When is MediaPipe Model Maker needed?

- This package is required if you want to train custom models with your own dataset.
- If you don't need to train or customize a model, you can simply install the [MediaPipe package](https://pypi.org/project/mediapipe/)
  - See the [Guide for Python](https://ai.google.dev/edge/mediapipe/solutions/setup_python) for installation instructions.
  - So if you run `pip install -r requirements.txt`, first edit the `requirements.txt` and remove `mediapipe-model-maker` from the install list.


## Related Notebooks/Code examples:

- [Code example: Gesture Recognizer with MediaPipe Tasks](https://colab.research.google.com/github/googlesamples/mediapipe/blob/main/examples/gesture_recognizer/python/gesture_recognizer.ipynb#scrollTo=L_cQX8dWu4Dv) (Run in Colab)
- [Hand gesture recognition model customization guide](https://ai.google.dev/edge/mediapipe/solutions/customization/gesture_recognizer) (Run in Colab)


## Related Repository:

- [Custom Hand Gesture Recognition Models (HGR)🖐️ with YOLOv8🚀 and MediaPipe👋 - Streamlit App](https://github.com/jk4e/my-hgr): Streamlit app with MediaPipe and Ultralytics YOLOv8 hand gesture recognition (HGR) demos using custom trained models.
- [Hands Model Zoo](https://github.com/jk4e/hands-model-zoo): A collection of pretrained models for hand gesture recognition (HGR) tasks.


## Helpful Resources

- [Customizing a gesture recognition model with MediaPipe](https://www.samproell.io/posts/ai/asl-detector-with-mediapipe-wsl/)


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Disclaimer

This project is for educational purposes only.