# 设备接入服务

**商业物联管理系统针对安卓设备提供了全面的接入支持，支持免开发接入，针对设备厂商系统权限的不同开放方式，提供了对应的解决方案：**

| 厂商系统权限开放方式 | 商业物联管理系统接入适配方案 | 支持能力说明                             |
|-----| ------------------------- |-------------------------------------|
| 支持系统签名 | 系统签名版的IoT助手APP | 支持所有能力 |
| 提供系统权限授权范围 | 厂商专属IoT助手APP | 支持厂商授权的相关能力 |
| 提供ROOT权限 | 硬件厂商授予IoT助手ROOT权限 | 支持所有能力 |
| 不开放 | 普通权限的IoT助手APP | 降级能力 |

备注：

[1]	系统签名版的IoT助手APP核心代码面向设备厂商开源，确保系统签名的代码透明可信赖；

[2]	需要系统签名支持的能力包括：重启设备/静默安装升级应用/定时开关机/拉取设备日志/远程协助/截屏/停用应用/应用前台运行等；

**接入步骤：**
1)	登录商业物联管理系统（控制台-->服务管理-->点击使用此服务，即可进入到商业物联管理系统）根据系统权限开放方式，下载对应的IoT助手；
2)	在设备出厂前，将IoT助手预装到设备中，有条件的厂商可将IoT助手设为开机自启；
3)	开机启动IoT助手时，设备自动激活入网；

## 设备接入安全机制
1) 一机一密：设备和平台进行双向证书验证后，建立安全的数据通道进行数据传输；
2) 支持国密SM4、SM2算法加密，确保数据传输安全合规;
3) 采用白名单机制杜绝非法设备动态注册；
4) 支持设备重复激活开关配置；

## 设备接入稳定机制
1)	支持双进程互相保活；
2)	通过备份通道实现连接异常恢复；
3)	通过自动识别网络环境实现长连接推送和短连接轮询机制自动切换；

