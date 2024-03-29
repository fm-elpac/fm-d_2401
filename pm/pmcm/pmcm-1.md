# PMCM-1
胖喵做饭机器


## 主要设计

主动部件:

+ 单臂移动平台 (含视觉及传感模块)  x2

  - 高速臂 x1

  - 低速臂 (大扭矩, 重载) x1

被动部件:

+ 固定视觉及传感模块 (含安全告警系统)

+ 手库 (多种末端执行器)

+ 临时容器 (陶瓷碗)

+ 带盖的容器 (调料等)

+ 普通工具: (人类使用的) 刀具, 勺子, 筷子 等

+ 加热工具: 锅, 电磁炉 等


## 区域划分

冷区: (任意部位温度不超过 60 摄氏度)

+ 仓库区域

+ 清洗及预处理区域 (含垃圾回收)

+ 临时区域 (临时存储, 以及初步加工, 比如案板)

+ 输出区域 (装盘)

热区: (温度可超过 60 度)

+ 加热区域 (锅 + 电磁炉)


## 执行方式

+ 输入: 固定视觉及传感模块, 可动视觉及传感模块

+ 数据处理和控制: 胖喵小云

+ 输出:
  单臂移动平台 (机械臂) --> 手库 (执行器)
  --> 普通工具 (刀具, 勺子, 筷子, 电磁炉 等)


## 手库

+ 铁锅操纵装置

+ 电磁炉操作装置

+ 刀具操纵装置

+ 勺子操纵装置

+ 筷子操纵装置

+ 陶瓷碗操纵装置

+ 带盖容器操纵装置

+ 仓库操作装置

+ 清洁清洗装置

+ 垃圾收集装置

TODO


## 视觉及传感模块

+ 普通 RGB 摄像头 (含双目立体视觉)

+ 热成像 (红外温度测量)

+ 温湿度传感器

+ 气压传感器

+ 光照传感器

+ 超声波距离传感器

+ 压力传感器 (重量测量)

TODO


## 安全告警系统

+ 多重急停系统

  - 急停按钮 (方便使用长木棍敲击)

  - 网络急停 (断网, 断开有线以太网)

    除了蓝牙急停, 不得使用无线网络 (难以快速切断)

    对主动部件的控制必须通过有线以太网进行 (胖喵小云)

    每条运动命令的持续时间不得超过 100ms (即断网后最多 100ms 会停止运动)

  - 电源急停 (断电, 切断运动的能源)

    不得含有大功率动力电池 (难以快速切断)

  - 蓝牙无线急停 (备用急停装置)

+ 火灾监测

+ 温度过高监测

+ 噪声监测

+ 功率过大监测

+ 破碎及翻倒 (倾泻) 监测

+ 不得使用燃气 (危险性较高)

+ 刀锁 (限制刀具的运动区域)

+ 防逃逸: 防止移动平台跑出厨房门

TODO


## 单臂移动平台

TODO
