# 雷速体育去广告 · Loon 插件

拦截雷速体育 iOS（`com.leisu.sports`）内嵌聚合广告 SDK 的网络请求：开屏 / 插屏 / Banner / 信息流 / 激励视频。

域名列表提取自 11.2.2 主程序的静态分析（Sigmob、倍孜 Beizi、AdGain、AdScope、OctAd/整数、JT 章鱼移动、TopOn/AnyThink、Ubix、TapTap、Tanx、穿山甲、优量汇、友盟归因等），纯域名 REJECT，**无需 MITM 证书**。

## 安装（Loon）

配置 → 插件 → 右上角 + → 从 URL 安装：

```
https://raw.githubusercontent.com/am-tmac/leisu-adblock/main/leisu-adblock.plugin
```

国内或 raw 被墙时用 jsDelivr 镜像：

```
https://cdn.jsdelivr.net/gh/am-tmac/leisu-adblock@main/leisu-adblock.plugin
```

Stash / Quantumult X / Shadowrocket 用户可自行按 `[Rule]` 段转换，规则均为标准 `DOMAIN-SUFFIX, xxx, REJECT`。

## 说明与边界

- 域名来自静态二进制分析，**没有真机抓包全量验证**。漏网的广告 SDK 域名欢迎提 issue 或 PR 补充。
- 服务端和正常内容混在同一接口下发的内容型广告拦不掉。
- 本插件只拦网络请求；不走网络或已缓存的开屏素材可能仍会短暂出现。
- 规则不针对任何厂商，仅供学习交流与个人去广告使用。

## License

MIT
