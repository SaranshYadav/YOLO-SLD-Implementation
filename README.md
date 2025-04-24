# YOLO SLD Implementation(not official)

As there was no publicly available implemenation of the research paper, I decided to make my own - [YOLO-SLD: An Attention Mechanism-Improved YOLO for License Plate Detection](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10571945)

## Installation

Conda environment (convinient)
1. Use the existing requirements.txt
   conda create -n myenv python=3.10
   conda activate myenv
   pip install -r requirements.txt
2. Download the checkpoint or you can train it yourself as well
   [Checkpoint](https://drive.google.com/file/d/1qUCXu8WdqeRPVvghiyRBAHz4EPNbUZ5V/view?usp=sharing)
3. Create dataset and label based on expected yolov7 format
   class, x_center, y_center, width, height
4. Change train, test and val dataset location in data/number_plate.yaml

## Training Images
![Screenshot from 2025-04-12 01-06-51](https://github.com/user-attachments/assets/dcf6e585-eb59-4e1d-8504-3c5212c0e613)

## Testing Images
![Screenshot from 2025-04-12 01-13-22](https://github.com/user-attachments/assets/f31e5e1d-32b9-4ae8-8765-2e96a72dfdc1)

 Results don't look the same. As in the research paper, they randomly selected 100k for training, 50k for val and 50k for test 
 I didn't look at the seed number.
## Detection
![Screenshot from 2025-04-25 04-18-36](https://github.com/user-attachments/assets/dad851db-e23c-4cd4-ac20-f401a728551e)

## Useful articles
[Step-by-step instructions for training YOLOv7 on a Custom Dataset](https://www.digitalocean.com/community/tutorials/train-yolov7-custom-data)

## Citation

```
@ARTICLE{10571945,
  author={Chung, Ming-An and Lin, Yu-Jou and Lin, Chia-Wei},
  journal={IEEE Access}, 
  title={YOLO-SLD: An Attention Mechanism-Improved YOLO for License Plate Detection}, 
  year={2024},
  volume={12},
  number={},
  pages={89035-89045},
  keywords={License plate recognition;YOLO;Neurons;Accuracy;Feature extraction;Visualization;Detectors;Deep learning;Deep learning;license plate detection;YOLOv7;SimAM;attention mechanism},
  doi={10.1109/ACCESS.2024.3419587}}

```

## Acknowledgements

<details><summary> <b>Expand</b> </summary>

* [https://github.com/AlexeyAB/darknet](https://github.com/WongKinYiu/yolov7)


</details>
