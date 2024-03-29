# 胖喵小窝 硬件配置需求: 网络, 计算, 存储

(pmlz-1 hw-ncs)

(2024-01)


## 典型配置

+ (网关) **wifi 6 无线路由器** (必需)

  参数要求:
  - 1Gbps 以太网口: 至少 2 个
  - 支持 WPA3 加密
  - 支持 wifi 6 (802.11ax)

  推荐型号:
  TODO

+ 中心交换机 (必需)

  参数要求 (基础配置):
  - 1Gbps 以太网口: 24 个及以上
  - 支持 VLAN (802.1q), 链路聚合

  推荐型号:
  TODO

  高配:
  - 2.5Gbps 以太网交换机
  - 10Gbps 光纤以太网交换机 (SPF+)

+ **副服务器** (second server) (必需)

  单板机 (SBC)

  参数要求:
  - 内存: 1GB 及以上
  - 存储: 16GB 及以上 (可以使用 SD 卡)
  - 1Gbps 以太网口
  - 操作系统: 支持 Debian 12 (aarch64)
  - (推荐) HDMI 接口: 支持 1080p 视频输出

  推荐型号:
  - (便宜) 香橙派 Orange pi Zero3 (内存 1GB/4GB, 处理器 H618)
  - (高配) 香橙派 Orange pi 5 (内存 8GB/16GB, 处理器 rk3588)

+ **存储服务器** (推荐)

  2U 服务器, 至少 2 台

  参数要求:
  - 3.5 英寸硬盘位: 12 个
  - 内存: 16GB 及以上

  推荐型号 (二手):
  TODO


TODO
