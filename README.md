# Object detection using nvidia-jetson-nano

## Team Members
- Aniket Choudhari (CS22B1010, GitHub:[Aniket-Choudhari-01](https://github.com/Aniket-Choudhari-01))
- Aditya Kumar Singh (CS22B1001, GitHub:[Adityacse1001](https://github.com/Adityacse1001/Adityacse1001))

## Overview
This project implements an object detection system on the Jetson Nano, leveraging NVIDIA's powerful edge computing capabilities. The system utilizes deep learning models to detect and classify objects in real-time from video streams or images. The project demonstrates the setup and optimization of the Jetson Nano for high-performance inference, making it suitable for various applications such as surveillance, robotics, and smart devices.This projects used for pre tained model of nvidia and used jetson nano for performance measure.

## Details
[Link](https://developer.nvidia.com/blog/realtime-object-detection-in-10-lines-of-python-on-jetson-nano/) to the given open source project of nvidia.

## Steps
1. Ensure your Jetson Nano is properly set up with the JetPack SDK, which includes TensorRT, CUDA, and cuDNN. Follow the official [guide](https://developer.nvidia.com/embedded/jetpack) to set up your Jetson Nano.
2. Open Terminal in jetson nano and set up the Jetson Infernece usig the below given Instruction 
```bash
# Clone the repository
git clone https://github.com/dusty-nv/jetson-inference.git

# Navigate to the project directory
cd jetson-inference

# Create a build directory
mkdir build
cd build

# Configure and build the project
cmake ..
make

# Install the library
sudo make install
sudo ldconfig
```
3. After setting up the environment now execute the command in the terminal for detection the objects in the real time
```python
python3 detectnet.py /dev/video0 images/test/output.mp4
```
## Results
#### Object detection using webcam streaming:

![video_Result](https://github.com/user-attachments/assets/cd6cf987-53db-46e3-8183-df13ef73a0df)
![Video2_Result](https://github.com/user-attachments/assets/aa8c2ebc-321d-459c-9b1a-2a870ba0e7f7)
#### Detecting Students in the Mess:
![live_video_result](https://github.com/user-attachments/assets/53493309-4e18-4b7e-ae3d-d401f444a33b)

