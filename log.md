# 修改日志

## 2026-11-12 重新标识为 goofish-yao-cli

- 项目从上游 `goofish-cli` 改为所有者自己的 CLI：PyPI/项目名 `goofish-yao-cli`，命令 `goofish-yao`，MCP 入口 `goofish-yao-cli`（别名 `goofish-yao-mcp`）。
- 默认状态目录改为 `~/.goofish-yao-cli`，环境变量前缀改为 `GOOFISH_YAO_`。
- Cookie 加密仍使用 Fernet + PBKDF2，salt 和机器密钥后缀改为本 fork 专用，不能解密上游 `~/.goofish-cli` 的 cookie。
- 仓库、插件和文档链接改为 `https://github.com/yaoyunchou/goofish-yao-cli`。项目元数据作者为 yaoyunchou，已去掉上游邮箱。
- 删除上游推广素材（IPWO 联盟横幅、优惠码、宣传海报/视频/GIF）。Apache-2.0 与 NOTICE 中的上游版权保留，并注明本 fork 的修改由 yaoyunchou 完成。
- Python 导入包由 `goofish_cli` 改为 `goofish_yao_cli`。业务接口、签名和命令行为未改。
