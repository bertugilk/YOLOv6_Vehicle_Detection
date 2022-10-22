# YOLOv6_Vehicle_Detection
I trained the dataset consisting of vehicles from Roboflow using YOLOv6 on the Nvidia RTX3070 graphics card.


## Installation

git clone https://github.com/meituan/YOLOv6<br>
pip install -r requirements.txt<br>
pip install torch==1.8.1+cu111 torchvision==0.9.1+cu111 torchaudio==0.8.1 -f https://download.pytorch.org/whl/torch_stable.html<br>

## Train

python tools/train.py --batch 16 --conf configs/yolov6s_finetune.py --data-path dataset.yaml --device 0 --epochs 10 --eval-interval 2

## Usage

python tools/infer.py --weights weights/best_ckpt.pt --source test_images/{}.jpg --yaml dataset.yaml --device 0


![c0a105b4fe3a7c55_jpg rf 28745179cd0f87dc9cae886872f95263](https://user-images.githubusercontent.com/48621020/197339801-289350a7-6724-41d2-9a42-39f993e10039.jpg)
