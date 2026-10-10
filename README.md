# Animal Encyclopedia — paxton

交互式 Three.js / WebGL 古籍。公开体验：
https://chamaeleon-living-manuscript.citruslion32.chatgpt.site/

## 直接使用

公开网址无需账户或登录，可在支持 WebGL 的电脑和手机浏览器中访问。
点击屏幕打开古书；电脑鼠标经过即显色，停住会逐渐扩散。全部显色保持 5.1 秒后恢复。
手机支持轻触开书、轻触书页显色与按压，不模拟鼠标悬停。

## 网站文件

根目录 index.html、main.js、style.css 与 assets/ 即完整网站，全部依赖本地托管，无需数据库、API 密钥或构建步骤。
可以原样上传 GitHub Pages、Cloudflare Pages、Netlify 等静态托管，发布目录选根目录。
所有资源使用相对路径，支持 GitHub 项目子目录。

## GitHub Pages

上传本包全部文件后，在仓库 Settings → Pages 中选择 Deploy from a branch，选择 main 分支和 / (root)，保存。
GitHub Pages 发布后，访问 https://你的用户名.github.io/仓库名/。

## 本地预览

运行 python3 -m http.server 4173，然后打开 http://localhost:4173。
offline.html 是全部资源内嵌的独立版本，可以尝试双击打开。该版本已通过 HTTP 运行检查；自动浏览器不允许 file: 协议，因此双击模式未完成自动实测。手机建议使用上方公开网址。

## 授权与来源

Three.js r180 使用 MIT 许可；Cormorant Garamond 使用 SIL Open Font License 1.1；完整许可见 licenses/。
插画、纸张及装饰为生成素材，来源与提示词见 ASSETS.md、asset-prompts.json。
模型是程序构建的古籍，树与动物是同轮廓配准的生成插画与浅浮雕材质，并非博物馆实物扫描或独立动物模型。
