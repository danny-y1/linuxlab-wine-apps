# LinuxLab Wine Apps

该仓库是 Linux 用机助手扫描的公开 Windows/Wine 应用目录。

- 机器入口：`linuxlab-apps.json`
- 单应用元数据：`apps/*.json`
- 安装文件：GitHub Releases
- 指定账号来源由产品标记为 `account_trusted`
- `account_trusted` 不代表已经验证 Wine 兼容或完成安装

更新顺序：创建不可变 Release、上传 asset、复验远端 SHA-256，最后更新 `linuxlab-apps.json`。