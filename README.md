# YOLO v9 ONNX Export

YOLO v9 Model exported for ONNX usage in Frigate. 

[Model Reference](https://github.com/WongKinYiu/yolov9)

[Frigate Export Guide](https://docs.frigate.video/configuration/object_detectors/#downloading-yolo-nas-model)

Although i had some issues with frigates own export guide, so i updated it on my own 
[My Update Guide](https://ioritro.com/blog/2025-09-01-frigate-onnx-detection-model/)

## 320

Upstream only publishes AP at 640, so this table has no AP columns. FLOPs are approximate (the 640 value ÷ 4).

| Model | Test Size | Param. | FLOPs | Exported |
| :-- | :-: | :-: | :-: | :-: |
| [**YOLOv9-T**](yolov9-t-320.onnx) | 320 | **2.0M** | **~1.9G** | ✅ |
| [**YOLOv9-S**](yolov9-s-320.onnx) | 320 | **7.1M** | **~6.6G** | ✅ |
| [**YOLOv9-M**](yolov9-m-320.onnx) | 320 | **20.0M** | **~19.1G** | ✅ |
| [**YOLOv9-C**](yolov9-c-320.onnx) | 320 | **25.3M** | **~25.5G** | ✅ |
| [**YOLOv9-E**](https://github.com/oritromax/YOLOv9-onnx/releases/tag/yolov9-e-320) | 320 | **57.3M** | **~47.3G** | ✅ |

## 640

| Model | Test Size | AP<sup>val</sup> | AP<sub>50</sub><sup>val</sup> | AP<sub>75</sub><sup>val</sup> | Param. | FLOPs | Exported |
| :-- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| [**YOLOv9-T**](yolov9-t-640.onnx) | 640 | **38.3%** | **53.1%** | **41.3%** | **2.0M** | **7.7G** | ✅ |
| [**YOLOv9-S**](yolov9-s-640.onnx) | 640 | **46.8%** | **63.4%** | **50.7%** | **7.1M** | **26.4G** | ✅ |
| [**YOLOv9-M**](yolov9-m-640.onnx) | 640 | **51.4%** | **68.1%** | **56.1%** | **20.0M** | **76.3G** | ✅ |
| [**YOLOv9-C**](yolov9-c-640.onnx) | 640 | **53.0%** | **70.2%** | **57.8%** | **25.3M** | **102.1G** | ✅ |
| [**YOLOv9-E**](https://github.com/oritromax/YOLOv9-onnx/releases/tag/yolov9-e-640) | 640 | **55.6%** | **72.8%** | **60.6%** | **57.3M** | **189.0G** | ✅ |

The E models are over GitHub's 100 MB per-file limit, so they are release downloads instead of repo files.
