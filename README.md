# WeChat_Face
**微信小程序：人脸检测/识别face_recognition库(基于dlib深度学习)的使用**

---

***关键字： Python & Tornado & MongoDB & face_recognition & dlib & WeChat & Admin***

---

> 0.加载图片，对图片进行初始化

```
0.使用face_recognition库中的load_image_file()方法，把图片转化为像素矩阵，方便后续调用
1.图形操作使用PIL
```

> 1.框选人脸功能

```
使用face_recognition库中的face_locations()方法查找人脸位置(位置算法)，基于轮廓算法
[(56, 683, 146, 593), (86, 354, 176, 265), (116, 494, 206, 404), (116, 155, 206, 66)]
左上角点、右下角点
```

> 2.人脸勾勒功能

```
通过face_recognition库中的face_landmarks()方法，特征算法获取所有的特征点
```

> 3.截取人脸功能

```
同样使用face_locations()方法查找人脸位置(位置算法)，基于轮廓算法
```

>4.人脸化妆

```
和第二项一样使用face_recognition库中的face_landmarks()方法，特征算法获取所有的特征点
```

> 5.人脸68个特征点获取

```
使用dlib库中的get_frontal_face_detector()特征提取器，并使用官方推荐的开源预测器训练好的模型shape_predictor_68_face_landmarks.dat
```

> 6.识别图片中的人是谁

```
通过face_recognition库中的face_encodings()方法，提取关键点值，并通过compare_faces()方法判断result
```

>6.实时人脸检测

```
使用OpenCV实现，还没实现...
```

### ...

