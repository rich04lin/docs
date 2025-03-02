## [ torch 参数更多 ]torch.nn.Dropout3d

### [torch.nn.Dropout3d](https://pytorch.org/docs/stable/generated/torch.nn.Dropout3d.html?highlight=dropout3d#torch.nn.Dropout3d)
```python
torch.nn.Dropout3d(p=0.5,
                   inplace=False)
```
### [paddle.nn.Dropout3D](https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/api/paddle/nn/Dropout3D_cn.html#dropout3d)
```python
paddle.nn.Dropout3D(p=0.5,
                    data_format='NCDHW',
                    name=None)
```

PyTorch 相比 Paddle 支持更多其他参数，具体如下：

### 参数映射

| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| p           | p         | 表示丢弃概率。        |
| inplace      | -            | 表示在不更改变量的内存地址的情况下，直接修改变量的值，Paddle 无此参数，一般对网络训练结果影响不大，可直接删除。  |
| -            | data_format  | 指定对输入的数据格式，PyTorch 无此参数，Paddle 保持默认即可。 |
