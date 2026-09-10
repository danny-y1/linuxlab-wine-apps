# LinuxLab Wine Apps

该仓库是 Linux 用机助手扫描的公开 Windows/Wine 应用目录。

- 机器入口：`linuxlab-apps.json`
- 单应用元数据：`apps/*.json`
- 大文件资源：`assets/**` 分片，由助手通过 GitHub Contents API 下载、逐片校验并重组
- 指定账号来源由产品标记为 `account_trusted`
- `account_trusted` 不代表已经验证 Wine 兼容或完成安装

更新顺序：生成不可变分片、校验每片和最终文件摘要、上传全部分片、远端逐片复验，最后更新 `linuxlab-apps.json`。