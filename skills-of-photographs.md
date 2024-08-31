![image](https://github.com/user-attachments/assets/98869d77-64b3-451b-8b15-ddc53d1cb721)![image](https://github.com/user-attachments/assets/e094d7ad-c55a-4d2d-a7d3-1448a5a7cca4)# 拍照技巧

## 环绕物体--拍照技巧

先来诉说我们对照片的要求。照片的清晰度和分辨率要高、拍摄物体的光照要均匀、以及照片适当的重叠覆盖物体。尽量把物体的所有地方都拍完整，这样重建效果最好。

###  正确方法

1.我们得保证照片的分辨率够高，分辨率按理来说分辨率越高越好。

![1](https://github.com/user-attachments/assets/f181e14a-4e09-4873-a5b9-d5ba0f444edc)

2.我们需要的拍摄物体光照均匀，iso保持一个数值，白平衡保持一个数值

![1](https://github.com/user-attachments/assets/e24a7999-57a8-4163-b505-daaa14f6e883)

3.重叠让colmap更好的提取特征点，尽量把物体拍全，每个角度尽量保证拍全


![38](https://github.com/user-attachments/assets/5ff96cdf-ac3e-4577-86ef-cdcbd850bafd)

![6](https://github.com/user-attachments/assets/876e7401-545a-44f5-bbca-8d1e249d31d3)

这里的数据一共是38张图片，在这就不一一列举了，这里给instant——ngp的结果，重建效果的光照因为不是很亮看着就和图片差不多的光度。

![image](https://github.com/user-attachments/assets/72c57522-cb86-496e-b70f-eb3fe100cf92)

### 错误方法
 
1.分辨率过低可能colmap都无法正常提取照片，更不必说照片的清晰度不足，这组照片虽然是环绕空间进行的重建，但究其原因还是无法提取更多有用的物体特征点，导致colmap跑崩了。之前跑环绕物体不好的照片删的差不多了，就用这个代替一下。

![image](https://github.com/user-attachments/assets/d0121f58-833c-44b5-bde0-ee27614d470d)

![81324cb61985df19c1c6b3d3f142d6a9](https://github.com/user-attachments/assets/56eca91c-1912-4f21-89df-951d6f1b91f8)

2.光照不够均匀，灯光补的有偏差，这边造成物体有影子出现，还有书本的反射光斑，导致最终重建有影响

![20](https://github.com/user-attachments/assets/5e96a8e5-4d2c-444a-bdf1-ad4cd00e0532)

这是instant-ngp跑出来的效果，这组图片还有对焦点出现在背景上出现的结果就是想要的物体清晰度不足

![image](https://github.com/user-attachments/assets/2378e357-6739-426a-8c71-0caf91fa510a)

![image](https://github.com/user-attachments/assets/e6b00083-b1bb-46de-9e4c-c840838c3fb8)

3.拍摄的角度不完整漏拍的角度无法呈现想要的效果，没有覆盖和重叠物体的每一个地方，所以这组照片86张照片不如上面那一组照片的效果好，以及白平衡问题，这组照片的白平衡是自动这个也得避免。

![image](https://github.com/user-attachments/assets/e7ab6467-b0d9-46bb-aa89-01bd9ff56c16)

## 环境空间--拍照技巧

照片要求和环绕物体一样，但多了需要第二条轴线承载拍摄物体，单独的一条轴难以支撑colmap提取特征，甚至使用一条轴无法达到预期的效果。

### 正确方法

1.使用补光灯进行光照平衡，并且在晚上拍摄避免白天太阳影响。这里可以看出被拍摄物体的辨识度很高，且光照影响很低。

![008](https://github.com/user-attachments/assets/f990c1cc-ac49-4b05-a2d1-90e738dfc8c4)

2.记得使用两条轴线，ngp显示不好看出来，但我们拍摄是以两条轴旋转下去的

![image](https://github.com/user-attachments/assets/7e4186c8-074b-4308-84a3-7c52e0486e85)

### 错误方法

1.有太阳光影响重建效果，出现蓝色斑点

![image](https://github.com/user-attachments/assets/d1c27808-e2e3-4da4-b608-1b404efcc28f)

2.单独一条轴线的重建，无法提取想要的特征

![1](https://github.com/user-attachments/assets/6e352722-5282-409e-ac32-d79e6d63118c)

![image](https://github.com/user-attachments/assets/3d3082a7-5095-4517-bbd6-9042e78c7f9a)

---
-钟启迪（2024.08.29）











