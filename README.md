# android_root_caps

## 系统改造

0. 加虚拟内存减少 app 冷启动 swapon /data/swapfile
1. 设置 /proc/sys/vm/swappiness (减少后台被回收 vs 大型 app 冷启动慢) t/1070045
2. 改 OOM 机制 /sys/module/lowmemorykiller/parameters/minfree
3. setprop persist.adb.tcp.port 5555 方便远程 adb.
4. 把 TF 卡挂载到/sdcard/Android 扩容 (TF 速度会影响性能)
5. 把 NAS 挂载到/sdcard/nas 当本地硬盘 (非 wifi 环境慎用)
6. 刷面具模块（系统去广告、主题破解），钛备份、脚本全量备份，刷内核，刷调度，黑域绿色守护，xp 框架（修改 app ），写轮眼（禁用 app 服务）
7. 息屏收 fcm 通知

## 特色应用

8. 看家/娃: 闲置手机自动接听视频电话. [t/1066631](https://www.v2ex.com/t/1066631)
9. [在 pixel 启用电信 LTE](https://github.com/cxOrz/pixel_ims_module)
10. [在 pixel 启用支付宝指纹](https://github.com/eritpchy/FingerprintPay)
11. [appops，更方便的管理权](https://appops.rikka.app/zh-hans/)
12. 存储空间隔离
13. 调度 [Thanox](https://tornaco.github.io/Thanox-Docs/zh/)  Scene
14. 美化（ iconify ）
15. 功能增强（ QAuxiliary 、Wxposed 、freedom+、mipush ）
16. 用 rclone 可以挂 samba, 版本是 v1.66.0-termux
17. 安装 acc 控制充电保护电池
18. 安装 lsposed 刷去 x 广告模块
19. 安装 revanced 去除油管广告
20. 安装 core patch 允许降级安装 app
21. 安装 fake location 虚拟定位
22. 数据备份
23. macrodroid/tasker 自动化
24. Hook App QAuxiliary FunBox Freedom TMoe 快捷切换 5G 伪装 Piexl 等
25. Acc 充电达到阈值断开
26. FakeIP 透明代理
27. YC 调度 Scene
28. 电池解容
29. rom 定制包 Flyme 原生
30. Fakelocation 虚拟定位
31. MT 管理器
32. 核心破解
33. Revanced 添加跳 y2b 广告片段功能
34. VCAM 虚拟摄像头 线上考试帮了不少忙
35. NFC 模拟 可以破解系统钱包限制模拟
36. 芝麻粒 实现支付宝自动化
37. 隐藏应用列表 防止某些软件偷看苦茶子
38. 拒绝强制亮度
39. 潘多拉核心 增加续航。
40. AdClose
41. fcmfix 修复 fcm
42. XposedSmsCode 自动提取验证码输入等
43. 游戏: CPU 锁频, 避免手机过热降速运行, 注意散热, 注意散热.
44. NAS: 挂硬盘跑 alist, BT, syncthing 等, 注意供电和散热.
45. screencam 录屏内录音频，解除 flag secure 截屏限制，ida pro 动态调试
46. 安装 [bromite webview](https://github.com/bromite/bromite/wiki/Installing-SystemWebView)

