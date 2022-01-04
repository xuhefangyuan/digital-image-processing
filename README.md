# digital-image-processing
答辩+代码材料
#### 介绍

**基于OpenCV的疲劳检测技术**

#### 软件架构

经查阅相关文献，疲劳在人体面部表情中表现出大致三个类型：打哈欠（嘴巴张大且相对较长时间保持这一状态）、眨眼（或眼睛微闭，此时眨眼次数增多，且眨眼速度变慢）、点头（瞌睡点头）。本实验从人脸朝向、位置、瞳孔朝向、眼睛开合度、眨眼频率、瞳孔收缩率等数据入手，并通过这些数据，实时地计算出驾驶员的注意力集中程度，分析是否疲劳驾驶和及时作出安全提示。

环境：Win10、Python3.7
使用的库：

- Opencv：图像处理
- Dlib：一个很经典的用于图像处理的开源库，shape_predictor_68_face_landmarks.dat是一个用于人脸68个关键点检测的dat模型库，使用这个模型库可以很方便地进行人脸检测，并进行简单的应用。
- Numpy：基于Python的n维数值计算扩展。
- Imutils ：一系列使得opencv 便利的功能，包括图像旋转、缩放、平移，骨架化、边缘检测、显示
- matplotlib 图像（imutils.opencv2matplotlib(image）。
- wx：python界面工具


#### 标准参数说明

疲劳认定标准：

- 眨眼：连续3帧内，眼睛长宽比为 0.2
- 打哈欠：连续3帧内，嘴部长宽比为 0.5
- 瞌睡点头：连续3帧内，pitch（x）旋转角为 0.3

(`真实运用中需要根据不同人的眼睛大小进行检测，人的眼睛大小，俯仰头习惯都不一样，这只是一个参考值`)

![image-20220104101124626](C:\Users\mmail\AppData\Roaming\Typora\typora-user-images\image-20220104101124626.png)


#### 使用说明

一、初始化界面

![初始化功能页面](https://images.gitee.com/uploads/images/2019/1225/233300_cbfbf3c5_5490475.png "屏幕截图.png")



2.参数设置



![image-20220104100321510](C:\Users\mmail\AppData\Roaming\Typora\typora-user-images\image-20220104100321510.png)

3.参数可调

![参数可调](https://images.gitee.com/uploads/images/2019/1225/233541_9343408f_5490475.png "屏幕截图.png")



#### 参与贡献

徐何方圆

刘嘉琳

陈显权

郭松铭

蔡仁杰

吕逢春
