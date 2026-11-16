# simpleppt

把 PDF 课件中的重复标题与正文保守合并，整理为连贯复习讲义。暖白与暗红界面，支持电脑、平板和手机。

网站地址：https://chengyulian0228-debug.github.io/yejian/

## 文件在你的浏览器里处理

选择文件后，PDF.js 与 pdf-lib 在浏览器本地读取、整理和导出 PDF，不上传课件，不调用 AI 服务。历史记录仅存入当前浏览器，建议及时下载讲义。首次打开需要加载网站与开源字体。

支持均衡、紧凑、批注留白版式；支持保留原页眉、主色或纯正文风格；可选页码范围与来源显示。扫描页和复杂图像页保留原页图像，不含 OCR。自动识别受 PDF 的结构影响，下载前请使用对比预览。

## 源码和更新

`source.zip` 是完整、可构建的前端源码包，内含 README、测试、字体许可及依赖锁文件。解压后运行：

```sh
npm ci
npm test
npm run dev
npm run build
```

GitHub Actions 会在推送后解压源码、运行测试、构建并部署 GitHub Pages。更新时上传新的 `source.zip` 即可。源码包不包含任何用户课件或历史记录。

中文字体采用 SIL Open Font License 1.1，详见源码包 `public/fonts/OFL.txt`。
