# DRL_collection
a  collection of DRL-repo in Github

| 时间 | 改动 | TODO | 版本 |
| :-----: | :-----: | :-----: | :-----:|
| 2019.12.27 | init | todo | v0.1 |
| 2020.1.6 | 加入keras-rl | 整理学院派资料和repo | v0.1 |
| 2020.1.10 | 整理学院派资料， 加入baselines | todo | v0.2 |
| - | - | - | - |
---
## 0. 学院派资料(北美)
很多资料都整理了这块的内容，我再简单的理清楚一下吧， 附带一些其他人的评价。
### UCL - RL Course by David Sliver
[课程主页](http://www0.cs.ucl.ac.uk/staff/d.silver/web/Teaching.html) \ [b站(熟肉)](https://www.bilibili.com/video/av45357759?p=1)

伦敦学院2015的经典课程， sutton体系。侧重RL的基本概念，没有深度RL方面的内容。偏重非深度的RL实现，重视数学证明convergence，以及value based RL。基本是把sutton的书精华提炼了一遍，大概学习路线是 agent-environment loop->MDP->Dynamic planning->Monte Carlo->TD->function approximation

### 加州大学伯克利分校 UCB - Deep RL Bootcamp
[课程主页](https://sites.google.com/view/deep-rl-bootcamp/lectures)

26-27 August 2017. UCB暑假课的课程，比较简洁全面的介绍一些RL方法。

### 加州大学伯克利分校 UCB - CS285 Fall 2019
CS 285: Deep Reinforcement Learning, Decision Making, and Control

[Home Page]() \ [youtube(生肉)](https://www.youtube.com/playlist?list=PLkFD6_40KJIwhWJpGazJ9VSj9CFMkb79A) \ [b站(生肉)](https://www.bilibili.com/video/av66523922?p=1) \ [b站CS294-112(熟肉)](https://www.bilibili.com/video/av39816961?p=1) \ 
[Homework_repo](https://github.com/Observerspy/CS294)

这门课原来叫cs294，首先294是伯克利Special Topics的课号，AP开的课很多都是在294+section这样的课号下试水。今年294-11２深度增强学习已经获得正式课号改为CS285。课程反应了Sergey Levine和整伯克利RL的积累，独立于《RL Introduction》的教学体系自成一派。符号风格和体系不同于《RL Introduction》体系。

CS285的精髓在于各种RL前沿方向全方位的推导和展示。前半部分讲各种RL的基础算法，后半部分讲RL算法的各种衍生，应用，科研。课程基本可以分为DRL介绍+模仿学习、model free、model based、Exploration+迁移+多任务+Meta-learning等四大部分，一共有四个很有趣的assignment（比春季的更好了）。如果你看过david silver的视频并且有机器学习的基础，那么至少你在model free部分是没问题的。秋季课程其实降低了对RL基础的要求，课上推导过程比较清晰。这门课后半model based部分恰好是对david silver等当前已有的课程、书籍里讲的比较少的内容的非常大的补充，不过这部分要求比较高。

### 斯坦福大学 Stanford [未验证]
CS234: Reinforcement Learning  [Home Page](http://web.stanford.edu/class/cs234/index.html) \ [Homework_repo](https://github.com/Observerspy/CS234)

CS239 Sequential Decision Making [Home Page](https://web.stanford.edu/class/aa229/cgi-bin/wp/)

AA228/CS238 Decision Making under Uncertainty [Home Page](https://web.stanford.edu/class/aa228/cgi-bin/wp/)

## 1. 深度强化学习
### [DRL_brief_course](https://github.com/Taospirit/DRL_brief_course)
Deep Reinforcement Learning Course

国外友人用精简的教程实现，附带有教程网站， 概念入门推荐。用游戏实现DRL经典算法: DQN \ DDQN \ PPO \ A2C ...
### [DRL_algorithms_lists](https://github.com/tigerneil/awesome-deep-rl)
整理很完备清晰的深度强化学习算法列表
### [DRL_with_pytorch](https://github.com/Taospirit/DRL-with-pytorch)
适合入手算法源码实践！ 中科院自动化所大佬用Pytorch写的DRL实现， 算法完整， 章节清晰， 2019年。 
### [DRL_with_imp_pytorch](https://github.com/p-christ/Deep-Reinforcement-Learning-Algorithms-with-PyTorch)
另一个版本基于Pytorch的DRL算法实现， 2019年。
### [DRL_with_tf_Morvan](https://github.com/Taospirit/DRL_with_tf_Morvan)
强烈推荐入门！ 莫烦大佬的基于tensorflow的DRL算法实现， 使用tf的中低层api实现网络。
### [Hands-On-Reinforcement-Learning-with-Python](https://github.com/PacktPublishing/Hands-On-Reinforcement-Learning-with-Python)
《用Python动手做强化学习》配套代码
### [tensorlayer](https://github.com/tensorlayer/tensorlayer)
**[官方]** 基于TF2.0开发的全套 [DRL算法库(面向科研)](https://github.com/tensorlayer/tensorlayer/tree/master/examples/reinforcement_learning) 和 [高层抽象算法库(面向产品化)](https://github.com/tensorlayer/RLzoo).  仿真环境基于gym。

鉴于当前(2020.01.08) TF2.0的稳定性, 该库待优化和验证， 可用于后期学习。
### [DRL_for_Keras](https://github.com/keras-rl/keras-rl)
高阶api实现的各种state-of-art的DRL算法，提供封装好的接口直接使用。[主页文档](https://keras-rl.readthedocs.io/en/latest/)
### [baselines](https://github.com/openai/baselines)
OpenAI Baselines is a set of high-quality implementations of reinforcement learning algorithms.

**[官方]** 官方上台， 吊打一切。 2017年开发，openai自己写的DRL实现库， 代码比较晦涩难懂， 但恰如其名。安装时注意MuJoCo的环境依赖。

### [Stable Baselines](https://github.com/hill-a/stable-baselines)
基于openai的baselines做的稳定版开发， 适合全面学习。 [主页文档](https://stable-baselines.readthedocs.io/en/master/)
- Unified structure for all algorithms
- PEP8 compliant (unified code style)
- Documented functions and classes
- More tests & more code coverage
- Additional algorithms: SAC and TD3 (+ HER support for DQN, DDPG, SAC and TD3)

### [rl-baselines-zoo](https://github.com/araffin/rl-baselines-zoo) 
基于baseline，已经训练好的库。推荐中期学习使用
### [MARL-Papers](https://github.com/LantaoYu/MARL-Papers)
多智能体的强化学习论文收集列表

---
## 2. 强化学习
### [RL_brief_collection](https://github.com/Taospirit/DRL_brief_collection)

awesome-reinforcement-learning

强化学习的相关学习资料\链接，精简完整的整理。

### [RL_basic_zh](https://github.com/Taospirit/RL_basic_zh)
强化学习从入门到放弃的资料

中文整理的强化学习资料（Reinforcement Learning）， 偏基础和理论。

附带各种课程链接，学院派资料集中地。

### [DRL_list](https://github.com/jgvictores/awesome-deep-reinforcement-learning)
**[未验证]** 从机器学习、神经网络、深度神经网络的全面的资料整理

### [RL_traditional](https://github.com/dennybritz/reinforcement-learning)
传统强化学习的算法介绍和实现， 无深度网络。

### [RL_sutton](https://github.com/ShangtongZhang/reinforcement-learning-an-introduction)
sutton第二版书的配套章节代码实现和学习

### [RL_solution_for_sutton_2nd](https://github.com/LyWangPX/Solutions-of-Reinforcement-Learning-An-Introduction-Sutton-2nd)
**[未验证]** sutton第二版书部分章节问题答案

---
## 3. 机器学习框架学习
### [Dive-into-DL-PyTorch](https://github.com/ShusenTang/Dive-into-DL-PyTorch)

将《动手学深度学习》原文中 MXnet 代码改为用 Pytorch 实现。[网页版主页](https://tangshusen.me/Dive-into-DL-PyTorch/#/) , [整书pdf下载](https://github.com/OUCMachineLearning/OUCML/blob/master/BOOK/Dive-into-DL-PyTorch.pdf)

## TODO...

---
## 4. 仿真环境
### [gym](https://github.com/openai/gym)
openai开发的经典环境， 安装简洁集成高效， 便于测试新算法。[主页](https://gym.openai.com/)

gym中整理的[openai环境](https://github.com/openai/gym/blob/master/docs/environments.md#pybullet-robotics-environments)
### [MuJoCO]()
[主页](http://www.mujoco.org/)
### [DM Control](https://github.com/deepmind/dm_control)
DeepMind: a tool for developing and testing reinforcement learning agents for the MuJoCo physics engine.
### [Lab](https://github.com/deepmind/lab)
DeepMind: A customisable 3D platform for agent-based AI research.


### [Marathon Environments](https://github.com/Unity-Technologies/marathon-envs)
A set of high-dimensional continuous control environments for use with Unity ML-Agents Toolkit.

