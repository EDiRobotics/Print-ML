# Print-ML

#### 安装: 
```
git clone https://github.com/EDiRobotics/printml
cd printml
pip install -e .
```
#### 配置
```
accelerate config
```
选择GPU卡数, 混合精度等(建议bf16)。然后在`Train.py`中配置训练参数。

#### 运行
1. 生成模拟数据集
```
cd Datasets
python GenerateFakeDataset.py
```
2. 开始训练
```
cd Scripts
accelerate launch TrainDeformPred.py
```

