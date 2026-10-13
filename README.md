# China Province SVG Icons

中国省级行政区 SVG 图标，适合在地点、旅行记录、生活随笔和地图界面中使用。

## 内容

- `china-provinces.svg`: 完整的中国省级行政区地图源文件。
- `provinces/`: 从源文件中提取的 33 个省级行政区轮廓图标。

每个单独图标都经过紧致裁切和居中处理，使用透明填充与统一描边，适合直接作为 `<img>`、CSS 背景或前端静态资源使用。图标保留了原始地图的坐标比例，但 `viewBox` 已按各自路径重新计算，因此不会带有整张地图的多余空白。

## 使用

```html
<img src="provinces/fujian.svg" alt="福建省" width="24" height="24">
```

可用文件名包括：

`anhui`、`beijing`、`chongqing`、`fujian`、`gansu`、`guangdong`、`guangxi`、`guizhou`、`hainan`、`hebei`、`heilongjiang`、`henan`、`hong-kong`、`hubei`、`hunan`、`inner-mongolia`、`jiangsu`、`jiangxi`、`jilin`、`liaoning`、`macau`、`ningxia`、`qinghai`、`shaanxi`、`shandong`、`shanghai`、`shanxi`、`sichuan`、`tianjin`、`tibet`、`xinjiang`、`yunnan`、`zhejiang`。

## 颜色与尺寸

图标默认使用 `#94a3b8` 描边，内部透明。若需要其他颜色，可以直接修改 SVG 中的 `stroke` 值。建议通过 `width` 和 `height` 控制显示尺寸，而不要修改路径数据。

## 来源说明

`china-provinces.svg` 基于用户提供的 Adobe Illustrator SVG 导出文件整理。单独图标由该源文件中的省级 `<g>` 路径提取，并重新计算 `viewBox`。如果你是原始制作者且希望补充署名或调整许可说明，请提交 issue 或 pull request。

## License

MIT License，详见 [LICENSE](./LICENSE)。
