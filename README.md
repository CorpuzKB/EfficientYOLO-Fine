# EfficientYOLO-Fine
[Under construction]

This repository is used to train an anchor-based YOLO variant using the following:

                    
Structure  | Basis | References
------------- | ------------- |-------------
Backbone  | EfficientNetV2 |[[1]](https://arxiv.org/abs/2104.00298) [[2]](https://www.tensorflow.org/api_docs/python/tf/keras/applications/efficientnet_v2)
SPPF | YOLOv5 | [[3]](https://github.com/ultralytics/yolov5/blob/76ea9ed3a4d42fe835e172672132f13cf5286648/models/common.py#LL218C4-L218C4)
Neck  | YOLOv5, PP-YOLOv2 | [[4]](https://github.com/ultralytics/yolov5) [[5]](https://github.com/ultralytics/yolov5/issues/280) [[6]](https://arxiv.org/abs/2104.10419)
Decoupled Head | YOLOX | [[7]](https://arxiv.org/pdf/2107.08430)

The last convolutional stage of the EfficientNetV2 is removed to enhance small-scale object detection as adopted from [[8]](https://www.mdpi.com/2072-4292/12/15/2501).
