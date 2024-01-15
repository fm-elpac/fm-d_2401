# FMMB-3
胖蚊 PCBA 工艺柜: 微型自动化产线 (非化学工艺)

+ 一个工艺柜实现 PCBA (PCB+SMT) 完整工艺, 全自动化

+ 总成本 1 万元以内


## 工艺名称

+ `FMMB-100p` 精度 100um 非化学多层 PCBA 工艺


## 工艺参数

+ 精度: 0.1mm (线宽线距, 过孔)

+ 大小: 200x200mm

+ 层数: 2 / 4 / 6 / 8

+ 材料: FR-4 玻纤板, 热电分离铜基板

+ 铜厚: 最低 0.1mm


## 主要设备 (8)

+ 密封防火机架

  宽 0.5m, 高 2.5m (3 层), 长 2m

  不锈钢方管支架, 背部/底部不锈钢薄板,
  前方/左侧/右侧钢化玻璃, 顶部亚克力板+塑料水箱

  顶部风道+风扇, 风管直连室外, 底部风道+空气过滤器

+ FMDP-4 胖蚊黑蜘蛛

  2 只机械臂, 机架内定制型号, 自动化整个流程

+ 小铣床 (自动换刀/对刀): 钻孔, 线路成形, 锣边

+ 热处理机: 真空层压, 热固化, 回流焊

+ 针管涂写机: 阻焊, 丝印, 锡膏

  点胶针头+注射器 设计, 自动换笔, 支持打印多种材质, 最细线宽 0.1mm

+ 铜丝点焊机: 过孔铜丝

+ 飞针测试机: 4 线低阻测试

+ 贴片机: 元件放置


## 测试

+ 光学检测

+ 飞针测试

  - 完全测试 (多遍测试)

  - 不完全测试

    先测连通, 再测断开.
    连通区域生长法, 最长线路法.


TODO