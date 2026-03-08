# ASTIG

商钰滢，侯英妍*，刘子楠，卢宛萱，黄宇鸿，王逸潇，于泓峰，付琨

此仓库为 **潜在扩散模型驱动的航空时序图像生成方法（ASTIG）** 的官方实现。

> **ASTIG: A Training-Free Framework for Aerial Spatio-Temporal Image Generation**

## 简介

ASTIG 是一种无需训练的航空时序图像生成框架，通过协同集成动态语义分解流程、语言绑定策略与时序锚点注意力机制，在无需额外训练的条件下实现语义精准、主体稳定且时序连贯的航空时序图像生成。

## 安装要求

```cmd
conda create -n astig python=3.10
conda activate astig
pip install -r requirements.txt
```

## 数据集

初始视频描述和筛选后的 ERA 视频描述已公开在 `dataset` 文件夹内。`configs` 文件夹中已提供三类帧提示文本样例。完整的帧提示数据集将在论文录用后公布。

## 运行

### 光照变化

```cmd
python main.py --config dataset/configs/light.yaml
```

<img src="image/README/1772871522444.gif" width="300">     <img src="image/README/1772871541425.gif" width="300">

**样例1**

<img src="image/README/1772870903530.jpg" width="600">

**样例2**

<img src="image/README/1772870930769.jpg" width="600">

### 冬季变化

```cmd
python main.py --config dataset/configs/winter.yaml
```

<img src="image/README/1772871436570.gif" width="300">     <img src="image/README/1772871455080.gif" width="300">

**样例1**

<img src="image/README/1772870990367.jpg" width="600">

**样例2**

<img src="image/README/1772871037713.jpg" width="600">

### 秋季变化

```cmd
python main.py --config dataset/configs/autumn.yaml
```

<img src="image/README/1772871209545.gif" width="300">     <img src="image/README/1772871277683.gif" width="300">

**样例1**

<img src="image/README/1772871313113.jpg" width="600">

**样例2**

<img src="image/README/1772871245302.jpg" width="600">

## 致谢

本项目基于 [Stable Diffusion](https://github.com/CompVis/stable-diffusion) 构建，感谢相关开源社区的贡献。
