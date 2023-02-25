# openwrt-actions

通过GitHub Actions自动编译Openwrt

`feeds.conf.default`配置需要的软件源

`.config`编译配置

通过`make menuconfig`或`make defconfig`生成`.config`文件，该文件为全量配置文件

通过`./scripts/diffconfig.sh > .config`生成`.config`文件，该文件为差异化配置文件

`diy-part1.sh`可以进行修改软件源等操作

`diy-part2.sh`可以修改其他配置

## 运行方式

点击`Actions`，在左侧选中需要运行的`workflow`，点击右侧`Run workflow`，等待2～3小时，即可在此处下载镜像
