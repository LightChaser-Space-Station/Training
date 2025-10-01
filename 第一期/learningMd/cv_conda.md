# 使用conda搭建OpenCV在Linux上的环境

```bash
#  创建并激活虚拟环境
conda create --name cvenv python=3.10
conda activate cvenv

#  下载opencv等图像处理库
conda install -c conda-forge opencv pillow scikit-image matplotlib

#  可以额外扩展安装深度学习的框架
#  请务必以官网生成的命令为准！
#  conda install pytorch torchvision torchaudio -c pytorch
#  conda install tensorflow

#  验证安装
python
```

```py
import cv2
import numpy as np

# 打印OpenCV的版本号
print(f"OpenCV version: {cv2.__version__}")

# 创建一个黑色的空白图像，验证Numpy和OpenCV的联动
blank_image = np.zeros((100, 200, 3), dtype=np.uint8)
print(f"Successfully created a blank image with shape: {blank_image.shape}")
```