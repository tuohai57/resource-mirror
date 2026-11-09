# 来源说明

抓取日期：2026-11-09　｜　仓库：`tuohai57/resource-mirror`（public）

## 已镜像

| 目录 | 上游 | 许可证 | 文件数 | 体积 |
|---|---|---|---|---|
| `rule-set/` | https://github.com/QuixoticHeart/rule-set | GPL-3.0 | 16 | 0.25 MB |
| `wool-scripts/` | https://github.com/fmz200/wool_scripts | GPL-3.0 | 4851 | 63.60 MB |
| `loonkiss-surge/` | https://github.com/QingRex/LoonKissSurge (surge.qingr.moe) | 未在仓库声明 | 513 | 1.59 MB |
| `yfamilys/` | https://yfamilys.com | 未在站点声明 | 1408 | 18.34 MB |
| `hub-kelee-one/` | https://github.com/luestr/ProxyResource (hub.kelee.one) | NOASSERTION（自定义） | 50 | 16.32 MB |

## 未镜像及原因

- `github.com/fmz200`（用户主页）：名下 11 个仓库合计 >1.2 GB，多数与代理配置无关；本次只取明确指定的 `wool_scripts`。
- `nutrepo.com`：Next.js 动态渲染，页面无内嵌资源文件，数据在后端接口后，未做接口逆向。
- `ddgksf2013.top`：资源导航站，页面内 119 个链接均指向第三方站点，没有本站托管的配置文件。
- `surge.qingr.moe`：目录索引页，所列 512 个 `.sgmodule` 均来自 `QingRex/LoonKissSurge`，已由 `loonkiss-surge/` 覆盖，未重复抓取。
- 网页 HTML 快照、订阅链接、机场推广内容：一律不镜像。

## 许可证与署名

- `QuixoticHeart/rule-set` 与 `fmz200/wool_scripts` 均为 **GPL-3.0**，许可证原文见 `licenses/`。再分发需保留许可证与来源标注。
- `QingRex/LoonKissSurge` 与 `yfamilys.com` 未在仓库／站点声明许可证，版权归原作者。
- `luestr/ProxyResource` 为 NOASSERTION 自定义许可，原文见 `licenses/`。

## 使用

```
https://cdn.jsdelivr.net/gh/tuohai57/resource-mirror@main/<路径>
```

原始 URL 与本地路径的对应关系见 `manifest.json`。
