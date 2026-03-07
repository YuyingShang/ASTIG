
# AeroSTIG

商钰滢，侯英妍*，刘子楠，卢宛萱，黄宇鸿，王逸潇，于泓峰，付琨

此仓库为 **潜在扩散模型驱动的空天时序图像生成方法** 的官方实现。

### 安装要求

```cmd
conda create -n fb python=3.10
conda activate AeroSTIG
pip install -r requirements.txt
```

### 运行

初始视频描述和筛选后的era视频描述已公开在dataset文件夹内。

configs文件夹中已提供三类帧提示文本样例，下附生成结果示例，模型实现代码及全部帧提示数据集将在论文录用后公布。

##### 光照变化

```cmd
python main.py --config dataset/configs/light.yaml
```

<img src="image/README/1772871522444.gif" width="300">     <img src="image/README/1772871541425.gif" width="300">

样例1

<img src="image/README/1772870903530.jpg" width="600">
样例2

<img src="image/README/1772870930769.jpg" width="600">
##### 冬季变化

```cmd
python main.py --config dataset/configs/winter.yaml
```

<img src="image/README/1772871436570.gif" width="300">     <img src="image/README/1772871455080.gif" width="300">

样例1

<img src="image/README/1772870990367.jpg" width="600">
样例2

<img src="image/README/1772871037713.jpg" width="600">
##### 秋季变化

```cmd
python main.py --config dataset/configs/autumn.yaml
```

<img src="image/README/1772871209545.gif" width="300">     <img src="image/README/1772871277683.gif" width="300">

样例1

<img src="image/README/1772871313113.jpg" width="600">
样例2

<img src="image/README/1772871245302.jpg" width="600">
