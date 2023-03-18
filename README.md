# 复现Flatten&对图像进行噪声标注(2d&3d)  

## Flatten

[Flatten文档](https://www.nanophys.kth.se/nanolab/afm/icon/bruker-help/Content/SoftwareGuide/Offline/ModifyCommands/Flatten.htm)    

### 不平坦STM图像
![不平坦STM图像](https://github.com/Xianyusyy/Flatten-Noise_label/blob/main/Image%20with%20Bow.png "不平坦STM图像")

### 多项式拟合
对每一行做三次多项式拟合，原始数据减去多项式拟合数值即可得到平坦图像的数值。

![单行多项式拟合](https://github.com/Xianyusyy/Flatten-Noise_label/blob/main/%E5%A4%9A%E9%A1%B9%E5%BC%8F%E6%8B%9F%E5%90%88.png "单行多项式拟合")

### Flatten以后的STM图像
![Flatten以后的STM图像](https://github.com/Xianyusyy/Flatten-Noise_label/blob/main/Image%20with%20Bow%20Removed.png "Flatten以后的STM图像")

## 噪声标注
噪声定义为：当前像素点A的值与以A为中心的边长为3的正方形底边缘上的像素值的平均值相差超过0.4的，且A的值为当前正方形领域内top 3。A点就是噪声点。

### 标注噪声的3d图像
![标注噪声的3d图像](https://github.com/Xianyusyy/Flatten-Noise_label/blob/main/noise.png "标注噪声的3d图像")

## 2d图像
![2d图像](https://github.com/Xianyusyy/Flatten-Noise_label/blob/main/65_2d%20.png "2d图像")
