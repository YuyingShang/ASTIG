# AeroSTIG

商钰滢，侯英妍*，刘子楠，卢宛萱，黄宇鸿，王逸潇，于泓峰，付琨

此仓库为 **潜在扩散模型驱动的空天时序图像生成方法** 的官方实现。

### 安装要求
```cmd
conda create -n fb python=3.10
conda activate AeroSTIG
pip install -r requirements.txt
```

### 生成示例
以 “ 秋天到冬天 ” 季节变化时序描述文本为例：
```cmd
python main.py --config dataset/configs/a2w.yaml
```

筛选数据集样例存储在：
```cmd
filter/config_captions_a2w.yaml
```

其余模型实现代码及数据集将在论文录用后公布。
