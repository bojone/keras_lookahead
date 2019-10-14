## Lookahead Optimizer for Keras

Keras implement of [Lookahead Optimizer: k steps forward, 1 step back](https://arxiv.org/abs/1907.08610).

Usage:
```
model.compile(optimizer=Adam(1e-3), loss='mse') # Any optimizer
lookahead = Lookahead(k=5, alpha=0.5) # Initialize Lookahead
lookahead.inject(model) # add into model
```

## Lookahead优化器的Keras实现

论文[《Lookahead Optimizer: k steps forward, 1 step back》](https://arxiv.org/abs/1907.08610)的Keras实现。

用法：
```
model.compile(optimizer=Adam(1e-3), loss='mse') # 用你想用的优化器
lookahead = Lookahead(k=5, alpha=0.5) # 初始化Lookahead
lookahead.inject(model) # 插入到模型中
```

中文介绍：[点击进入](https://mp.weixin.qq.com/s/3J-28xd0pyToSy8zzKs1RA)

## 交流
QQ交流群：67729435，微信群请加机器人微信号spaces_ac_cn
