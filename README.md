# My Clash Rules

自定义 Clash 分流规则，配合 [sub converter](https://github.com/tindy2013/subconverter) 使用。

## 规则文件

| 文件 | 用途 | 对应 proxy group |
|------|------|------------------|
| `Clash/AdBlock.list` | 广告拦截 | 🍃 应用净化 → REJECT |
| `Clash/Direct.list` | 国内直连 | 🎯 全球直连 → DIRECT |
| `Clash/HK.list` | 香港节点 | 🇭🇰 香港节点 |
| `Clash/Select.list` | 节点选择 | 🚀 节点选择 |

## 使用方法

在 sub converter 的 `custom.ini` 中引用：

```ini
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/576272658/my-clash-rules/main/Clash/AdBlock.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/576272658/my-clash-rules/main/Clash/Direct.list
ruleset=🇭🇰 香港节点,https://raw.githubusercontent.com/576272658/my-clash-rules/main/Clash/HK.list
ruleset=🚀 节点选择,https://raw.githubusercontent.com/576272658/my-clash-rules/main/Clash/Select.list
```

## 更新日志

- 2026-08-08: 新增 `Select.list`，`cf.api.fan` 走节点选择
- 2026-05-01: 初始版本，从自定义 config.ini 提取
