# Volleyball-Detector

 Hi my name is Shailoh Arias.For my final project on the Jetson Nano, and for my final project I decided to make a volleyball detector. The point of the project is to help coaches or players to train better.  

![add image descrition here](direct image link here)

## The Algorithm
This project uses a condensed version of [this](https://universe.roboflow.com/wenxuans-workspace/volleyball-7yzmq/dataset/3) volleyball object-detection dataset from Roboflow. The model was trained on 1092 images.

- `cd jetson-inference`
- `./docker/run.sh`
- `cd  python/training/detection/ssd`
- `python3 train_ssd.py --data=data/rf_volleyball --model-dir=models/rf_model --batch-size=4 --epochs=30`


## Running this project
Clone the project repo
`git clone https://github.com/shailoharias/Volleyball-Detector.git`
Change into the project folder
- `cd Volleyball-Detector`

Set the network variable
-`NET=model`

Run this command to test on a live recording:
-`detectnet  --model=$NET/ssd-mobilenet.onnx  --labels=$NET/labels.txt     --input-blob=input_0  --output-cvg=scores  --output-bbox=boxes      /dev/video0 output.mp4`


[View a video explanation here](video link)
