# 来源说明

抓取日期：2026-11-09　｜　仓库：`tuohai57/resource-mirror`（public）

## 已镜像

| 目录 | 上游 | 许可证 | 文件数 | 体积 |
|---|---|---|---|---|
| `rule-set/` | https://github.com/QuixoticHeart/rule-set | GPL-3.0 | 16 | 0.25 MB |
| `wool-scripts/` | https://github.com/fmz200/wool_scripts | GPL-3.0 | 4852 | 63.60 MB |
| `loonkiss-surge/` | https://github.com/QingRex/LoonKissSurge (surge.qingr.moe) | 未在仓库声明 | 513 | 1.59 MB |
| `yfamilys/` | https://yfamilys.com | 未在站点声明 | 1408 | 18.34 MB |
| `hub-kelee-one/` | https://github.com/luestr/ProxyResource (hub.kelee.one) | NOASSERTION（自定义） | 50 | 16.32 MB |
| `nutrepo/` | https://nutrepo.com（前端 JS 内嵌的模块链接） | 各上游仓库各自声明 | 61 | 0.24 MB |
| `ddgksf2013-top/` | https://ddgksf2013.top | 未在站点声明 | 2 | 0.10 MB |

## 未镜像及原因

- `github.com/fmz200`（用户主页）：名下 11 个仓库合计 >1.2 GB，多数与代理配置无关；本次只取明确指定的 `wool_scripts`。
- `nutrepo.com`：页面本身为 Next.js 动态渲染，但资源链接硬编码在前端 JS chunk 中，已提取并镜像到 `nutrepo/`。其中 3 条 `NSRingo/LocationService` 链接的上游仓库已删除（API 404），无法取得；`BiliUniverse/Enhanced` 与 `NSRingo/WeatherKit` 的 release 资产名与站点写法不符，已按上游实际名称更正后下载。
- `ddgksf2013.top`：纯导航站，无本站托管的配置文件；已把页面 119 个外链整理为 `ddgksf2013-top/links.json`，并镜像了其中唯一一个 gist 脚本。其 Supabase 仅用于 `counters` 访问计数，不含资源数据。
- `surge.qingr.moe`：目录索引页，所列 512 个 `.sgmodule` 均来自 `QingRex/LoonKissSurge`，已由 `loonkiss-surge/` 覆盖，未重复抓取。
- 网页 HTML 快照、CSS/图片等网页资产、订阅链接、机场推广内容：一律不镜像。
- `README-RULE.md` 的 733 条规则列表已解析为结构化索引 `rule-index.json`（含 Raw / Loon / QuanX / Surge / Egern 各类安装链接）。

## 许可证与署名

- `QuixoticHeart/rule-set` 与 `fmz200/wool_scripts` 均为 **GPL-3.0**，许可证原文见 `licenses/`。再分发需保留许可证与来源标注。
- `QingRex/LoonKissSurge` 与 `yfamilys.com` 未在仓库／站点声明许可证，版权归原作者。
- `luestr/ProxyResource` 为 NOASSERTION 自定义许可，原文见 `licenses/`。

## 使用

```
https://cdn.jsdelivr.net/gh/tuohai57/resource-mirror@main/<路径>
```

原始 URL 与本地路径的对应关系见 `manifest.json`。
