# win12-theme

此仓库存放了 Win12 网页版的主题文件

> [!NOTE]
> [原主题仓库](https://codeberg.org/win12-online/win12-theme-legacy) 已弃用，此仓库为整理并压缩图片后的新版仓库

## 贡献主题

你的主题文件夹应该位于 `themes` 目录下，文件夹名应为全英文小写且采用 kebab-case 格式（也就是使用连字符分隔单词）。

在主题文件夹内，上传两个图片文件：

- `background.webp`: 桌面背景图片（最短边应当长于 250-300px）
- `thumbnail.webp`: 背景缩略图（图片大小尽量小一些）

这两个图片都**必须为 WebP 格式**，且图片大小不宜过大。

> 93MiB 压缩到 8.4MiB，WebP 科技恐怖如斯  
> -- [lingbopro](https://codeberg.org/lingbopro)

接下来在主题文件夹内创建 `theme.json`：

```json
{
  "name": "示例", // 主题名称
  "colors": {
    "color1": "#c66f62", // 渐变主题色
    "color2": "#0167bc", // 渐变主题色
    "href": "#4cc2ff" // 主题色（我也不知道为啥叫href，tjy的小巧思说是）
  }
}
```

（注：实际文件中不应包含注释，因为 JSON 标准不允许注释）

`theme.json` 文件需使用 Prettier 格式化。
