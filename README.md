# YOLO v9 ONNX Export

YOLO v9 Model exported for ONNX usage in Frigate. 

[Model Reference](https://github.com/WongKinYiu/yolov9)

[Frigate Export Guide](https://docs.frigate.video/configuration/object_detectors/#downloading-yolo-nas-model)

Although i had some issues with frigates own export guide, so i updated it on my own 
[My Update Guide](https://ioritro.com/blog/2025-09-01-frigate-onnx-detection-model/)

| Model | Test Size | AP<sup>val</sup> | AP<sub>50</sub><sup>val</sup> | AP<sub>75</sub><sup>val</sup> | Param. | FLOPs | Exported |
| :-- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| [**YOLOv9-T**] | 640 | **38.3%** | **53.1%** | **41.3%** | **2.0M** | **7.7G** | [ ] |
| [**YOLOv9-S**] | 640 | **46.8%** | **63.4%** | **50.7%** | **7.1M** | **26.4G** | [x] |
| [**YOLOv9-M**] | 640 | **51.4%** | **68.1%** | **56.1%** | **20.0M** | **76.3G** | [ ] |
| [**YOLOv9-C**] | 640 | **53.0%** | **70.2%** | **57.8%** | **25.3M** | **102.1G** | [x] |
| [**YOLOv9-E**] | 640 | **55.6%** | **72.8%** | **60.6%** | *57.3M** | **189.0G** | [ ] |
