# PMMC-2
胖喵缓存镜像: 简单的本地缓存镜像服务.

A very simple and small auto cache mirror server.

正式名称: 紫腹巨蚊 () 系列 红皮土豆 (Solanum tuberosum) 系统

+ 推荐域名: `*.mc.pmlz.test:52406`

超小, 超简单的自动化本地缓存镜像.
适用于不超过 100 台设备的小型局域网.

+ 参考实现 (镜像站): <https://mirror.sjtu.edu.cn/>

+ 发布 github (容器镜像): fm-elpac/pmmc2

+ 配置文件: 本地 JSON

  无需登录管理后台 (页面为非特权页面).
  (最简单的登录就是无需登录)


## 功能特性 (feature)

+ 自动缓存 (HTTP)

+ 定期自动更新 (默认 60 分钟)

  自动下载新版软件包

+ 下载统计与自动清理

  - 清理旧版本软件包 (默认 30 天)

  - 移除没有使用 (下载) 的软件包 (默认 180 天)

+ 存储空间统计, 日志记录


## 技术栈

+ deno <https://deno.com/>

  (TypeScript)

+ fresh <https://fresh.deno.dev/>

### 数据库和文件目录

+ 配置文件 (默认): `/etc/pmmc2/pmmc2-conf.json`

  环境变量: `PMMC2_FP_CONF`

+ 主数据目录 (默认): `/var/lib/pmmc2`

  环境变量: `PMMC2_DIR_DATA`

+ 运行目录 (默认): `/run/pmmc2`

  环境变量: `PMMC2_DIR_RUN`

数据库技术: deno-kv <https://deno.com/kv>

+ 主数据库 (缓存数据库): PMMC2_DIR_DATA`/db/pmmc2.db`

+ 运行数据库 (临时数据): PMMC2_DIR_RUN`/pmmc2-run.db`

+ 日志数据库 (日志数据): PMMC2_DIR_DATA`/db/pmmc2-log.db`

文件存储目录 (本地存储后端):

+ 临时目录 (部分下载文件): PMMC2_DIR_DATA`/tmp/**/*.dl`

+ 缓存目录 (软件包): PMMC2_DIR_DATA`/cache/NAME/*`

配置文件格式 (示例):

```json
{
  "global": {
    "dn": "*.mc.pmlz.test:52406",
    "update_m": 60,
    "update_min": 2,
    "rm_old_d": 30,
    "rm_unuse_d": 180,
    "dl_t": 8
  },
  "mirror": {
    "archlinux": {
      "upstream": [
        "TODO"
      ],
      "url": "https://mirror.sjtu.edu.cn/docs/archlinux"
    }
  }
}
```


## 支持镜像

+ 容器镜像 (docker ?)

  TODO

  - gcr.io 上游: <https://mirror.sjtu.edu.cn/docs/gcr.io>

+ ArchLinux (pacman)

  上游:
  - <https://mirror.sjtu.edu.cn/docs/archlinux>
  - <https://mirror.tuna.tsinghua.edu.cn/help/archlinux/>

+ flathub (flatpak)

  上游: <https://mirror.sjtu.edu.cn/docs/flathub>

+ f-droid (apk)

  上游: <https://mirror.tuna.tsinghua.edu.cn/help/fdroid/>

+ termux (apt)

  上游: <https://mirror.tuna.tsinghua.edu.cn/help/termux/>

+ crates (rust/cargo)

  上游:
  - <https://mirror.sjtu.edu.cn/docs/crates.io>
  - <https://mirror.tuna.tsinghua.edu.cn/help/crates.io-index/>

+ rust-static

  上游: <https://mirror.sjtu.edu.cn/docs/rust-static>

+ github-release

  上游: <https://mirror.tuna.tsinghua.edu.cn/github-release/>

+ npm

  上游: <https://mirror.sjtu.edu.cn/docs/npm-registry>

+ pypi (python)

  上游: <https://mirror.sjtu.edu.cn/docs/pypi-packages>

+ fedora-ostree

  上游: <https://mirror.sjtu.edu.cn/docs/fedora-ostree>

+ armbian

  上游: <https://mirror.sjtu.edu.cn/docs/armbian>

+ debian (apt)

  上游: <https://mirror.sjtu.edu.cn/docs/debian>

+ ubuntu (apt)

  上游: <https://mirror.sjtu.edu.cn/docs/ubuntu>

+ fedora (RPM)

  上游: <https://mirror.sjtu.edu.cn/docs/fedora/linux>

+ google-fonts

  上游: <https://mirror.sjtu.edu.cn/docs/google-fonts>

+ OpenWrt

  上游: <https://help.mirrors.cernet.edu.cn/openwrt/?mirror=SJTUG-Siyuan>

  TODO


TODO
