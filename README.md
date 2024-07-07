# Helmet Detection Project

## Overview
This project focuses on detecting helmets, heads, and persons using a finetuned version of YOLOv10. The aim is to enhance safety measures by accurately identifying whether individuals are wearing helmets in various environments.

## Features
- **Helmet Detection**: Identify if a person is wearing a helmet.
- **Head Detection**: Detect the presence of a person's head.
- **Person Detection**: Detect and locate persons in the frame.

## Dataset
The dataset used for training the model consists of annotated images containing helmets, heads, and persons.

## Installation
To run this project, you need to have Python and the required dependencies installed.

1. Clone this repository:
    ```bash
    git clone https://github.com/hiephoangt/HelmetDetection.git
    cd HelmetDetection
    ```

2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Training
To finetune the YOLOv10 model with your dataset, follow these steps:

1. Prepare your dataset and place it in the `data/` directory.
2. Update the configuration file with your dataset details.
3. Run the training script:
    ```bash
    python train.py --config config.yaml
    ```

## Inference
To run inference with the trained model:

1. Place the images you want to test in the `images/` directory.
2. Run the inference script:
    ```bash
    python detect.py --source images/
    ```

## Results
The results of the detection will be saved in the `output/` directory with bounding boxes around detected helmets, heads, and persons.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License.

## Acknowledgements
- The YOLOv10 team for their powerful object detection framework.
- Contributors and the open-source community for their invaluable work.

