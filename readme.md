# cs61A project2
[资源](https://inst.eecs.berkeley.edu/~cs61a/sp18/proj/ants/)
## 运行
```shell
python gui.py
python gui.py --water #(泳池)
```

## 代码解释

这个AntColony类主要用于表示整个蚂蚁殖民地的游戏状态和模拟时间。其核心功能是模拟蜜蜂对蚂蚁殖民地的攻击过程。以下是代码的详细解释：

属性:

time: 表示经过的时间。
food: 当前殖民地的食物总量。
queen: 代表蚁后所在的位置。
places: 代表殖民地中所有的位置的列表。
bee_entrances: 蜜蜂可以进入的位置列表。
构造函数 (__init__):
此函数用于初始化蚂蚁殖民地。

strategy: 一个部署蚂蚁的函数。
hive: 一个充满蜜蜂的蜂巢。
ant_types: 蚂蚁构造函数的列表。
create_places: 一个创建位置集的函数。
dimensions: 游戏布局的尺寸。
configure方法:
配置殖民地中的位置。

simulate方法:
模拟对蚂蚁殖民地的攻击（即玩游戏）。该函数执行以下主要步骤：

从蜂巢中的蜜蜂入侵。
在合适的地方部署蚂蚁。
让蚂蚁采取行动。
让蜜蜂采取行动。
deploy_ant方法:
如果有足够的食物，就在某个地方放置一个蚂蚁。

remove_ant方法:
从殖民地中移除一个蚂蚁。

ants属性:
返回殖民地中所有蚂蚁的列表。

bees属性:
返回殖民地中所有蜜蜂的列表。

insects属性:
返回殖民地中所有昆虫的列表。

总结:
这个AntColony类负责管理整个游戏的状态和逻辑，它跟踪当前的时间，食物供应，以及所有的蚂蚁和蜜蜂。最核心的simulate方法模拟了整个游戏过程，包括蜜蜂的进攻、蚂蚁的部署和它们的行动。

