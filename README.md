![image](https://github.com/Robotics-Aerial-Robots/Homework/blob/master/LOGO%20中英文橫.png)
# 108 年度 機器人學：多軸旋翼機 

### HW3
Deadline: 
---
## 題目
學習基本Eigen操作，並了解旋轉矩陣和四元數與歐拉角的關係，
更多Eigen應用可參考https://eigen.tuxfamily.org/dox/group__QuickRefPage.html

### 指令
```
	roscore
	rosrun HW3 eigen_tutorial
	rosrun HW3 eigen_transform 

```
### eigen_tutorial.cpp
Declare Eigen 4x4 Matrix with each element as double.
We can directly given the matrix value by <<.
Matrix addition and subtraction can also be apply by + and -.
<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/1.png" width="80%" height="40%">

Declare Eigen 3x1 Vector with each element as double.
Vector dot and cross operation are applied.
<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/2.png" width="80%" height="50%">

Declare Eigen 3x3 Matrix and 3x1 Vector.
By apply block operation to Eigen 4x4 Matrix, we can obtain a sub-block.
For example, block<3,3>(0,0) means extract a Eigen 3x3 Matrix from the matrix in (0,0) element.
Then apply two transformation to the vector.
We should notice applying rotation first and translation first will have different result.
These two types of transformation is oftenly used, one should use rotation first or translation first depend on the frame of transformation.
<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/3.png" width="80%" height="50%">

### eigen_transform.cpp

<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/4.png" width="80%" height="40%">


<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/5.png" width="70%" height="30%">


<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/6.png" width="80%" height="40%">


<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/7.png" width="80%" height="50%">


<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/8.png" width="60%" height="30%">


<img src="https://github.com/Robotics-Aerial-Robots/Homework3/blob/master/Figures/9.png" width="80%" height="40%">
---
