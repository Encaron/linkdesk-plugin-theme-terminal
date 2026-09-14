# 更新日志

## v1.0.5（2026-09-15）

- 配方 `$schema` 改**文档唯一认可的写法**（`./node_modules/@linkdesk/plugin-sdk/schemas/theme.schema.json`，相对工程根）——原来用的是已作废的越界相对路径（`../..` 一路指到壳仓 `public/schemas/`，脱离壳仓后编辑器的补全与校验全失效）
- 分发件随包带 **MIT 许可证**（`LICENSE`）——MIT 要求副本里带版权声明，而 zip 才是用户真正拿到的那份
- 新增 `AGENTS.md`：在这个仓里单开 AI 干活时的进场说明（这只插件是什么 / 规矩在哪 / 命令怎么敲）

## v1.0.4（2026-09-14）

- 源码迁入独立仓（E6#99，L7 第 7.2 轮）——从壳仓 `Encaron/linkdesk` 抽出本插件子树，历史全保（hash 变）
- 随包 `plugin.json` 显式声明 `pluginId`（E6#98g）：插件身份不再靠目录名兜底，独立仓构建出的包名与身份稳定
- `$schema` 改指本仓 `node_modules/@linkdesk/plugin-sdk`（脱离壳仓后原相对路径指到仓外，编辑器补全/校验会失效）


## v1.0.3（2026-09-11）

- 更新记录迁入包内的 `CHANGELOG.md`（E6#92 元数据归一）——此前写在 `plugin.json` 的 `changelog` 字段里，市场详情页读不到

## v1.0.2（2026-09-09）

- 图标身份分工（E6#69 三图模型）：新增 icon=resources/icon.svg（Type-2 彩色身份图），撤 marketIcon=cover.svg——整幅封面迁入 README 展示
