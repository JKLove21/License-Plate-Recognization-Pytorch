# License-Plate-Recognization-Pytorch
该工作的内容主要是面向中国车牌识别系统的。车牌的检测系统通过YOLOv3系统来实现，检测后的车牌会通过空间变换网络进行倾斜校正。校正后的图片经由LPRNet进行识别。目前在1000张图片上测试的最终准确率可达93.3%
YOLOv3运行的时候需要输入命令语句python object_detection_yolo.py --image=图片名.jpg
YOLOv3的权重模型，可以从链接：https://pan.baidu.com/s/1I2Hv__uiN7ql7RLe99nWsw 
提取码：rsue得到
LPRNet需要测试的车牌可以放进test文件夹内，size为94×24
LPRNet只需要运行LPRNet test函数即可得到结果
其中我们已经添加了STN网络，如果您想去掉STN，只需要对images = STN（images）进行注释即可
如果您认可我们的工作，麻烦给我们一个星星，谢谢您
