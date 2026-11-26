# 地球-诸神の黄昏（网页版）

在线游玩：**https://xzq-wanbao.github.io/wanbao-earth/?v=af06c1a**

这个仓库只放网页构建产物（`index.html` + `assets/`），由 GitHub Pages 托管。

## 更新方式

1. 在本地重新运行 `node build.js` 生成 `dist/`
2. 把 `dist/` 里的 **内容**（不是 `dist` 文件夹本身）覆盖到本仓库根目录
3. 提交后 GitHub Pages 会自动重新构建

## 说明

- 存档保存在浏览器的 `localStorage`，与域名绑定；换域名不会带走旧存档
- 音乐文件较大，首次打开会需要一点加载时间
- 浏览器禁止自动播放音乐，进游戏后点左下角音乐按钮
