# 反作弊

目前服务器安装有AAC反作弊插件，自动检测并处理作弊行为。

----------
### 处罚措施

反作弊系统检测并认定为作弊后，会自动被踢出或封禁31天。

如多次作弊，服务器可能会追加封禁时间，直至永久

----------

### 封禁/踢出代码

在你被封禁时（希望永远不会），你将在踢出页面得到一串代码，例如下面这样：

`[MGEN5 | 20.0 | 13]`

其中：

 - MGEN  代表行为（action)。
 - 20.0 代表封禁时服务器tps
 - 13 代表玩家到服务器的延迟

下面是可能出现的封禁代码：

1.战斗类修改作弊(Combat)
- `CG` | 代表违规者已使用各种战斗性修改很长一段时间
- `CARA` | 自瞄（瞄准辅助）/杀戮光环
- `CCLK` | 连点器
- `CHBX` | 使用某种形式上的自瞄（瞄准辅助）/杀戮光环

2.移动类修改作弊(Movement)

- `MGEN` | 移速修改/飞行
- `MNSD` | 无减速，减小或删除蜘蛛网、进食、护盾阻挡、流水/岩浆所造成的的减速。**强制疾跑不在检测范围之内**
- `MVCL` | 修改实体骑乘时的移速 (马、矿车等)
- `MNF` | 规避掉落伤害,
- `MELY` | 鞘翅相关作弊
- `MTMR` | 尝试加速服务器时间刻以规避速度检测
- `MVEL` | 尝试减小或规避击退效果
- `MSNK` | 同时潜行/冲刺

3.利用延迟/交互作弊(Blocks)

- `DLLY` | 尝试以更快的速度放置/破坏方块
- `IG` | 尝试使用修改过的客户端进行无效交互

4.其他

- `IB` | 尝试向服务器发送无效数据包

----------

### 误判与申诉

某些客户端（例如Badlion、Lunar）等可能会导致误判。服务器始终建议使用原版客户端以避免误判

如果你坚信你没有作弊，请到服务器官网[提交申诉](https://usolia.net/forums/%E7%94%B3%E8%AF%89.24/)。