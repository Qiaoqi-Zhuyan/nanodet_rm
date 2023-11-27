# 5 points -> 13 points
# 目前项目仍在修改, 并非修改后的版本... (- w -)

yolo format: label x y w h 
SJTU RM format: label x y w h x1 y1 x2 y2 x3 y3 x4 y4 

p1->p4 为灯条的四个点

goal: label (red/blue + num), p1->p4 (解算世界坐标系下位置)

filter: 

0. 本质问题是如何做到关键点回归...
1. 如何过滤非同一个装甲板上的四个点? 注意保证p1 ~ p4 的这八个数据属于同一个装甲板
2. 装甲板跳变问题: 可以在之后的滤波中, 设置


# Reference
## label 参考:

https://github.com/xinyang-go/LabelRoboMaster

将RMUL不会用到的(前哨战, 死亡目标), 不对其进行标注, 作为负样本

## 4-key-point 参考:

https://github.com/zRzRzRzRzRzRzR/YOLO-of-RoboMaster-Keypoints-Detection-2023

https://github.com/Harry-hhj/CVRM2021-sjtu/tree/main


## 部署参考:
https://github.com/fb029ed/yolov5_cpp_openvino


