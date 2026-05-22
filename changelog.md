# Changelog

## 2026-05-22 暗黑主题改版

### 重构
- 全站从粉红主题改为暗黑色系（#0a0a0a 底色 + #c9a96e 暖金点缀）
- 字体：Noto Serif SC + ZCOOL XiaoWei，文学质感

### 新增
- **一言风格首页**：全屏背景图 + 文学名句轮播（8秒切换，6组图文）
- **密码登录门**：全屏锁屏，SHA-256 校验，sessionStorage 保持登录态
- **拾光模块数据驱动**：`data/memories.json` 提供图文数据，自动渲染瀑布流
- **全部模块数据驱动**：一言(hitokoto)、时间线(timeline)、音乐(music)、地图(locations) 均 JSON 驱动
- **回忆详情弹窗**：点击拾光卡片弹出大图 + 文字详情

### 调整
- 倒计时从首页移至第二屏「时光」区块
- 地图瓦片改为 CARTO Dark 暗色底图
- 导航文字改为单字：序 / 时光 / 纪年 / 拾光 / 行迹 / 听风
- 回忆墙 hover 显示文字叠加层

### 数据文件
| 文件 | 说明 |
|------|------|
| `data/hitokoto.json` | 一言图文轮播数据 |
| `data/memories.json` | 拾光回忆墙数据（支持 `style: "tall"/"wide"` 布局） |
| `data/timeline.json` | 爱情时间线数据 |
| `data/music.json` | 音乐收藏数据 |
| `data/locations.json` | 旅行足迹坐标数据 |
