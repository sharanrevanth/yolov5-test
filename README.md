## Requirements

Python 3.7 or later with all `requirements.txt` dependencies installed, including `torch >= 1.5`. To install run:
```bash
$ pip install -U -r requirements.txt
```
## Inference

Inference can be run on most common media formats. Results are saved to `./inference/output`.To run inference on examples in the `./inference/images` folder
```bash

python detect.py --weights "/content/drive/My Drive/yolo weight/yolov5x.pt" 
                 --img 416 
                 --conf 0.4 
                 --source ./inference/images/ 
                 --deepsort ./config/deep_sort.yaml
