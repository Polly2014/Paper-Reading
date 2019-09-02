# Trust management for Vehicular Networks: An Adversary-Oriented Overview
## 摘要
> 两大重要防御方法
> - 密码学 Cryptography
> - Trust
## 1. Introduction
- 车载自主网络VANET安全很重要
- 网络安全靠Cryptograpy来保证
  - 证数、签名、公钥、指令检测系统、第三方插件
- 另一些场景：高速移动等，Cryptography方法表现并不好
  - 一个经过授权与验证的用户被恶意感染了
  - 信任管理Trust Management来补充这一不足
  - Trust可定义为：a subjective belief of a peer about other peers belonging to the same society or geographical zone
- VANET场景下
  - 信任评估基于历史的直接或间接交互行为
  - 由于基于历史数据计算，不存在延迟
- 信任模型分类
  - entity-oriented trust model
  - data-oriented trust model
  - hybird trust model
- 信任模型主要关注网络内部攻击 inside attack
- 文章阐述Trust对Cryptography何时更优、更差、或为补充
