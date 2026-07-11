# ⚠️ 此项目非官方项目，实现为第三方实现
# 仍在开发阶段，出现问题请反馈

# 皎月连修改版

自用的皎月连第三方改版，做了部分修改

本项目不是官方客户端，不代表官方立场，也不提供官方支持

## 主要功能

见皎月连：[www.natpierce.cn](https://www.natpierce.cn)

## 和官方客户端的区别

不使用全局接管流量的方式进行组网，虚拟组网入口改为 SOCKS5，适合给浏览器、开发工具、代理软件或支持 SOCKS5 的应用单独配置使用

平均性能比原版应用高 3-5 倍

## 使用方式

下载对应平台的 Release 压缩包，解压后运行：

```powershell
# 启动程序
.\natpierce-compat.exe

# 查看启动参数
.\natpierce-compat.exe help

# 指定配置文件路径
.\natpierce-compat.exe --config .\config
```

默认情况下，程序会读取同目录下的 `config`。如果没有 `config`，会以空白本机配置启动；登录或保存设置后会创建配置文件

`config` 与官方客户端兼容，你可以直接将此程序放到官方客户端文件夹下替代使用

Windows 下支持开机自启，其他平台请自行配置。

仅在 Windows 下有托盘。

## 注意事项

- 当前主要面向 Windows/Linux 使用；macOS 平台构建产物未做测试
- 本项目按现状提供，不保证适合所有网络环境
