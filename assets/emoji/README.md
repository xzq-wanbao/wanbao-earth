# 游戏 Emoji 图标（无描边）

- 来源：**Twemoji 15.0.3**（Twitter/X，jdecked fork），CC-BY 4.0，仓库 https://github.com/jdecked/twemoji
- 自定义图标：
  - `culture_masks.png`：文化图标（蓝/黄面具），来自 **Noto Color Emoji**（Google，Apache-2.0），缩放到 72×72。
  - `mine_gear_orange.png`：工业区橙色齿轮，由 Twemoji 齿轮重新着色。
- 用途：游戏地图/区域/工程/作物/灾害里用到的图标 emoji 全部保存为本地 PNG（72×72），由 `src/00b-emoji.js` 在 DOM 中替换成 `<img>`、在 Canvas 中用 `drawImage` 绘制。
- 风格：**全部为无描边原图**，因此图标没有黑边，在不同系统/浏览器上显示一致，也不再受系统 emoji 字体影响。
- 映射：字符 → 文件名的对应关系见自动生成的 `src/00b-emoji-data.js`。
- 重新生成（会扫描 `ICONS` / `BUILDINGS` / 作物 / 地图额外图标，并下载缺失图片；`CUSTOM_IMAGES` 里的自定义图标会被保留）：

```bash
node tools/fetch-emoji.js          # 只下载缺失图片并重写映射
node tools/fetch-emoji.js --force  # 强制重新下载全部 Twemoji 图片（不覆盖自定义图片）
```

需要能访问外网；Node 22+ 需要 `NODE_USE_ENV_PROXY=1`（项目运行环境已配置代理时可直接使用）。
