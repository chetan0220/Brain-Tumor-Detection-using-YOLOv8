# Brain Tumor Detection using YOLOv8
In this project we have used different sizes of the YOLOv8 model to detect ansd classsify brain tumor in the MRI images
## Dataset 
[Link To Dataset](https://www.kaggle.com/datasets/ammarahmed310/labeled-mri-brain-tumor-dataset)
Dataset was obtained from Kaggle. It contains 2176 samples of various clinical circumstances. There 455 samples of "glioma", 551 samples of "meningiomas", 620 samples of "pituitary" and 550 samples of "No Tumor". 
## Training 

Training was done on nano and medium size of YOLOv8 model. The training process was optimised with various choice of Optimizers like Adam, Adamax and RMSprop. 
Following are the training parameters and results. 
| **Sr No** | **Size** | **Epochs** | **Batch Size** | **Learning Rate** | **Optimizer** | **Momentum** | **Dropout** | **Precision** | **Recall** |
|:---------:|:--------:|:----------:|:--------------:|:-----------------:|:-------------:|:------------:|:-----------:|:-------------:|:----------:|
|     1     |   Nano   |     25     |       109      |        0.01       |      Auto     |       -      |      -      |      90.1     |    79.1    |
|     2     |   Nano   |     30     |       32       |       0.001       |     Adamax    |     0.85     |     0.5     |      84.5     |    80.6    |
|     3     |  Medium  |     30     |       32       |       0.001       |    RMSprop    |     0.90     |     0.2     |      54.7     |    48.5    |
|     4     |  Medium  |     30     |       32       |       0.001       |      Adam     |     0.90     |     0.3     |      84.4     |    84.7    |
|     5     |  Medium  |     30     |       32       |       0.001       |     Adamax    |     0.89     |     0.4     |      89.9     |    86.5    |
## Results
1. Nano model with Auto Optimizer
![PR_curve](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/2bc4fa5e-381a-4b19-913f-7da4b6477f06) <br>

![image](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/5ce90e66-372c-4ee3-9640-fb29aad7e308)<br>

2. Nano model with Adamax Optimizer
![PR_curve (1)](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/79075a41-187c-48e4-9c37-367bdfef7336)<br>

![image](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/d915b016-d80a-4096-8e3f-edaff20c107b)<br>

3. Medium model with RMSprop Optimizer<br>
![PR_curve (2)](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/16e68aee-ed3d-4d55-bacc-fd5d2ec1616c)<br>

![image](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/2f2ab826-5449-412e-b92b-599b72a498f5)<br>

4. Medium model with Adam Optimizer
![PR_curve (3)](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/e89a369f-8155-4743-8a6f-ffd2d88fed7c)<br>

![image](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/f3f42569-c9c8-4882-85ac-2d79946b5944)<br>

5. Medium model with Adamax Optimizer
![PR_curve (4)](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/5ce1e550-a557-44dd-b8fb-88ed7bc1984f)<br>

![image](https://github.com/chetan0220/Brain-Tumor-Detection-using-YOLOv8/assets/97821311/aa5856e0-2633-42e4-a04e-78aa806f4312)<br>
