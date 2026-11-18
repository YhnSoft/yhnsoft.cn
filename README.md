# yhnsoft.cn

一块旋转鸡块，部署在 Cloudflare Workers 静态资源（Workers Static Assets）上。

线上地址：<https://yhnsoft.cn/>

## 本地预览

直接用浏览器打开 `index.html` 即可，页面零依赖、自包含。

## 部署

```bash
npx wrangler deploy
```

`wrangler.jsonc` 中的 Worker 名为 `yhnsoft-cn`，根域 `yhnsoft.cn` 已通过
Worker 自定义域名绑定到该 Worker。静态资源目录为仓库根目录，
`.assetsignore` 控制不随站点发布的文件。
