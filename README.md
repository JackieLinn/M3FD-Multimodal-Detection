<div align="center">
    <h1>M3FD-Multimodal-Detection</h1>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="">&nbsp;&nbsp;&nbsp;
    <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="">
</div>

<br>

YNU's Introduction to Artificial Intelligence course final assignment repository.

## Get Started

```bash
git clone https://github.com/JackieLinn/M3FD-Multimodal-Detection.git
cd ./M3FD-Multimodal-Detection/
```

## Environments

You can install the environment by the following method:

```bash
pip install -r requirements.txt
```

Alternatively, you can install a full conda environment:

```bash
conda env create -f environment.yml
```

Then go to the PyToch website to install the PyToch version that is compatible with your environment.

## Dataset Configuration

You need to store the dataset in the following format:

```
dataset/                  # 数据集的地址
│   ├── visible/          # 存储 可见光图像 + 标签
│   │   ├── train/        # 训练
│   │   │    ├── image1.jpg 
│   │   │    ├── image1.txt   
│   │   │    ├── image2.jpg   
│   │   │    ├── image2.txt 
│   │   │    └── ...
│   │   │    
│   │   └── test/        # 验证/测试
│   │        ├── image5.jpg 
│   │        ├── image5.txt   
│   │        ├── image6.jpg   
│   │        ├── image6.txt 
│   │        └── ...
│   │       
│   └── infrared/         # 存储红外图像 + 标签
│       ├── train/        # 训练
│       │    ├── image1.jpg 
│       │    ├── image1.txt   
│       │    ├── image2.jpg   
│       │    ├── image2.txt 
│       │    └── ...
│       │    
│       └── test/         # 验证/测试
│            ├── image5.jpg 
│            ├── image5.txt   
│            ├── image6.jpg   
│            ├── image6.txt 
│            └── ...
labels/                 # 可选 这个目录可不用
    ├── train/          # 训练图像标签
    │   ├── image1.txt   
    │   └── image2.txt   
    └── test/           # 验证/测试标签
        ├── image5.txt 
        └── image6.txt 
```

## Run scripts

You can execute the training and validation code using the following command:

```bash
python train.py --mode mode_name
python val.py --mode mode_name
```

### If you are interested in this project, feel free to fork and star!
