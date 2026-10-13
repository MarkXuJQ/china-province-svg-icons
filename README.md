# China Province SVG Icons

中国省级行政区 SVG 图标，提供两套精度版本，适合地点、旅行记录、生活随笔和地图界面。

## 目录

### `provinces/`（高精度，默认）

基于 DataV.GeoAtlas 省级 GeoJSON 生成。每个省份由地市级 `MultiPolygon` 边界组成，保留更多海岸线、地市边界和复杂轮廓细节。当前包含 34 个区域，包括台湾省、香港特别行政区和澳门特别行政区。

### `high-precision/provinces/`

高精度版本的明确目录，与根目录 `provinces/` 内容相同，便于在项目中显式选择版本。

### `low-precision/provinces/`

旧版低精度图标。它们来自用户提供的 Adobe Illustrator 中国地图 SVG，每个区域只有一条简化外轮廓路径，文件体积更小，适合对包体积敏感的场景。

### `china-provinces.svg`

旧版完整中国地图源文件，属于低精度版本的原始来源文件，继续保留以便追溯。

## 使用

```html
<!-- 高精度（默认） -->
<img src="provinces/fujian.svg" alt="福建省" width="24" height="24">

<!-- 低精度 -->
<img src="low-precision/provinces/fujian.svg" alt="福建省" width="24" height="24">
```

高精度图标文件名包括：

`anhui`、`beijing`、`chongqing`、`fujian`、`gansu`、`guangdong`、`guangxi`、`guizhou`、`hainan`、`hebei`、`heilongjiang`、`henan`、`hong-kong`、`hubei`、`hunan`、`inner-mongolia`、`jiangsu`、`jiangxi`、`jilin`、`liaoning`、`macau`、`ningxia`、`qinghai`、`shaanxi`、`shandong`、`shanghai`、`shanxi`、`sichuan`、`taiwan`、`tianjin`、`tibet`、`xinjiang`、`yunnan`、`zhejiang`。

所有单独图标都按自身边界重新计算 `viewBox` 并居中，使用透明填充和灰蓝色描边。可以直接通过 `width`、`height` 控制显示尺寸，也可以修改 SVG 中的 `stroke` 颜色。

## 高精度数据来源

高精度图标由 [zhChuXiao/ChinaGeoJson](https://github.com/zhChuXiao/ChinaGeoJson) 中的省级 GeoJSON 生成。该仓库说明数据来自阿里云 [DataV.GeoAtlas](https://datav.aliyun.com/portal/school/atlas/area_selector)，并以 MIT License 发布仓库内容。

由于地理边界数据来自上游服务，使用者应自行确认其项目对上游数据的再分发和商业使用要求。本仓库不对上游数据权利作额外保证。来源和生成说明见 [`sources/README.md`](./sources/README.md)。

## 低精度来源

`china-provinces.svg` 和 `low-precision/provinces/` 基于用户提供的 Adobe Illustrator SVG 导出文件整理。单独图标由其中的省级 `<g>` 路径提取，并重新计算 `viewBox`。

## License

仓库中的整理代码、文档和低精度图标使用 MIT License，详见 [LICENSE](./LICENSE)。高精度地理边界数据请同时遵守上游数据来源的条款。
