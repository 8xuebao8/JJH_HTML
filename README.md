
````markdown
# 耳环佩戴比例视觉化工具
# Earring Proportion Studio

为珠宝设计阶段提供耳环长度与佩戴比例的直观参考。

**在线体验 / Live demo**  
https://8xuebao8.github.io/JJH_HTML/

## 功能

- **中英文切换**：整体界面切换，自动记住语言选择。
- **本地图片处理**：支持 PNG、JPG/JPEG，点击上传或拖放。
- **两点标定**：手动设置悬挂点和最低点，排除图片上下留白。
- **佩戴预览**：人物背景、动态标尺、可调整耳垂位置。
- **长度调节**：2–15 cm，步长 0.5 cm，支持滑块、数字输入和快捷按钮。
- **旋转与比较**：佩戴角度 ±15°；A/B 独立调整长度。
- **图片编辑**：裁切、左右旋转 90°、水平及垂直镜像。
- **取色去底**：颜色容差实时生效，支持清除不相连的同色区域。
- **细节修补**：擦除、恢复、撤销、原图对比及 PNG 下载。
- **响应式布局**：支持电脑和手机操作。

## 使用方法

1. 上传耳环图片，或点击「使用示例耳环」。
2. 如需去底，打开「编辑图片」，吸取背景颜色并调整颜色容差。
3. 点击「设置挂点与最低点」，分别标记耳环的悬挂点和最低点。
4. 输入两点之间的实际垂直长度，查看佩戴效果。
5. 根据需要调整耳垂位置、旋转角度，或比较两个长度。

取色后，增大容差会去除更多相近颜色，调小会恢复本次多去除的部分。
切换画笔或重新取色会保留当前结果；误操作可撤销。

裁切、旋转或镜像后，请检查标定点。如果两点不再有效，
工具会恢复默认位置并提示重新标定。

## 本地运行

项目为单文件 `index.html`，使用 HTML、CSS 和原生 JavaScript。
无需安装依赖，无需构建，直接使用现代浏览器打开即可。

也可在项目目录启动本地静态服务器：

```bash
python3 -m http.server 8000
```

然后在浏览器中访问本地服务器的 8000 端口。

## 部署与更新

本项目使用 GitHub Pages：

- 发布分支：`main`
- 发布目录：仓库根目录 `/`
- 推送到 `main` 后，GitHub Pages 自动重新部署。

可在仓库的 Actions 页面查看部署进度。
若页面仍显示旧版，请等待部署完成后刷新。

## 隐私与使用限制

上传图片在浏览器中处理，不上传到服务器。
语言偏好保存在浏览器本地。

纯色、浅色背景更适合取色去底。珍珠、高光、细链条和透明宝石
可能被误删，可通过降低容差、恢复画笔或撤销修正。

人物与标尺仅用于视觉比例参考，不代表精确的人体测量或实际佩戴效果。
输入长度按标定两点的垂直距离计算，不是沿耳环轮廓测量的长度。

刷新或关闭页面前，请下载需要保留的编辑图片；
图片和编辑进度不会自动保存。

## English

A lightweight, browser-based tool for exploring earring length and wearing
proportions during jewelry design.

### Features

- Chinese/English interface with a remembered language preference.
- Local PNG/JPEG uploads and automatic empty-edge trimming.
- Manual hanging-point and lowest-point calibration.
- Adjustable earlobe position, live ruler, and 2–15 cm length controls.
- ±15° wearing rotation and independent A/B length comparison.
- Crop, 90° rotation, horizontal and vertical flipping.
- Background color picking with reversible live tolerance.
- Erase/restore brushes, undo, original comparison, and PNG export.
- Desktop and mobile layouts.

### Quick start

Upload a design, optionally edit its background, and mark its hanging and
lowest points. Enter the real vertical distance between these points,
then adjust the preview or compare two lengths.

Open `index.html` directly in a modern browser, or run the Python static
server shown above. No dependencies or build step are required.

Images are processed locally and are not uploaded. Only the language
preference is persisted; export edited images before refreshing or closing
the page.

This tool provides visual proportion reference, not precise measurements
or a guarantee of actual fit.
````
