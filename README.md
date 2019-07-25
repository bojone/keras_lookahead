## lookahead优化器的Keras实现

论文<a href="https://arxiv.org/abs/1907.08610" target="_blank">《Lookahead Optimizer: k steps forward, 1 step back》</a>的Keras实现。

用法：
```
model.compile(optimizer=Adam(1e-3), loss='mse') # 用你想用的优化器
lookahead = Lookahead(k=5, alpha=0.5) # 初始化Lookahead
lookahead.inject(lookahead) # 插入到模型中
```

中文介绍：https://mp.weixin.qq.com/s/3J-28xd0pyToSy8zzKs1RA

## lookahead optimizer for keras

Keras implement of <a href="https://arxiv.org/abs/1907.08610" target="_blank">Lookahead Optimizer: k steps forward, 1 step back</a>

Usage:
```
model.compile(optimizer=Adam(1e-3), loss='mse') # Any optimizer
lookahead = Lookahead(k=5, alpha=0.5) # Initialize Lookahead
lookahead.inject(lookahead) # add into model
```
