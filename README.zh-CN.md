# Phone Use Skills

[English](README.md) | **简体中文**

[Phone Use](https://github.com/nidhoggfgg/PhoneUse) 的可安装 agent Skills，用于观察和操作 Android 手机。本仓库只包含 Skill 及其运行文件，安装时无需下载 Android 源码和主项目的 Git 历史。

## 安装

```sh
npx skills add nidhoggfgg/phone-use-skills --skill phone-use
```

按提示选择 AI 客户端与安装范围。电脑需要 Node.js 22.20+、Git 和 Python 3.10+。手机运行 Phone Use 服务，电脑能通过局域网访问手机，首次配对由用户在手机批准。

然后让 AI 执行：

> 使用 $phone-use 连接 http://192.168.1.20:8443，显示核对码，等我在手机批准后查看当前界面。

详见 [Skill 中文说明](phone-use/README.zh-CN.md)和[安装指南](https://github.com/nidhoggfgg/PhoneUse/blob/main/docs/integrations.zh-CN.md)。

## 维护

主仓库通过 `skills/` Git 子模块引用本仓库。Python 客户端和 API 参考以主仓库中的文件为源，修改后在主仓库运行 `python tools/sync_skill.py`。先在本仓库提交并推送，再在主仓库提交更新后的子模块指针。详见[贡献指南](https://github.com/nidhoggfgg/PhoneUse/blob/main/CONTRIBUTING.zh-CN.md)。

采用 [MIT 许可证](LICENSE)。
