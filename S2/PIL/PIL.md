1. 什么是 PIL
PIL 全称 Python Imaging Library，是 Python 里最早、最经典的 图像处理库。
它提供了打开、处理、保存图片的各种功能，例如：读取 JPG/PNG、缩放、裁剪、旋转、滤镜、颜色处理等。
但是 PIL 很久以前就停止维护了（2009年最后更新）。
2. Pillow —— PIL 的继任者
现在大家常用的其实是 Pillow，它是 PIL 的一个分支（fork），社区继续维护和升级。
现代 Python 里你安装的是 Pillow，但导入时还是用：
from PIL import Image
这是为了兼容老的 PIL 代码。
所以当你看到 from PIL import Image，实际上用的就是 Pillow，而不是原始的 PIL。

Pillow 的常用功能点可以概括为：
- 文件 I/O（打开、保存、格式转换）
- 基本属性（尺寸、模式、格式）
- 颜色空间转换（RGB ↔ 灰度/HSV 等）
- 几何变换（缩放、裁剪、旋转、翻转、仿射）
- 像素级操作（直接访问像素，或转 numpy/tensor）
- 滤镜/增强（模糊、锐化、对比度、亮度）
- 绘图（画框、文字，常用在数据可视化）
- 通道操作（拆分/合并 R、G、B）
- 深度学习接口（与 torchvision transforms 配合）

```
```