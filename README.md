# resource-mirror

第三方代理配置资源镜像。按来源分目录，只保存**会被配置实际引用的资源文件**（规则集、模块、脚本、图标），不含网页快照、订阅凭据或机场链接。

## 访问前缀

```
https://cdn.jsdelivr.net/gh/tuohai57/resource-mirror@main/<路径>
https://raw.githubusercontent.com/tuohai57/resource-mirror/main/<路径>
```

jsDelivr 只能读公开仓库，本仓库为 public。

## 目录结构

| 目录 | 上游来源 |
|---|---|
| `rule-set/` | `QuixoticHeart/rule-set`（GPL-3.0） |
| `wool-scripts/` | `fmz200/wool_scripts`（GPL-3.0） |
| `loonkiss-surge/` | `QingRex/LoonKissSurge`，即 `surge.qingr.moe` 目录页所列文件 |
| `yfamilys/` | `yfamilys.com` 的 `/rule/*.list` 规则集 |
| `hub-kelee-one/` | `luestr/ProxyResource`，`hub.kelee.one` 插件中心的数据仓库 |
| `manifest.json` | 原始 URL → 本地路径 的映射表 |
| `SOURCES.md` | 来源、许可证、抓取时间、未镜像项说明 |
| `SCAN_REPORT.md` | 上传前的敏感信息扫描结果 |
| `licenses/` | 上游 GPL-3.0 许可证原文 |

## 约定

- 文件按原始字节保存，仓库通过 `.gitattributes`（`* -text`）禁用 CRLF 转换。
- 不要改名、不要改目录名：`manifest.json` 依赖固定路径映射。
- 上游许可证与来源标注必须保留；GPL-3.0 仓库的派生/再分发需遵守其条款。

## 免责

本仓库仅为个人配置引用的资源镜像，内容版权归各上游作者所有。若上游作者不希望被镜像，请提交 issue，会立即移除对应目录。
