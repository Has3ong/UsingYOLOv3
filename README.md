# UsingYOLOv3

####Using Simple YOLOv3

<img width=600 src="https://user-images.githubusercontent.com/44635266/62702994-1cb8b700-ba23-11e9-9bd6-88d60bc48eaa.PNG">

### Step 1 - Settings
* Anaconda – Python 3.6 (Win 10) https://www.anaconda.com/download/
```
conda env create -f yolo.yml
```

If that does not work, try installing the dependencies with:
```
pip install -r requirements.txt
```
* CUDA Toolkit - V9.0 

* CuDNN - V 7.05

```
Copy the following files into the CUDA Toolkit directory.

Copy \cuda\bin\cudnn64_7.dll to C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v9.0\bin.

Copy \cuda\ include\cudnn.h to C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v9.0\include.

Copy \cuda\lib\x64\cudnn.lib to C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v9.0\lib\x64.

Add the following paths to Environmental Variables C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v9.0\bin

C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v9.0\include

C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v9.0\lib\x64
```

### Step 2 - PyTorch Yolo v3

* Clone Yolo v3 Repo
```
git clone https://github.com/ayooshkathuria/pytorch-yolo-v3.git
```
* Download the Weights, into pytorch-yolo-v3

🔗https://pjreddie.com/media/files/yolov3.weights

### Step 3 - PyTorch Yolo v3

```
cd pytorch-yolo-v3
```
Download any test video (.mp4/.avi)

Run demo on video
```
python video_demo.py --video video.mp4
```
Run demo on webcam
```
python cam_demo.py
```