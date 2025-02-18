
# YOLOv7 for Pose Estimation

Pose estimation is an important task in computer vision, where the objective is to determine the positions of a person's body in an image or video. This can be used in various applications like augmented reality, human-computer interaction, sports analysis, and more.

## Why YOLOv7?

YOLOv7 is one of the latest advancements in the YOLO (You Only Look Once) family of models, optimized for speed and accuracy. It is well-suited for real-time applications and can perform both object detection and pose estimation efficiently.

### Key Features:
- **Real-Time Performance**: YOLOv7 allows for high-speed processing, making it ideal for applications requiring live feedback.
- **High Accuracy**: It has demonstrated high accuracy in detecting keypoints and poses, even in complex environments.
- **Single-Pass Detection**: The algorithm processes the input in one pass, reducing computational overhead and making it faster than multi-stage models.

## Advantages of Using YOLOv7 for Pose Estimation

- **Faster Processing**: YOLOv7's optimized architecture ensures that pose estimation can be performed in real time with minimal delay.
- **Accuracy and Precision**: It offers high accuracy in detecting multiple keypoints and body parts.
- **Scalability**: YOLOv7 can be used in a variety of tasks beyond pose estimation, such as object detection, making it highly versatile.


### Steps to Run Code


- **Clone the repository**:
  ```bash
  git clone https://github.com/RizwanMunawar/yolov7-pose-estimation.git
  ```
- **Go to the cloned folder**:
  ```bash
  cd yolov7-pose-estimation
  ```
- **Create a virtual environment** (recommended):
  ```bash
  # Linux
  python3 -m venv psestenv
  source psestenv/bin/activate

  # Windows
  python3 -m venv psestenv
  cd psestenv/Scripts
  activate

  #mac
  conda create --name <env_name> python=3.x
  conda activate <env_name>

  ```
- **Upgrade pip**:
  ```bash
  pip install --upgrade pip
  ```
- **Install requirements**:
  ```bash
  pip install -r requirements.txt
  ```
- **Download YOLOv7 weights** and move to the working directory:
  [yolov7-w6-pose.pt](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-w6-pose.pt)

- **Run the code**:
  ```bash
  python pose-estimate.py

  # Options:
  python pose-estimate.py --source "your-video.mp4" --device cpu  # For CPU
  python pose-estimate.py --source 0 --view-img  # For Webcam
  python pose-estimate.py --source "rtsp://your-ip" --device 0 --view-img  # For LiveStream
  ```

- Output: The processed video will be saved as **your-file-keypoint.mp4**

### RESULTS

<table>
  <tr>
    
  <td>Live Stream</td>
  </tr>
  <tr>
    
  <td><img src="https://user-images.githubusercontent.com/62513924/185587159-6643529c-7840-48d6-ae1d-2d7c27d417ab.png" width=300></td>
  </tr>
</table>

### References
- YOLOv7 Repo: https://github.com/WongKinYiu/yolov7
- Ultralytics: https://github.com/ultralytics/yolov5

### 📖 Articles
- [YOLOv7 Training Guide](https://medium.com/augmented-startups/yolov7-training-on-custom-data-b86d23e6623)
- [Computer Vision Roadmap](https://medium.com/augmented-startups/roadmap-for-computer-vision-engineer-45167b94518c)
