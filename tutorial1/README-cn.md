基础强化学习教程 1 ： Q-learning

这个教程覆盖使用cat-mouse-cheese 例子的 Q-learning 算法

# 目录
- [背景](#background)
- [ *World* and *Cat* 玩家的实现](#world)
- [ *Mouse* 玩家](#mouse)
  - [Q-learning 实现](#q-learning)
- [结果](#results)
- [你自己来重新实现](#reproduce)


<div id='background'/>
### 背景
值函数（value function）是一个状态-动作对（state-action pair）函数，用来估计在一个特定状态（state）下，一个动态（action）的优劣，或者返回价值（评分）最高的动作


Q-learning 是一个离线（*off-policy*）算法（可以根据推断的action来更新值函数，其实并没有去尝试这个action）