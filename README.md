# Volleyball-Detector

 Hi my name is Shailoh Arias.For my final project on the Jetson Nano, and for my final project I decided to make a volleyball detector. The point of the project is to help coaches or players to train better.  

![add image descrition here](direct image link here)

## The Algorithm
This project uses a condensed version of [this](https://universe.roboflow.com/wenxuans-workspace/volleyball-7yzmq/dataset/3) volleyball object-detection dataset from Roboflow. The model was trained on 1092 images.

- `cd jetson-inference`
- `./docker/run.sh`
- `cd  python/training/detection/ssd`
- `python3 train_ssd.py --data=data/rf_volleyball --model-dir=models/rf_model --batch-size=4 --epochs=30`
This is how i trained my model


## Running this project

1. Add steps for running this project.
2. Make sure to include any required libraries that need to be installed for your project to run.

[View a video explanation here](video link)
