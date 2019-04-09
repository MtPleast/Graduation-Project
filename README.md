# Lithium Battery Management System
==
计划使用平台：MatLab
--
## 第一步：选定模型（等效电路模型）-thenevin
--
第二步：HPPC测试
--
第三步：从HPPC测试中得到一组取样点，拟合得到OCV-SOC曲线（MatLab curvefitting）
--
第四步：thenevin模型中系统输出U和输入I在z域的传递函数；使用HPPC测试数据，使用递推最小二乘参数辨识（RLS）的方法，得到thenevin模型参数（MatLab）
--
第五步：写出thenevin等效电路模型的离散状态空间方程；对该模型使用拓展卡尔曼滤波（EKF）的方法，估计系统的状态变量SOC（State of Charge,荷电状态）
--
第六步：电池组串并联模拟仿真
--
