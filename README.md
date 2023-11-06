# object detection agumon

This is an example usage of Faster R-CNN in OpenMMLab toolbox for object detection.

![](example1.PNG)

Pictures for agumon are collected and then annotated by LabelBee with bounding box.

The labels of the pictures are saved in coco format. 

The data splits into training and test set. You could further split the data into validation set to check the model performance during training.

The model is trained with 12 epoch. The learning rate is 2.5e-05 and the estimated time for completion is 2 seconds. The training time for this iteration is 0.668 seconds, with 0.263 seconds spent on loading data. The memory usage is 3613 MB. The loss for each component of the model is also shown, including loss_rpn_cls (classification loss for region proposal network), loss_rpn_bbox (bounding box regression loss for region proposal network), loss_cls (classification loss for object detection), and loss_bbox (bounding box regression loss for object detection).

The evaluation shows that the result of the model using the mmdetection library on the validation dataset at epoch 12. The evaluation metric used is mean average precision (mAP) for bounding boxes. The overall bbox_mAP for this epoch is 0.8506, which is a measure of the average precision over different intersection-over-union (IoU) thresholds. The bbox_mAP_50 is 1.0000, which means that the model is able to correctly detect objects with an IoU of 0.5 or more. The bbox_mAP_75 is 0.9691, which means that the model is able to correctly detect objects with an IoU of 0.75 or more. The evaluation also includes separate mAP values for small, medium, and large objects, denoted as bbox_mAP_s, bbox_mAP_m, and bbox_mAP_l, respectively. The bbox_mAP_copypaste is a copy-paste friendly version of the evaluation results.

Finally, the log shows that the evaluation results have been successfully loaded and prepared, with a loading time of 0.00 seconds.

In the final section, only one sample is shown to minimize the file size, you could show more samples if you wish.  


