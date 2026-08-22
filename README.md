# CatAssistant 游戏素材仓库

CatAssistant（小猫桌面助手）「游戏」tab 的联网素材仓库。app 启动后拉取 `manifest.json`，异步下载各游戏的美术与音频素材并缓存到本地；下载失败或离线时，回退到 app 内置的兜底美术，游戏始终完整可玩。

## 目录结构

```
manifest.json          # 素材清单：版本号 + 每款游戏的素材表
assets/<game-id>/      # 每款游戏一个目录
  art/                 # 图片素材
  audio/               # 音效 / 背景音乐
```

## 约定

- 只收录 CC0 / 免版权素材，或用代码生成的自制素材
- 修改素材后 `commit + push` 即可生效，无需重新发 app
- 建议通过 jsDelivr CDN 访问（免缓存问题）：
  `https://cdn.jsdelivr.net/gh/<用户名>/catassistant-game-assets@main/manifest.json`
