# 上传前敏感信息扫描报告

扫描日期：2026-11-09

扫描范围：所有文本类资源文件（跳过图片等二进制文件与 >3MB 文件）。
排除规则：`gh[pousr]_` / `github_pat_` 令牌、Bearer 长串、URL 中带长 token 参数。
占位符（`{{{...}}}`、`${...}`）与域名规则不视为凭据。

## 结果

- 高危命中并隔离：**0** 个文件
- 低风险关键字命中（保留）：**169** 处

## 已隔离（未上传）

无。

## 低风险命中样例（最多 30 条）

- `rule-set/LICENSE`：`authorization`
- `rule-set/custom/crypto.list`：`token.com`
- `wool-scripts/LICENSE`：`authorization`
- `wool-scripts/package-lock.json`：`tokenizer/token":`
- `wool-scripts/README.md`：`token合集'`
- `wool-scripts/boxjs/fmz200_boxjs.json`：`token1\",`
- `wool-scripts/Egern/config/Egern_iOS.yaml`：`token合集`
- `wool-scripts/icons/icons-all.json`：`Password",`
- `wool-scripts/Loon/readme.md`：`token合集'`
- `wool-scripts/Loon/plugin/Auto_Join_TF.plugin`：`Token`
- `wool-scripts/Loon/plugin/blockAds.plugin`：`secretmedia.s3.amazonaws.com,`
- `wool-scripts/Loon/plugin/blockAdsV2.plugin`：`secretmedia.s3.amazonaws.com,`
- `wool-scripts/Loon/plugin/cookies.plugin`：`token合集`
- `wool-scripts/Loon/plugin/WeChatMiniAds.plugin`：`token\/commonSkipToken\/common\/getAdList`
- `wool-scripts/Loon/plugin/split/part!!/AffiliateMarketing.lpx`：`token.rubiconproject.com,`
- `wool-scripts/Loon/plugin/split/partA/Amazon.lpx`：`secretmedia.s3.amazonaws.com,`
- `wool-scripts/Loon/plugin/split/partA/Apple.lpx`：`token.safebrowsing.apple,`
- `wool-scripts/Loon/plugin/split/partD/DongHuaFeng.lpx`：`token|m3u8).php\?`
- `wool-scripts/Loon/plugin/split/partF/Flightradar24.lpx`：`subscribe)`
- `wool-scripts/Loon/plugin/split/partK/KuaiDi100.lpx`：`token.umeng.com,REJECT`
- `wool-scripts/Loon/plugin/split/partQ/QiDianReading.lpx`：`subscribe`
- `wool-scripts/Loon/plugin/split/partS/ShouQiYueChe.lpx`：`token\/leachtoken\/webservice\/homepage\/queryADs`
- `wool-scripts/Loon/plugin/split/partW/Vipshop.lpx`：`api_key`
- `wool-scripts/Loon/plugin/split/partX/Ximalaya.lpx`：`subscribe\/v\d\/subscribe\/tagAlbumList$`
- `wool-scripts/Loon/plugin/split/partZ/ZhangLeCaiFuTong.lpx`：`token`
- `wool-scripts/Loon/rule/Facebook.list`：`secrets.com`
- `wool-scripts/Loon/rule/rejectAd.list`：`token.safebrowsing.apple`
- `wool-scripts/QuantumultX/filter/filter.list`：`token.safebrowsing.apple,`
- `wool-scripts/QuantumultX/rewrite/00-How-To-Use-Rewrite.md`：`token":123},"info":[{"ad":"example.jpg"}],"result":0}`
- `wool-scripts/QuantumultX/rewrite/cleanup.snippet`：`token\/commonSkipToken\/common\/getAdList`
