华硕Bios中系统硬盘能识别但是启动顺序里找不到任何硬盘的解决办法

PXE E61
PXE OEF

问题发现:用PE进系统，发现系统C盘中的开机引导盘部分的引导文件只支持普通模式，不支持uefi模式

启动 启动设置 设置模式 将EZ模式改成高级模式

启动 CSM 将从存储设备启动中的UEFI only改成忽略

启动 CSM 将启动设备控制改成UEFI与Legacy Oprom
