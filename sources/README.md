# Sources

高精度 SVG 来自省级 GeoJSON 的转换，而不是手工绘制。

源仓库：<https://github.com/zhChuXiao/ChinaGeoJson>

源目录：<https://github.com/zhChuXiao/ChinaGeoJson/tree/master/province>

数据说明：源仓库注明数据来自阿里云 DataV.GeoAtlas：<https://datav.aliyun.com/portal/school/atlas/area_selector>

生成方式：读取每个省级 GeoJSON 的 `FeatureCollection`，将各地市 `Polygon`/`MultiPolygon` 坐标转换为 SVG 路径，计算所有路径的紧致边界并加入少量留白，再输出透明填充的轮廓 SVG。高精度文件同时保留地市边界，因此放大查看时比低精度版本包含更多细节。

上游仓库当前标注 MIT License，但地理数据的再分发和商业使用仍应由使用者自行核对 DataV.GeoAtlas 的实际条款。
