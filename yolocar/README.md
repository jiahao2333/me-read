# **yolov7车牌识别算法，支持12种中文车牌类型**

**1.单行蓝牌**
**2.单行黄牌**
**3.新能源车牌**
**4.白色警用车牌**
**5 教练车牌**
**6 武警车牌**
**7 双层黄牌**
**8 双层武警**
**9 使馆车牌**
**10 港澳牌车**
**11 双层农用车牌**
**12 民航车牌**

## **那么？怎么跑起来呢？**

首先 建议您使用conda虚拟环境 请先安装conda

安装后 打开conda prompt 输入
```
conda create -n opencv python=3.9
conda activate opencv
```
第一行opencv为环境名 可以随意更改

进入到项目目录 输入
```
pip install -r requirements.txt
```
安装所需要的库 

**测试demo:**
以yolov7-lite-s 为例:
```
python detect_rec_plate.py --detect_model weights/yolov7-lite-s.pt  --rec_model weights/plate_rec.pth --source imgs --output result
```

测试文件夹imgs，结果保存再 result 文件夹中


